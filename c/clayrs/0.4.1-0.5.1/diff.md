# Comparing `tmp/clayrs-0.4.1.tar.gz` & `tmp/clayrs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clayrs-0.4.1.tar", last modified: Mon Jun 12 09:58:37 2023, max compression
+gzip compressed data, was "clayrs-0.5.1.tar", last modified: Tue Jul  4 17:30:00 2023, max compression
```

## Comparing `clayrs-0.4.1.tar` & `clayrs-0.5.1.tar`

### file list

```diff
@@ -1,269 +1,304 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.777305 clayrs-0.4.1/
--rw-rw-rw-   0        0        0    35823 2023-06-12 09:52:17.000000 clayrs-0.4.1/LICENSE
--rw-rw-rw-   0        0        0       26 2023-06-12 09:52:17.000000 clayrs-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8186 2023-06-12 09:58:37.777305 clayrs-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     6977 2023-06-12 09:52:17.000000 clayrs-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.452087 clayrs-0.4.1/clayrs/
--rw-rw-rw-   0        0        0       80 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.497641 clayrs-0.4.1/clayrs/content_analyzer/
--rw-rw-rw-   0        0        0      777 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/__init__.py
--rw-rw-rw-   0        0        0    19919 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/config.py
--rw-rw-rw-   0        0        0    13001 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_analyzer_main.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.501662 clayrs-0.4.1/clayrs/content_analyzer/content_representation/
--rw-rw-rw-   0        0        0       28 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/__init__.py
--rw-rw-rw-   0        0        0    17711 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/content.py
--rw-rw-rw-   0        0        0     9660 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/content_representation/representation_container.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.504662 clayrs-0.4.1/clayrs/content_analyzer/embeddings/
--rw-rw-rw-   0        0        0      134 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.516769 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/
--rw-rw-rw-   0        0        0      259 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/__init__.py
--rw-rw-rw-   0        0        0     2015 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py
--rw-rw-rw-   0        0        0    12971 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py
--rw-rw-rw-   0        0        0     1918 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py
--rw-rw-rw-   0        0        0     2999 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py
--rw-rw-rw-   0        0        0     2716 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py
--rw-rw-rw-   0        0        0     2961 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py
--rw-rw-rw-   0        0        0     1791 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.525175 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/
--rw-rw-rw-   0        0        0      182 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/__init__.py
--rw-rw-rw-   0        0        0     3502 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py
--rw-rw-rw-   0        0        0     1265 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py
--rw-rw-rw-   0        0        0     1362 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py
--rw-rw-rw-   0        0        0     6168 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py
--rw-rw-rw-   0        0        0     2327 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py
--rw-rw-rw-   0        0        0     4182 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_source.py
--rw-rw-rw-   0        0        0      659 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/exceptions.py
--rw-rw-rw-   0        0        0    27437 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/exogenous_properties_retrieval.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.532183 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/
--rw-rw-rw-   0        0        0      251 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.536472 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/
--rw-rw-rw-   0        0        0      271 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py
--rw-rw-rw-   0        0        0    22732 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py
--rw-rw-rw-   0        0        0    17916 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py
--rw-rw-rw-   0        0        0     3346 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py
--rw-rw-rw-   0        0        0     7598 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.544383 clayrs-0.4.1/clayrs/content_analyzer/information_processor/
--rw-rw-rw-   0        0        0       84 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/__init__.py
--rw-rw-rw-   0        0        0    11229 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/ekphrasis.py
--rw-rw-rw-   0        0        0     2402 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/information_processor.py
--rw-rw-rw-   0        0        0    11713 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/nltk.py
--rw-rw-rw-   0        0        0    11797 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/information_processor/spacy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.548856 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/
--rw-rw-rw-   0        0        0       55 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5433 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py
--rw-rw-rw-   0        0        0    12924 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/text_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.555330 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/
--rw-rw-rw-   0        0        0      154 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/__init__.py
--rw-rw-rw-   0        0        0    31916 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/ratings.py
--rw-rw-rw-   0        0        0     2776 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/score_processor.py
--rw-rw-rw-   0        0        0     1163 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py
--rw-rw-rw-   0        0        0    14008 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/raw_information_source.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.559810 clayrs-0.4.1/clayrs/content_analyzer/utils/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/check_tokenization.py
--rw-rw-rw-   0        0        0     1252 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/content_analyzer/utils/id_merger.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.567256 clayrs-0.4.1/clayrs/evaluation/
--rw-rw-rw-   0        0        0      206 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/__init__.py
--rw-rw-rw-   0        0        0     6053 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_model.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.569324 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/
--rw-rw-rw-   0        0        0        2 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/__init__.py
--rw-rw-rw-   0        0        0     7634 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py
--rw-rw-rw-   0        0        0      158 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.580837 clayrs-0.4.1/clayrs/evaluation/metrics/
--rw-rw-rw-   0        0        0      412 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0    23860 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/classification_metrics.py
--rw-rw-rw-   0        0        0     7918 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/error_metrics.py
--rw-rw-rw-   0        0        0    23608 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/fairness_metrics.py
--rw-rw-rw-   0        0        0     1043 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/metrics.py
--rw-rw-rw-   0        0        0    26717 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/plot_metrics.py
--rw-rw-rw-   0        0        0    20138 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/metrics/ranking_metrics.py
--rw-rw-rw-   0        0        0     5220 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/statistical_test.py
--rw-rw-rw-   0        0        0     3696 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/evaluation/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.589179 clayrs-0.4.1/clayrs/recsys/
--rw-rw-rw-   0        0        0      528 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/__init__.py
--rw-rw-rw-   0        0        0      967 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.594184 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/
--rw-rw-rw-   0        0        0      224 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.598183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/
--rw-rw-rw-   0        0        0       89 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/__init__.py
--rw-rw-rw-   0        0        0    12467 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py
--rw-rw-rw-   0        0        0     1262 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.603180 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/
--rw-rw-rw-   0        0        0      171 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/__init__.py
--rw-rw-rw-   0        0        0    13108 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py
--rw-rw-rw-   0        0        0    12738 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py
--rw-rw-rw-   0        0        0    13336 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py
--rw-rw-rw-   0        0        0     3369 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/contents_loader.py
--rw-rw-rw-   0        0        0     1291 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.606183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/
--rw-rw-rw-   0        0        0       37 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/__init__.py
--rw-rw-rw-   0        0        0    13239 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.610183 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/
--rw-rw-rw-   0        0        0      204 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/__init__.py
--rw-rw-rw-   0        0        0    13600 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py
--rw-rw-rw-   0        0        0    12396 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py
--rw-rw-rw-   0        0        0    32721 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/experiment.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.613178 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/
--rw-rw-rw-   0        0        0       55 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/__init__.py
--rw-rw-rw-   0        0        0     5848 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.618328 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/
--rw-rw-rw-   0        0        0       38 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/__init__.py
--rw-rw-rw-   0        0        0    14333 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py
--rw-rw-rw-   0        0        0     3864 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.622328 clayrs-0.4.1/clayrs/recsys/graphs/
--rw-rw-rw-   0        0        0      123 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.628330 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/
--rw-rw-rw-   0        0        0      201 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0      138 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/exceptions.py
--rw-rw-rw-   0        0        0    12098 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py
--rw-rw-rw-   0        0        0     7116 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py
--rw-rw-rw-   0        0        0    10668 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/graph.py
--rw-rw-rw-   0        0        0      390 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/graph_metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.633660 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/
--rw-rw-rw-   0        0        0      145 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/__init__.py
--rw-rw-rw-   0        0        0    12188 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py
--rw-rw-rw-   0        0        0    11042 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py
--rw-rw-rw-   0        0        0    14361 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py
--rw-rw-rw-   0        0        0    12052 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/methodology.py
--rw-rw-rw-   0        0        0    14672 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/partitioning.py
--rw-rw-rw-   0        0        0    31969 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/recsys/recsys.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.646727 clayrs-0.4.1/clayrs/utils/
--rw-rw-rw-   0        0        0       77 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/__init__.py
--rw-rw-rw-   0        0        0     1223 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/automatic_methods.py
--rw-rw-rw-   0        0        0     1422 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/class_utils.py
--rw-rw-rw-   0        0        0      327 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/const.py
--rw-rw-rw-   0        0        0     1784 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/context_managers.py
--rw-rw-rw-   0        0        0     1313 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/custom_logger.py
--rw-rw-rw-   0        0        0     1852 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/load_content.py
--rw-rw-rw-   0        0        0    16554 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/report.py
--rw-rw-rw-   0        0        0     4166 2023-06-12 09:52:17.000000 clayrs-0.4.1/clayrs/utils/save_content.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.488671 clayrs-0.4.1/clayrs.egg-info/
--rw-rw-rw-   0        0        0     8186 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11194 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      440 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 09:58:37.000000 clayrs-0.4.1/clayrs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2023-06-12 09:52:18.000000 clayrs-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0      467 2023-06-12 09:52:18.000000 clayrs-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 09:58:37.779575 clayrs-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1691 2023-06-12 09:58:30.000000 clayrs-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.648738 clayrs-0.4.1/test/
--rw-rw-rw-   0        0        0       85 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.655269 clayrs-0.4.1/test/content_analyzer/
--rw-rw-rw-   0        0        0      114 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.660259 clayrs-0.4.1/test/content_analyzer/content_representation/
--rw-rw-rw-   0        0        0      114 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/__init__.py
--rw-rw-rw-   0        0        0     6125 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/test_content.py
--rw-rw-rw-   0        0        0     3165 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/content_representation/test_representation_container.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.662262 clayrs-0.4.1/test/content_analyzer/embeddings/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.674038 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/__init__.py
--rw-rw-rw-   0        0        0      837 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py
--rw-rw-rw-   0        0        0     5370 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py
--rw-rw-rw-   0        0        0      837 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py
--rw-rw-rw-   0        0        0     2596 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py
--rw-rw-rw-   0        0        0     2578 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py
--rw-rw-rw-   0        0        0     2492 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py
--rw-rw-rw-   0        0        0      835 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.679042 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py
--rw-rw-rw-   0        0        0     1015 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py
--rw-rw-rw-   0        0        0     7373 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py
--rw-rw-rw-   0        0        0     1464 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/embeddings/test_embedding_source.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.685241 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.689243 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
--rw-rw-rw-   0        0        0     1839 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py
--rw-rw-rw-   0        0        0     5328 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py
--rw-rw-rw-   0        0        0     5441 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py
--rw-rw-rw-   0        0        0      761 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py
--rw-rw-rw-   0        0        0     1123 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.694672 clayrs-0.4.1/test/content_analyzer/information_processor/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/__init__.py
--rw-rw-rw-   0        0        0     6760 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_ekphrasis.py
--rw-rw-rw-   0        0        0     4666 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_nlp.py
--rw-rw-rw-   0        0        0     5417 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/information_processor/test_spacy.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.697676 clayrs-0.4.1/test/content_analyzer/memory_interfaces/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/memory_interfaces/__init__.py
--rw-rw-rw-   0        0        0     5970 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/memory_interfaces/test_text_interface.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.703334 clayrs-0.4.1/test/content_analyzer/ratings_manager/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/__init__.py
--rw-rw-rw-   0        0        0     1634 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_rating_processor.py
--rw-rw-rw-   0        0        0    16379 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_ratings.py
--rw-rw-rw-   0        0        0      878 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py
--rw-rw-rw-   0        0        0     2861 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_config.py
--rw-rw-rw-   0        0        0    13832 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_content_analyzer_main.py
--rw-rw-rw-   0        0        0    12250 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_exogenous_properties_retrieval.py
--rw-rw-rw-   0        0        0    16062 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/test_raw_information_source.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.706735 clayrs-0.4.1/test/content_analyzer/utils/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/test_check_tokenization.py
--rw-rw-rw-   0        0        0      769 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/content_analyzer/utils/test_id_merger.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.712530 clayrs-0.4.1/test/evaluation/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.715633 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/__init__.py
--rw-rw-rw-   0        0        0     7197 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.722831 clayrs-0.4.1/test/evaluation/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/__init__.py
--rw-rw-rw-   0        0        0    37484 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_classification_metrics.py
--rw-rw-rw-   0        0        0     9022 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_error_metrics.py
--rw-rw-rw-   0        0        0    30699 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_fairness_metrics.py
--rw-rw-rw-   0        0        0    24104 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_plot_metrics.py
--rw-rw-rw-   0        0        0    18261 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/metrics/test_ranking_metrics.py
--rw-rw-rw-   0        0        0    11551 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_eval_model.py
--rw-rw-rw-   0        0        0    15955 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_statistical_tests.py
--rw-rw-rw-   0        0        0     3818 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/evaluation/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.730845 clayrs-0.4.1/test/recsys/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.734847 clayrs-0.4.1/test/recsys/content_based_algorithm/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.738842 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/__init__.py
--rw-rw-rw-   0        0        0     7435 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py
--rw-rw-rw-   0        0        0     1020 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.741844 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/__init__.py
--rw-rw-rw-   0        0        0     8845 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/test_classifier.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.745116 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/__init__.py
--rw-rw-rw-   0        0        0     7134 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/index_query/test_index_query.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.747113 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/__init__.py
--rw-rw-rw-   0        0        0     9912 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/regressor/test_regression.py
--rw-rw-rw-   0        0        0     4739 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/test_content_based_algorithm.py
--rw-rw-rw-   0        0        0     1887 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/content_based_algorithm/test_contents_loader.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.750115 clayrs-0.4.1/test/recsys/graph_based_algorithm/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.754113 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/__init__.py
--rw-rw-rw-   0        0        0     6780 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py
--rw-rw-rw-   0        0        0     5312 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py
--rw-rw-rw-   0        0        0     3161 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.756360 clayrs-0.4.1/test/recsys/graphs/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.760439 clayrs-0.4.1/test/recsys/graphs/feature_selection/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/__init__.py
--rw-rw-rw-   0        0        0     6561 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection.py
--rw-rw-rw-   0        0        0     7296 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py
--rw-rw-rw-   0        0        0     2288 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_graph.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.765582 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/__init__.py
--rw-rw-rw-   0        0        0    16619 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py
--rw-rw-rw-   0        0        0    14057 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py
--rw-rw-rw-   0        0        0    15747 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py
--rw-rw-rw-   0        0        0    19963 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_experiment.py
--rw-rw-rw-   0        0        0    17658 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_methodology.py
--rw-rw-rw-   0        0        0     8271 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_partitioning.py
--rw-rw-rw-   0        0        0    15538 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/recsys/test_recsys.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:58:37.775301 clayrs-0.4.1/test/utils/
--rw-rw-rw-   0        0        0      115 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/__init__.py
--rw-rw-rw-   0        0        0     2663 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_automatic_methods.py
--rw-rw-rw-   0        0        0     1105 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_class_utils.py
--rw-rw-rw-   0        0        0     1495 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_context_managers.py
--rw-rw-rw-   0        0        0      451 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_load_content.py
--rw-rw-rw-   0        0        0    10245 2023-06-12 09:52:18.000000 clayrs-0.4.1/test/utils/test_report.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.699079 clayrs-0.5.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-04 17:29:33.000000 clayrs-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-04 17:29:33.000000 clayrs-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8123 2023-07-04 17:30:00.699079 clayrs-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6965 2023-07-04 17:29:33.000000 clayrs-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.319683 clayrs-0.5.1/clayrs/
+-rw-rw-rw-   0        0        0       80 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.335787 clayrs-0.5.1/clayrs/content_analyzer/
+-rw-rw-rw-   0        0        0      777 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/__init__.py
+-rw-rw-rw-   0        0        0    20544 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/config.py
+-rw-rw-rw-   0        0        0    13302 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/content_analyzer_main.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.339347 clayrs-0.5.1/clayrs/content_analyzer/content_representation/
+-rw-rw-rw-   0        0        0       28 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/content_representation/__init__.py
+-rw-rw-rw-   0        0        0    18388 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/content_representation/content.py
+-rw-rw-rw-   0        0        0     9660 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/content_representation/representation_container.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.343351 clayrs-0.5.1/clayrs/content_analyzer/embeddings/
+-rw-rw-rw-   0        0        0      134 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.352819 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/
+-rw-rw-rw-   0        0        0      259 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/__init__.py
+-rw-rw-rw-   0        0        0     2015 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py
+-rw-rw-rw-   0        0        0    12984 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py
+-rw-rw-rw-   0        0        0     1918 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py
+-rw-rw-rw-   0        0        0     2999 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py
+-rw-rw-rw-   0        0        0     2716 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py
+-rw-rw-rw-   0        0        0     2961 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py
+-rw-rw-rw-   0        0        0     1791 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.363624 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/
+-rw-rw-rw-   0        0        0      182 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/__init__.py
+-rw-rw-rw-   0        0        0     3502 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py
+-rw-rw-rw-   0        0        0     1265 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py
+-rw-rw-rw-   0        0        0     1502 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py
+-rw-rw-rw-   0        0        0     6168 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py
+-rw-rw-rw-   0        0        0     2327 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py
+-rw-rw-rw-   0        0        0     4182 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_source.py
+-rw-rw-rw-   0        0        0     1411 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/exceptions.py
+-rw-rw-rw-   0        0        0    27437 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/exogenous_properties_retrieval.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.368644 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/
+-rw-rw-rw-   0        0        0      294 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.379189 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/
+-rw-rw-rw-   0        0        0      271 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py
+-rw-rw-rw-   0        0        0    23027 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py
+-rw-rw-rw-   0        0        0    18854 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py
+-rw-rw-rw-   0        0        0     3355 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py
+-rw-rw-rw-   0        0        0     7607 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.388244 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/visual_techniques/
+-rw-rw-rw-   0        0        0      243 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/visual_techniques/__init__.py
+-rw-rw-rw-   0        0        0     8268 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/visual_techniques/high_level_techniques.py
+-rw-rw-rw-   0        0        0    23415 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/visual_techniques/low_level_techniques.py
+-rw-rw-rw-   0        0        0    10331 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/visual_techniques/visual_content_techniques.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.398162 clayrs-0.5.1/clayrs/content_analyzer/information_processor/
+-rw-rw-rw-   0        0        0      186 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/__init__.py
+-rw-rw-rw-   0        0        0    11238 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/ekphrasis_processor.py
+-rw-rw-rw-   0        0        0     2683 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/information_processor_abstract.py
+-rw-rw-rw-   0        0        0    11722 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/nltk_processor.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.400160 clayrs-0.5.1/clayrs/content_analyzer/information_processor/postprocessors/
+-rw-rw-rw-   0        0        0       30 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/postprocessors/__init__.py
+-rw-rw-rw-   0        0        0    23345 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/postprocessors/postprocessor.py
+-rw-rw-rw-   0        0        0    12042 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/spacy_processor.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.403593 clayrs-0.5.1/clayrs/content_analyzer/information_processor/visual_preprocessors/
+-rw-rw-rw-   0        0        0       82 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/visual_preprocessors/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/visual_preprocessors/torch_builtin_augmenter.py
+-rw-rw-rw-   0        0        0    20112 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/information_processor/visual_preprocessors/torch_builtin_transformer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.410221 clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/
+-rw-rw-rw-   0        0        0       55 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5433 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py
+-rw-rw-rw-   0        0        0    12924 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/text_interface.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.415038 clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/
+-rw-rw-rw-   0        0        0      154 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/__init__.py
+-rw-rw-rw-   0        0        0    52932 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/ratings.py
+-rw-rw-rw-   0        0        0     2776 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/score_processor.py
+-rw-rw-rw-   0        0        0     1163 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py
+-rw-rw-rw-   0        0        0    14037 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/raw_information_source.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.417789 clayrs-0.5.1/clayrs/content_analyzer/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/utils/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/utils/check_tokenization.py
+-rw-rw-rw-   0        0        0     1256 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/content_analyzer/utils/id_merger.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.424756 clayrs-0.5.1/clayrs/evaluation/
+-rw-rw-rw-   0        0        0      206 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     6803 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/eval_model.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.428416 clayrs-0.5.1/clayrs/evaluation/eval_pipeline_modules/
+-rw-rw-rw-   0        0        0        2 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/eval_pipeline_modules/__init__.py
+-rw-rw-rw-   0        0        0     8084 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py
+-rw-rw-rw-   0        0        0      158 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.439634 clayrs-0.5.1/clayrs/evaluation/metrics/
+-rw-rw-rw-   0        0        0      412 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0    23806 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/classification_metrics.py
+-rw-rw-rw-   0        0        0     8371 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/error_metrics.py
+-rw-rw-rw-   0        0        0    24027 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/fairness_metrics.py
+-rw-rw-rw-   0        0        0     1724 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/metrics.py
+-rw-rw-rw-   0        0        0    26804 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/plot_metrics.py
+-rw-rw-rw-   0        0        0    24048 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/metrics/ranking_metrics.py
+-rw-rw-rw-   0        0        0     7758 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/statistical_test.py
+-rw-rw-rw-   0        0        0     3807 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/evaluation/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.454789 clayrs-0.5.1/clayrs/recsys/
+-rw-rw-rw-   0        0        0      567 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.463289 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/
+-rw-rw-rw-   0        0        0      224 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.467381 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/centroid_vector/
+-rw-rw-rw-   0        0        0       89 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/centroid_vector/__init__.py
+-rw-rw-rw-   0        0        0    13322 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py
+-rw-rw-rw-   0        0        0     1170 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/centroid_vector/similarities.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.471321 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/
+-rw-rw-rw-   0        0        0      171 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/__init__.py
+-rw-rw-rw-   0        0        0    13072 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py
+-rw-rw-rw-   0        0        0    12738 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py
+-rw-rw-rw-   0        0        0    46156 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py
+-rw-rw-rw-   0        0        0     3637 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/contents_loader.py
+-rw-rw-rw-   0        0        0     1291 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.474321 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/index_query/
+-rw-rw-rw-   0        0        0       37 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/index_query/__init__.py
+-rw-rw-rw-   0        0        0    14388 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.479459 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/
+-rw-rw-rw-   0        0        0      204 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/__init__.py
+-rw-rw-rw-   0        0        0    13919 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py
+-rw-rw-rw-   0        0        0    12396 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py
+-rw-rw-rw-   0        0        0    33451 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/experiment.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.482042 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/
+-rw-rw-rw-   0        0        0       55 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/__init__.py
+-rw-rw-rw-   0        0        0     5275 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.486051 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/page_rank/
+-rw-rw-rw-   0        0        0       38 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/page_rank/__init__.py
+-rw-rw-rw-   0        0        0    14200 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py
+-rw-rw-rw-   0        0        0     5668 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/page_rank/page_rank.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.490162 clayrs-0.5.1/clayrs/recsys/graphs/
+-rw-rw-rw-   0        0        0      123 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.495664 clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/
+-rw-rw-rw-   0        0        0      201 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/exceptions.py
+-rw-rw-rw-   0        0        0    12098 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py
+-rw-rw-rw-   0        0        0     7120 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py
+-rw-rw-rw-   0        0        0    10671 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/graph.py
+-rw-rw-rw-   0        0        0      390 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/graph_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.502204 clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/
+-rw-rw-rw-   0        0        0      145 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/__init__.py
+-rw-rw-rw-   0        0        0    12634 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py
+-rw-rw-rw-   0        0        0    11044 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py
+-rw-rw-rw-   0        0        0    14363 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py
+-rw-rw-rw-   0        0        0    16280 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/methodology.py
+-rw-rw-rw-   0        0        0    15721 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/partitioning.py
+-rw-rw-rw-   0        0        0    35069 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/recsys.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.503215 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/
+-rw-rw-rw-   0        0        0       19 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.514409 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/vbpr/
+-rw-rw-rw-   0        0        0       34 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/vbpr/__init__.py
+-rw-rw-rw-   0        0        0    25190 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/vbpr/vbpr_algorithm.py
+-rw-rw-rw-   0        0        0     5024 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/recsys/visual_based_algorithm/vbpr/vbpr_network.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.529100 clayrs-0.5.1/clayrs/utils/
+-rw-rw-rw-   0        0        0       77 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1223 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/automatic_methods.py
+-rw-rw-rw-   0        0        0     1422 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/class_utils.py
+-rw-rw-rw-   0        0        0      327 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/const.py
+-rw-rw-rw-   0        0        0     2845 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/context_managers.py
+-rw-rw-rw-   0        0        0     1313 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/custom_logger.py
+-rw-rw-rw-   0        0        0     1852 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/load_content.py
+-rw-rw-rw-   0        0        0    16643 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/report.py
+-rw-rw-rw-   0        0        0     4166 2023-07-04 17:29:33.000000 clayrs-0.5.1/clayrs/utils/save_content.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.328235 clayrs-0.5.1/clayrs.egg-info/
+-rw-rw-rw-   0        0        0     8123 2023-07-04 17:30:00.000000 clayrs-0.5.1/clayrs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13297 2023-07-04 17:30:00.000000 clayrs-0.5.1/clayrs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 17:30:00.000000 clayrs-0.5.1/clayrs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      589 2023-07-04 17:30:00.000000 clayrs-0.5.1/clayrs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-04 17:30:00.000000 clayrs-0.5.1/clayrs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2023-07-04 17:29:33.000000 clayrs-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      624 2023-07-04 17:29:33.000000 clayrs-0.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-04 17:30:00.700076 clayrs-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-07-04 17:29:33.000000 clayrs-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.530093 clayrs-0.5.1/test/
+-rw-rw-rw-   0        0        0      190 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.536598 clayrs-0.5.1/test/content_analyzer/
+-rw-rw-rw-   0        0        0      114 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.541113 clayrs-0.5.1/test/content_analyzer/content_representation/
+-rw-rw-rw-   0        0        0      114 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/content_representation/__init__.py
+-rw-rw-rw-   0        0        0     6125 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/content_representation/test_content.py
+-rw-rw-rw-   0        0        0     3165 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/content_representation/test_representation_container.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.544112 clayrs-0.5.1/test/content_analyzer/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.554361 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/__init__.py
+-rw-rw-rw-   0        0        0      847 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py
+-rw-rw-rw-   0        0        0     5380 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py
+-rw-rw-rw-   0        0        0      847 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py
+-rw-rw-rw-   0        0        0     2596 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py
+-rw-rw-rw-   0        0        0     2578 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py
+-rw-rw-rw-   0        0        0     2492 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py
+-rw-rw-rw-   0        0        0      845 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.561430 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/__init__.py
+-rw-rw-rw-   0        0        0     1682 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py
+-rw-rw-rw-   0        0        0     1015 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py
+-rw-rw-rw-   0        0        0     7373 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py
+-rw-rw-rw-   0        0        0     1464 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/embeddings/test_embedding_source.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.567025 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.574547 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
+-rw-rw-rw-   0        0        0     1839 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py
+-rw-rw-rw-   0        0        0     5360 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py
+-rw-rw-rw-   0        0        0     9823 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py
+-rw-rw-rw-   0        0        0      765 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py
+-rw-rw-rw-   0        0        0     1131 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.583608 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/visual_technique/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/visual_technique/__init__.py
+-rw-rw-rw-   0        0        0    13031 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/visual_technique/test_high_level_techniques.py
+-rw-rw-rw-   0        0        0    19518 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/visual_technique/test_low_level_techniques.py
+-rw-rw-rw-   0        0        0     9814 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/visual_technique/test_visual_content_technique.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.597076 clayrs-0.5.1/test/content_analyzer/information_processor/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/__init__.py
+-rw-rw-rw-   0        0        0     6770 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_ekphrasis.py
+-rw-rw-rw-   0        0        0     4676 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_nlp.py
+-rw-rw-rw-   0        0        0     5427 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_spacy.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.600596 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpostprocessors/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpostprocessors/__init__.py
+-rw-rw-rw-   0        0        0     9620 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpostprocessors/test_visualpostprocessor.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.603597 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpreprocessors/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpreprocessors/__init__.py
+-rw-rw-rw-   0        0        0     1260 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpreprocessors/test_torch_builtin_augmenter.py
+-rw-rw-rw-   0        0        0    11728 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/information_processor/test_visualpreprocessors/test_torch_builtin_transformer.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.606108 clayrs-0.5.1/test/content_analyzer/memory_interfaces/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/memory_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     5970 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/memory_interfaces/test_text_interface.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.613129 clayrs-0.5.1/test/content_analyzer/ratings_manager/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/ratings_manager/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/ratings_manager/test_rating_processor.py
+-rw-rw-rw-   0        0        0    41229 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/ratings_manager/test_ratings.py
+-rw-rw-rw-   0        0        0      878 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py
+-rw-rw-rw-   0        0        0     2861 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/test_config.py
+-rw-rw-rw-   0        0        0    10796 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/test_content_analyzer_main.py
+-rw-rw-rw-   0        0        0    12250 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/test_exogenous_properties_retrieval.py
+-rw-rw-rw-   0        0        0    16062 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/test_raw_information_source.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.615636 clayrs-0.5.1/test/content_analyzer/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/utils/test_check_tokenization.py
+-rw-rw-rw-   0        0        0      769 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/content_analyzer/utils/test_id_merger.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.621258 clayrs-0.5.1/test/evaluation/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.625846 clayrs-0.5.1/test/evaluation/eval_pipeline_modules/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/eval_pipeline_modules/__init__.py
+-rw-rw-rw-   0        0        0    14393 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/eval_pipeline_modules/test_metric_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.633435 clayrs-0.5.1/test/evaluation/metrics/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0    38574 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/test_classification_metrics.py
+-rw-rw-rw-   0        0        0     9024 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/test_error_metrics.py
+-rw-rw-rw-   0        0        0    31052 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/test_fairness_metrics.py
+-rw-rw-rw-   0        0        0    24092 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/test_plot_metrics.py
+-rw-rw-rw-   0        0        0    18617 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/metrics/test_ranking_metrics.py
+-rw-rw-rw-   0        0        0    11765 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/test_eval_model.py
+-rw-rw-rw-   0        0        0    21327 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/test_statistical_tests.py
+-rw-rw-rw-   0        0        0     4313 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/evaluation/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.647991 clayrs-0.5.1/test/recsys/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.652989 clayrs-0.5.1/test/recsys/content_based_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.661463 clayrs-0.5.1/test/recsys/content_based_algorithm/centroid_vector/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/centroid_vector/__init__.py
+-rw-rw-rw-   0        0        0     6217 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py
+-rw-rw-rw-   0        0        0     2764 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/centroid_vector/test_similarities.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.663464 clayrs-0.5.1/test/recsys/content_based_algorithm/classifier/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/classifier/__init__.py
+-rw-rw-rw-   0        0        0     7562 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/classifier/test_classifier.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.666015 clayrs-0.5.1/test/recsys/content_based_algorithm/index_query/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/index_query/__init__.py
+-rw-rw-rw-   0        0        0     5827 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/index_query/test_index_query.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.667569 clayrs-0.5.1/test/recsys/content_based_algorithm/regressor/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/regressor/__init__.py
+-rw-rw-rw-   0        0        0     7751 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/regressor/test_regression.py
+-rw-rw-rw-   0        0        0    22632 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/test_content_based_algorithm.py
+-rw-rw-rw-   0        0        0     1887 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/content_based_algorithm/test_contents_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.670577 clayrs-0.5.1/test/recsys/graph_based_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graph_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.673949 clayrs-0.5.1/test/recsys/graph_based_algorithm/page_rank/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graph_based_algorithm/page_rank/__init__.py
+-rw-rw-rw-   0        0        0    11501 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graph_based_algorithm/page_rank/test_nx_page_rank.py
+-rw-rw-rw-   0        0        0     5312 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py
+-rw-rw-rw-   0        0        0     3070 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.678006 clayrs-0.5.1/test/recsys/graphs/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.681015 clayrs-0.5.1/test/recsys/graphs/feature_selection/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/feature_selection/__init__.py
+-rw-rw-rw-   0        0        0     6561 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/feature_selection/test_feature_selection.py
+-rw-rw-rw-   0        0        0     7296 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py
+-rw-rw-rw-   0        0        0     3216 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/test_graph.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.686521 clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/__init__.py
+-rw-rw-rw-   0        0        0    16189 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py
+-rw-rw-rw-   0        0        0    14057 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py
+-rw-rw-rw-   0        0        0    15747 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py
+-rw-rw-rw-   0        0        0    20910 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/test_experiment.py
+-rw-rw-rw-   0        0        0    22395 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/test_methodology.py
+-rw-rw-rw-   0        0        0    13746 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/test_partitioning.py
+-rw-rw-rw-   0        0        0    23495 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/test_recsys.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.687027 clayrs-0.5.1/test/recsys/visual_based_algorithm/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/visual_based_algorithm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.689060 clayrs-0.5.1/test/recsys/visual_based_algorithm/vbpr/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/visual_based_algorithm/vbpr/__init__.py
+-rw-rw-rw-   0        0        0    16231 2023-07-04 17:29:33.000000 clayrs-0.5.1/test/recsys/visual_based_algorithm/vbpr/test_vbpr.py
+drwxrwxrwx   0        0        0        0 2023-07-04 17:30:00.698076 clayrs-0.5.1/test/utils/
+-rw-rw-rw-   0        0        0      115 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/__init__.py
+-rw-rw-rw-   0        0        0     2663 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/test_automatic_methods.py
+-rw-rw-rw-   0        0        0     1105 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/test_class_utils.py
+-rw-rw-rw-   0        0        0     1495 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/test_context_managers.py
+-rw-rw-rw-   0        0        0      451 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/test_load_content.py
+-rw-rw-rw-   0        0        0     9746 2023-07-04 17:29:34.000000 clayrs-0.5.1/test/utils/test_report.py
```

### Comparing `clayrs-0.4.1/LICENSE` & `clayrs-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/PKG-INFO` & `clayrs-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: clayrs
-Version: 0.4.1
+Version: 0.5.1
 Summary: Complexly represent contents, build recommender systems, evaluate them. All in one place!
 Home-page: https://github.com/swapUniba/ClayRS
 Author: Antonio Silletti, Elio Musacchio, Roberta Sallustio
 License: GPL-3.0
 Keywords: recommender system,cbrs,evaluation,recsys
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/26851363/172485577-be6993ef-47c3-4b3c-9187-4988f6c44d94.svg" alt="ClayRS logo" style="width:75%;"/>
 </p>
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
```

### Comparing `clayrs-0.4.1/README.md` & `clayrs-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/__init__.py` & `clayrs-0.5.1/clayrs/content_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/config.py` & `clayrs-0.5.1/clayrs/content_analyzer/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import re
 from abc import ABC
 from typing import List, Dict, Union, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.field_content_production_techniques.field_content_production_technique import \
         FieldContentProductionTechnique
-    from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+    from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
     from clayrs.content_analyzer.exogenous_properties_retrieval import ExogenousPropertiesRetrieval
     from clayrs.content_analyzer.memory_interfaces.memory_interfaces import InformationInterface
     from clayrs.content_analyzer.raw_information_source import RawInformationSource
+    from clayrs.content_analyzer.information_processor.visualpostprocessor import VisualPostProcessor
 
 from clayrs.content_analyzer.field_content_production_techniques.field_content_production_technique import \
     OriginalData
 
 
 class FieldConfig:
     """
@@ -76,31 +77,39 @@
         id: Custom id that can be used later by the user to easily refer to the representation generated by this config.
             IDs for a single field should be unique! And should only contain '_', '-' and alphanumeric characters
     """
 
     def __init__(self,
                  content_technique: FieldContentProductionTechnique = OriginalData(),
                  preprocessing: Union[InformationProcessor, List[InformationProcessor]] = None,
+                 postprocessing: Union[VisualPostProcessor, List[VisualPostProcessor]] = None,
                  memory_interface: InformationInterface = None,
                  id: str = None):
 
         if preprocessing is None:
             preprocessing = []
 
+        if postprocessing is None:
+            postprocessing = []
+
         if id is not None:
             self._check_custom_id(id)
 
         self.__content_technique = content_technique
         self.__preprocessing = preprocessing
+        self.__postprocessing = postprocessing
         self.__memory_interface = memory_interface
         self.__id = id
 
         if not isinstance(self.__preprocessing, list):
             self.__preprocessing = [self.__preprocessing]
 
+        if not isinstance(self.__postprocessing, list):
+            self.__postprocessing = [self.__postprocessing]
+
     @property
     def memory_interface(self):
         """
         Getter for the index associated to the field config
         """
         return self.__memory_interface
 
@@ -115,14 +124,21 @@
     def preprocessing(self):
         """
         Getter for the list of preprocessor of the field config
         """
         return self.__preprocessing
 
     @property
+    def postprocessing(self):
+        """
+        Getter for the list of postprocessor of the field config
+        """
+        return self.__postprocessing
+
+    @property
     def id(self):
         """
         Getter for the id of the field config
         """
         return self.__id
 
     def _check_custom_id(self, id: str):
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/content_analyzer_main.py` & `clayrs-0.5.1/clayrs/content_analyzer/content_analyzer_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 import json
 import pickle
 import re
 import lzma
 import os
 import shutil
 
-from typing import List, Dict, TYPE_CHECKING
+from typing import List, Dict, TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.config import ContentAnalyzerConfig
     from clayrs.content_analyzer.memory_interfaces.memory_interfaces import InformationInterface
 
 from clayrs.content_analyzer.content_representation.content import Content, IndexField, ContentEncoder
 from clayrs.utils.const import logger
-from clayrs.utils.context_managers import get_progbar
+from clayrs.utils.context_managers import get_iterator_thread
 from clayrs.content_analyzer.utils.id_merger import id_merger
 
 
 class ContentAnalyzer:
     """
     Class to whom the control of the content analysis phase is delegated. It uses the data stored in the configuration
     file to create and serialize the contents the user wants to produce. It also checks that the configurations the
     user wants to run on the raw contents have unique ids (otherwise it would be impossible to refer to a particular
     field representation or exogenous representation)
     Args:
         config (ContentAnalyzerConfig): configuration for processing the item fields. This parameter provides
             the possibility of customizing the way in which the input data is processed.
     """
 
-    def __init__(self, config: ContentAnalyzerConfig):
+    def __init__(self, config: ContentAnalyzerConfig, n_thread: int = 1):
         self._config: ContentAnalyzerConfig = config
+        self._n_thread = n_thread
 
     def set_config(self, config: ContentAnalyzerConfig):
         self._config = config
 
     def fit(self):
         """
         Processes the creation of the contents and serializes the contents. This method starts the content production
@@ -63,31 +64,33 @@
         created_contents = contents_producer.create_contents()
 
         if self._config.export_json:
             json_path = os.path.join(self._config.output_directory, 'contents.json')
             with open(json_path, "w") as data:
                 json.dump(created_contents, data, cls=ContentEncoder, indent=4)
 
-        with get_progbar(created_contents) as pbar:
+        # with get_progbar(created_contents) as pbar:
+        with get_iterator_thread(self._n_thread, self._serialize_content, created_contents,
+                                 keep_order=False, progress_bar=True, total=len(created_contents)) as pbar:
             pbar.set_description("Serializing contents")
 
-            for content in pbar:
-                self.__serialize_content(content)
+            for _ in pbar:
+                pass
 
-    def __serialize_content(self, content: Content):
+    def _serialize_content(self, content: Content):
         """
         This method serializes a specific content in the output directory defined by the content analyzer config
         Args:
             content (Content): content instance that will be serialized
         """
 
         file_name = re.sub(r'[^\w\s]', '', content.content_id)
         path = os.path.join(self._config.output_directory, file_name + '.xz')
         with lzma.open(path, 'wb') as f:
-            pickle.dump(content, f, protocol=4)
+            pickle.dump(content, f, protocol=pickle.HIGHEST_PROTOCOL)
 
     def __check_field_dict(self):
         """
         This function checks that there are no duplicate ids in the field_dict for a specific field_name.
         If this is not the case and a duplicate is found, a ValueError exception is thrown to warn the user.
         If the config id is None, the representation name will be kept as None even if it is not unique.
         So any case where the id is None is not considered.
@@ -134,15 +137,15 @@
         """
         # Static access method
         if ContentsProducer.__instance is None:
             ContentsProducer.__instance = ContentsProducer()
         return ContentsProducer.__instance
 
     def __init__(self):
-        self.__config: ContentAnalyzerConfig = None
+        self.__config: Optional[ContentAnalyzerConfig] = None
         # dictionary of memory interfaces defined in the FieldConfigs. The key is the directory of the memory interface
         # and the value is the memory interface itself (only one memory interface can be defined for each directory)
         # if a memory interface has an already defined directory, the memory interface associated to said directory
         # will be considered instead
         self.__memory_interfaces: Dict[InformationInterface] = {}
         # Virtually private constructor.
         if ContentsProducer.__instance is not None:
@@ -191,15 +194,15 @@
 
             for repr_number, field_config in enumerate(self.__config.get_configs_list(field_name)):
 
                 # technique_result is a list of field representation produced by the content technique
                 # each field repr in the list will refer to a content
                 # technique_result[0] -> contents_list[0]
                 technique_result = field_config.content_technique.produce_content(
-                    field_name, field_config.preprocessing, self.__config.source)
+                    field_name, field_config.preprocessing, field_config.postprocessing, self.__config.source)
 
                 if field_config.memory_interface is not None:
                     memory_interface = field_config.memory_interface
                     # if the index for the directory in the config hasn't been defined yet in the contents producer,
                     # the index associated to the field config that is being processed is added to the
                     # contents producer's memory interfaces list, and will be used for the future field configs with
                     # an assigned memory interface that has the same directory.
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/content_representation/content.py` & `clayrs-0.5.1/clayrs/content_analyzer/content_representation/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Dict, Union, List, Tuple, TYPE_CHECKING
 import numpy as np
 import json
+from numbers import Number
 
 from scipy import sparse
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.memory_interfaces.memory_interfaces import InformationInterface
 
 from clayrs.content_analyzer.content_representation.representation_container import RepresentationContainer
@@ -42,15 +43,15 @@
 class FeaturesBagField(FieldRepresentation):
     """
     Class for field representation using a bag of features.
     This class can also be used to represent a bag of words: <keyword, score>;
     this representation is produced by the EntityLinking and tf-idf techniques
 
     Args:
-        features (dict<str, object>): the dictionary where features are stored
+        sparse_scores: the sparse matrix where features are stored
     """
     __slots__ = ('__scores', '__pos_feature_tuples')
 
     def __init__(self, sparse_scores: sparse.csc_matrix, pos_feature_tuples: List[Tuple[int, str]]):
         self.__scores = sparse_scores
         self.__pos_feature_tuples = pos_feature_tuples
 
@@ -101,15 +102,15 @@
     def __repr__(self):
         return '{} - {}'.format(str(self), type(self.value))
 
     def __eq__(self, other):
         return self.__value == other.__value
 
 
-class EmbeddingField(FieldRepresentation):
+class EmbeddingField(FieldRepresentation, np.lib.mixins.NDArrayOperatorsMixin):
     """
     Class for field representation using embeddings (dense numeric vectors)
     this representation is produced by the EmbeddingTechnique.
 
     Examples:
         shape (4) = [x,x,x,x]
         shape (2,2) = [[x,x],
@@ -128,15 +129,32 @@
     def value(self) -> np.ndarray:
         return self.__dense_array
 
     def __str__(self):
         return np.array2string(self.__dense_array, threshold=np.inf, separator=',')
 
     def __eq__(self, other):
-        return self.__dense_array == other.__sparse_array
+        return self.__dense_array == other.__dense_array
+
+    def __array__(self, dtype=None):
+        return self.__dense_array.astype(dtype)
+
+    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+        if method == '__call__':
+            scalars = []
+            for input in inputs:
+                if isinstance(input, Number):
+                    scalars.append(input)
+                elif isinstance(input, self.__class__):
+                    scalars.append(input.value)
+                else:
+                    return NotImplemented
+            return self.__class__(ufunc(*scalars, **kwargs))
+        else:
+            return NotImplemented
 
 
 class IndexField(FieldRepresentation):
     """
     Class for field representation using an index.
     Allows to dynamically retrieve the contents representations serialized in an index.
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/content_representation/representation_container.py` & `clayrs-0.5.1/clayrs/content_analyzer/content_representation/representation_container.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/doc2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/embedding_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from abc import abstractmethod
 from typing import List, Union, TYPE_CHECKING
 
 import numpy as np
 from gensim.models import KeyedVectors
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+    from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
     from clayrs.content_analyzer.raw_information_source import RawInformationSource
 
 from clayrs.content_analyzer.embeddings.embedding_source import EmbeddingSource
 from clayrs.content_analyzer.utils.check_tokenization import check_tokenized, tokenize_in_sentences, check_not_tokenized
 from clayrs.utils.const import logger
 from clayrs.utils.context_managers import get_progbar
 
@@ -151,15 +151,15 @@
         Method that applies modifications to the data in order to fit the granularity of the technique
 
         Args:
             doc_data (str): data to be modified
 
         Returns:
             doc_data modified to fit the granularity. For example, if the technique had word granularity and doc_data
-            was "this is an example", the output would be ["this", "is", "an", "example"]
+                was "this is an example", the output would be ["this", "is", "an", "example"]
         """
         raise NotImplementedError
 
     @abstractmethod
     def save(self):
         """
         Saves the model in the path stored in the file_path attribute
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/fasttext.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/latent_semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/lda.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/random_indexing.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_learner/word2vec.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/embedding_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/gensim.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/sbert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sentence_transformers import SentenceTransformer
 import numpy as np
 
 from clayrs.content_analyzer.embeddings.embedding_loader.embedding_loader import SentenceEmbeddingLoader
+from clayrs.utils.const import logger
 
 
 class Sbert(SentenceEmbeddingLoader):
     """
     Class that produces sentences embeddings using sbert.
 
     The model will be automatically downloaded if not present locally.
@@ -16,25 +17,27 @@
     """
 
     def __init__(self, model_name_or_file_path: str = 'paraphrase-distilroberta-base-v1'):
         super().__init__(model_name_or_file_path)
 
     def load_model(self):
         try:
+            logger.info(f"Downloading/Loading {str(self)}")
+
             return SentenceTransformer(self.reference)
         except (OSError, AttributeError):
-            raise FileNotFoundError
+            raise FileNotFoundError("Model not found!")
 
     def get_vector_size(self) -> int:
         return self.model.get_sentence_embedding_dimension()
 
     def get_embedding(self, sentence: str) -> np.ndarray:
         return self.model.encode(sentence, show_progress_bar=False)
 
     def get_embedding_token(self, sentence: str) -> np.ndarray:
         raise NotImplementedError("The model chosen can't return token embeddings")
 
     def __str__(self):
-        return "Sbert"
+        return f"Sbert {self.reference}"
 
     def __repr__(self):
         return f"Sbert(model_name_or_file_path={self.reference})"
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/transformer.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_loader/vector_strategy.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/embeddings/embedding_source.py` & `clayrs-0.5.1/clayrs/content_analyzer/embeddings/embedding_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/exceptions.py` & `clayrs-0.5.1/clayrs/content_analyzer/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 from functools import wraps
 
+import numpy as np
 
-def Handler_ScoreNotFloat(func):
+
+def handler_score_not_float(func):
     """
     Handler that catches the above exception.
 
     Tries to run the functions normally, if one of the above exceptions is caught then it must return
     an empty frame for the user since predictions can't be calculated for it.
     """
     @wraps(func)
-    def Inner_Function(*args, **kwargs):
+    def inner_function(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except ValueError:
-            raise ValueError("The 'score' column must contains numbers!\n"
-                             "Try the same column with a score processor or change column!")
+            raise ValueError("The 'score' and 'timestamp' columns must contains numbers!\n"
+                             "Try to apply a score processor or change columns!") from None
+
+    return inner_function
+
+
+def handler_empty_matrix(dtype):
+
+    def handler_for_function(func):
+        """
+        Handler that catches the above exception.
+
+        Tries to run the functions normally, if one of the above exceptions is caught then it must return
+        an empty frame for the user since predictions can't be calculated for it.
+        """
+        @wraps(func)
+        def inner_function(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except IndexError:
+                return np.array([], dtype=dtype)
+
+        return inner_function
+
+    return handler_for_function
+
+
+class UserNone(Exception):
+    pass
+
 
-    return Inner_Function
+class ItemNone(Exception):
+    pass
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/exogenous_properties_retrieval.py` & `clayrs-0.5.1/clayrs/content_analyzer/exogenous_properties_retrieval.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py` & `clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py` & `clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     from clayrs.content_analyzer.embeddings.embedding_learner.embedding_learner import WordEmbeddingLearner, \
         SentenceEmbeddingLearner, DocumentEmbeddingLearner
     from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
         CombiningTechnique
     from clayrs.content_analyzer.embeddings.embedding_loader.embedding_loader import \
         WordEmbeddingLoader, SentenceEmbeddingLoader, DocumentEmbeddingLoader
     from clayrs.content_analyzer.embeddings.embedding_loader.embedding_loader import EmbeddingSource
-    from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+    from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
     from clayrs.content_analyzer.raw_information_source import RawInformationSource
+    from clayrs.content_analyzer.information_processor.visualpostprocessor import VisualPostProcessor
 
 from clayrs.content_analyzer.embeddings.embedding_learner.embedding_learner import EmbeddingLearner
 from clayrs.content_analyzer.content_representation.content import EmbeddingField
 from clayrs.content_analyzer.embeddings.embedding_loader.embedding_loader import EmbeddingLoader, EmbeddingSource
 from clayrs.content_analyzer.field_content_production_techniques.field_content_production_technique import \
     SingleContentTechnique
 from clayrs.content_analyzer.utils.check_tokenization import check_tokenized, tokenize_in_sentences, check_not_tokenized
@@ -80,14 +81,15 @@
                                 % embedding_source_str)
 
     @property
     def embedding_source(self):
         return self.__embedding_source
 
     def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[VisualPostProcessor],
                         source: RawInformationSource) -> List[FieldRepresentation]:
         representation_list: List[FieldRepresentation] = []
 
         if isinstance(self.__embedding_source, EmbeddingLoader) and self.__embedding_source.model is None:
             raise FileNotFoundError("The reference %s was not valid for the %s source" %
                                     (self.__embedding_source.reference, self.__embedding_source))
 
@@ -108,14 +110,16 @@
             for content_data in pbar:
 
                 pbar.set_description(f"Processing and producing contents with {self.__embedding_source}")
 
                 processed_data = self.process_data(content_data[field_name], preprocessor_list)
                 representation_list.append(self.produce_single_repr(processed_data))
 
+            representation_list = self.postprocess_representations(representation_list, postprocessor_list)
+
         self.embedding_source.unload_model()
         return representation_list
 
     @abstractmethod
     def produce_single_repr(self, field_data: Union[List[str], str]) -> EmbeddingField:
         """
         Method that builds the semantic content starting from the embeddings contained in field_data which can
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py` & `clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import List, Union, Callable, Optional, TYPE_CHECKING
 
+import numpy as np
 from scipy.sparse import csr_matrix
 
+from clayrs.utils.const import logger
+from clayrs.utils.context_managers import get_progbar
+
 if TYPE_CHECKING:
     from clayrs.content_analyzer.content_representation.content import FieldRepresentation
+    from clayrs.content_analyzer.information_processor.postprocessors.postprocessor import PostProcessor
 
-from clayrs.content_analyzer.content_representation.content import FeaturesBagField, SimpleField
-from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+from clayrs.content_analyzer.content_representation.content import FeaturesBagField, SimpleField, EmbeddingField
+from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
 from clayrs.content_analyzer.raw_information_source import RawInformationSource
 from clayrs.content_analyzer.utils.check_tokenization import check_not_tokenized
 
 
 class FieldContentProductionTechnique(ABC):
     """
     Generic abstract class used to define the techniques that can be applied to the content's fields in order to
@@ -38,16 +44,26 @@
         """
         processed_data = data
         for preprocessor in preprocessor_list:
             processed_data = preprocessor.process(processed_data)
 
         return processed_data
 
+    @staticmethod
+    def postprocess_representations(representations: List[FieldRepresentation],
+                                    postprocessor_list: List[PostProcessor]) -> List[FieldRepresentation]:
+        processed_list = representations
+        for postprocessor in postprocessor_list:
+            processed_list = postprocessor.process(processed_list)
+
+        return processed_list
+
     @abstractmethod
     def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[PostProcessor],
                         source: RawInformationSource) -> List[FieldRepresentation]:
         """
         Abstract method that defines the methodology used by a technique to produce a list of FieldRepresentation.
         This list of FieldRepresentation objects contains all the complex representations referring to a specific
         field for each content. So if there were 3 contents (in their original/raw form) passed to the method in total,
         there would be 3 elements in the list (one for each content) and each one of these elements would be the
         representation generated by the technique. The data contained in the field for each content is also
@@ -74,50 +90,73 @@
             the NLTK() processor will be applied to the data contained in the field 'Plot' for each content and, after
             this process, the field representation will be elaborated.
 
         Args:
              field_name (str): name of the contents' field on which the technique will be applied
              preprocessor_list (List[InformationProcessor]): list of information processors that will pre-process the
                 data contained in the field for each content
+             postprocessor_list (List[PostProcessor]): list of post-processors that will process the data generated by
+                the technique itself
             source (RawInformationSource): source where the raw data of the contents is stored
 
         Returns:
             representation_list(List[FieldRepresentation]): list containing the representations generated by the
                 technique for each content on a specific field
         """
         raise NotImplementedError
 
     @abstractmethod
+    def __str__(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def __repr__(self):
+        raise NotImplementedError
+
+
+class TextualContentTechnique(FieldContentProductionTechnique):
+
+    @abstractmethod
+    def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[PostProcessor],
+                        source: RawInformationSource) -> List[FieldRepresentation]:
+        raise NotImplementedError
+
+    @abstractmethod
     def __repr__(self):
         raise NotImplementedError
 
 
-class SingleContentTechnique(FieldContentProductionTechnique):
+class SingleContentTechnique(TextualContentTechnique):
     """
     Technique specialized in the production of representations that don't need any external information in order
     to be processed. This type of technique only considers the raw data within the content's field to create
     the complex representation
     """
 
     def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[PostProcessor],
                         source: RawInformationSource) -> List[FieldRepresentation]:
         """
         This method creates a list of FieldRepresentation objects, where each object is associated to a content
         and a specific field from the ones in said content. In order to do so, a simple preprocessing operation
         is done on the original data of the field (for each content) followed by the creation of the complex
         representation using the processed data. The complex representations are stored in a list and returned.
         """
         representation_list: List[FieldRepresentation] = []
 
-        # it iterates over all contents contained in the source in order to retrieve the raw data
-        # the data contained in the field_name is processed using each information processor in the processor_list
-        # the data is passed to the method that will create the single representation
-        for content_data in source:
-            processed_data = self.process_data(content_data[field_name], preprocessor_list)
-            representation_list.append(self.produce_single_repr(processed_data))
+        with get_progbar(list(source)) as pbar:
+            # it iterates over all contents contained in the source in order to retrieve the raw data
+            # the data contained in the field_name is processed using each information processor in the processor_list
+            # the data is passed to the method that will create the single representation
+            for content_data in pbar:
+                processed_data = self.process_data(content_data[field_name], preprocessor_list)
+                representation_list.append(self.produce_single_repr(processed_data))
+
+        representation_list = self.postprocess_representations(representation_list, postprocessor_list)
 
         return representation_list
 
     @abstractmethod
     def produce_single_repr(self, field_data: Union[List[str], str]) -> FieldRepresentation:
         """
         This method creates a single FieldRepresentation using the field data only (in the complete process made by the
@@ -128,22 +167,23 @@
 
         Returns:
             FieldRepresentation: complex representation created using the field data
         """
         raise NotImplementedError
 
 
-class CollectionBasedTechnique(FieldContentProductionTechnique):
+class CollectionBasedTechnique(TextualContentTechnique):
     """
     Technique specialized in the production of representations that are in need of the entire collection in order
     to be processed. This type of technique performs a refactoring operation on the original dataset,
     so that each content in the collection is modified accordingly to the technique's needs
     """
 
     def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[PostProcessor],
                         source: RawInformationSource) -> List[FieldRepresentation]:
         """
         This method creates a list of FieldRepresentation objects, where each object is associated to a content
         and a specific field from the ones in said content. In order to do so, the entire dataset where the original
         contents are stored has to be modified (and also processed using the preproccesors). After that, it re-creates
         the content_id for each content and uses it to retrieve the content from the refactored dataset. Finally, the
         refactored dataset is deleted.
@@ -156,14 +196,16 @@
 
         # produces the representation, retrieving it from the dataset given the content's position in the refactored
         # dataset
 
         for i in range(0, dataset_len):
             representation_list.append(self.produce_single_repr(i))
 
+        representation_list = self.postprocess_representations(representation_list, postprocessor_list)
+
         # once the operation is complete the refactored collection is deleted
         self.delete_refactored()
 
         return representation_list
 
     @abstractmethod
     def produce_single_repr(self, content_position: int) -> FieldRepresentation:
@@ -202,133 +244,117 @@
         """
         Once the content production phase is completed, the refactored dataset is useless. This method will delete the
         refactored dataset
         """
         raise NotImplementedError
 
 
-class OriginalData(FieldContentProductionTechnique):
+class OriginalData(SingleContentTechnique):
     """
     Technique used to retrieve the original data within the content's raw source without applying any
     processing operation.
 
     Note that if specified, preprocessing operations will still be applied!
 
     This technique is particularly useful if the user wants to keep the original
     data of the contents
 
     Args:
-        dtype: If specified, data will be casted to the chosen dtype
+        dtype: If specified, data will be cast to the chosen dtype
 
     """
 
     def __init__(self, dtype: Callable = str):
         super().__init__()
         self.__dtype = dtype
 
-    def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
-                        source: RawInformationSource) -> List[SimpleField]:
+    def produce_single_repr(self, field_data: Union[List[str], str]) -> SimpleField:
         """
         The contents' raw data in the given field_name is extracted and stored in a SimpleField object.
         The SimpleField objects created are stored in a list which is then returned.
         No further operations are done on the data in order to keep it in the original form.
         Because of that the preprocessor_list is ignored and not used by this technique
         """
+        return SimpleField(self.__dtype(check_not_tokenized(field_data)))
+
+    def __str__(self):
+        return "OriginalData"
+
+    def __repr__(self):
+        return f'OriginalData(dtype={self.__dtype})'
 
-        representation_list: List[SimpleField] = []
 
-        for content_data in source:
-            processed_data = self.process_data(content_data[field_name], preprocessor_list)
-            representation_list.append(SimpleField(self.__dtype(check_not_tokenized(processed_data))))
+class FromNPY(FieldContentProductionTechnique):
+    """
+    Technique used to import a collection of numpy arrays where each row will be treated as a separate
+    instance of data for the specified field
+
+    In this case, the expected field data from the source is a string representing an integer (that is the row of the
+    numpy collection corresponding to the representation associated to that content instance)
+
+    Note that if specified, preprocessing operations will ***NOT*** be applied! Preprocessing is skipped with this
+    technique
+
+    This technique is particularly useful if the user wants to import data generated by a different library
+
+    Args:
+        npy_file_path: Path where the numpy collection is stored
+
+    """
+
+    def __init__(self, npy_file_path: str):
+
+        self.npy_file_path = npy_file_path
+        self.np_matrix = np.load(npy_file_path)
+
+        if len(self.np_matrix) > 0:
+            self.dim_if_missing = self.np_matrix[0].shape
+        else:
+            raise ValueError('Matrix should have at least 1 row')
+
+        self._missing: Optional[int] = None
+
+    def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
+                        postprocessor_list: List[PostProcessor],
+                        source: RawInformationSource) -> List[FieldRepresentation]:
+
+        self._missing = 0
+
+        representation_list: List[FieldRepresentation] = []
+
+        with get_progbar(list(source)) as pbar:
+            # it iterates over all contents contained in the source in order to retrieve the raw data
+            # the data contained in the field_name is processed using each information processor in the processor_list
+            # the data is passed to the method that will create the single representation
+            for content_data in pbar:
+                representation_list.append(self.produce_single_repr(content_data[field_name]))
+
+        representation_list = self.postprocess_representations(representation_list, postprocessor_list)
+
+        if self._missing > 0:
+            logger.warning(f"{self._missing} items could not be mapped (non int index). Empty arrays will be used")
 
         return representation_list
 
-    def __repr__(self):
-        return f'OriginalData(dtype={self.__dtype})'
+    def produce_single_repr(self, field_data: Union[List[str], str]) -> EmbeddingField:
+        try:
+            index = int(field_data)
+        except ValueError:
+            raise ValueError(f'Values should be integers but {field_data} was found of type {type(field_data)}!')
+        try:
+            return EmbeddingField(self.np_matrix[index])
+        except IndexError:
+            raise IndexError(f'Specified index ({field_data}) is greater than number of '
+                             f'rows in matrix ({self.np_matrix.shape[0]}') from None
 
-# DECODE POSSIBLE REPRESENTATION: Not implemented for now
-#
-# class DefaultTechnique(FieldContentProductionTechnique):
-#     """
-#     Default technique used when no FieldContentProductionTechnique is defined in the FieldConfig.
-#     """
-#
-#     def __init__(self):
-#         super().__init__()
-#
-#     def produce_content(self, field_name: str, preprocessor_list: List[InformationProcessor],
-#                         source: RawInformationSource) -> List[FieldRepresentation]:
-#         """
-#         The content's raw data is decoded using the appropriate method (in case the data is not a string).
-#         Each decoded representation is added to a list which is then returned
-#         """
-#         representation_list: List[FieldRepresentation] = []
-#
-#         for content_data in source:
-#             # if a preprocessor is specified, then surely we must import the field data as a string,
-#             # there's no other option
-#             if len(preprocessor_list) != 0:
-#                 representation = SimpleField(check_not_tokenized(self.process_data(str(content_data[field_name]),
-#                                                                                    preprocessor_list)))
-#
-#             # If a preprocessor isn't specified, well maybe it is a complex representation:
-#             # let's decode what kind of complex representation it is and import it accordingly.
-#             else:
-#                 representation = self.__decode_field_data(str(content_data[field_name]))
-#
-#             representation_list.append(representation)
-#
-#         return representation_list
-#
-#     def __decode_field_data(self, field_data: str):
-#         # Decode string into dict or list
-#         try:
-#             loaded = json.loads(field_data)
-#         except json.JSONDecodeError:
-#             # in case the dict is {'foo': 1} json expects {"foo": 1}
-#             reformatted_field_data = field_data.replace("\'", "\"")
-#             try:
-#                 loaded = json.loads(reformatted_field_data)
-#             except json.JSONDecodeError:
-#                 # if it has issues decoding we consider the data as str
-#                 loaded = reformatted_field_data
-#
-#         # By default the representation decoded is what json tells us
-#         decoded = SimpleField(loaded)
-#
-#         # if the decoded is a list, maybe it is an EmbeddingField repr
-#         if isinstance(loaded, list):
-#             arr = np.array(loaded)
-#
-#             # if the array values has can be converted into floats then we consider it as a dense vector
-#             # else it is not and we do nothing
-#             try:
-#                 arr = arr.astype(float)
-#                 decoded = EmbeddingField(arr)
-#
-#             # Can't be converted
-#             except ValueError:
-#                 pass
-#
-#         # if the decoded is a dict, maybe it is a FeaturesBagField
-#         elif isinstance(loaded, dict):
-#             # if all values of the dict are numbers or can be converted into numbers,
-#             # then we consider it as a bag of words
-#             # else it is not and we do nothing
-#             if len(loaded.values()) != 0:
-#                 try:
-#                     dict_converted = {k: float(loaded[k]) for k in loaded}
-#
-#                     decoded = FeaturesBagField(dict_converted)
-#
-#                 # Can't be converted
-#                 except ValueError:
-#                     pass
-#
-#         return decoded
+    def __str__(self):
+        return "FromNPY"
+
+    def __repr__(self):
+        return f'FromNPY(npy_file_path={self.npy_file_path})'
 
 
 class TfIdfTechnique(CollectionBasedTechnique):
     """
     Abstract class that generalizes the implementations that produce a Bag of words with tf-idf metric
     """
 
@@ -358,14 +384,15 @@
         del self._feature_names
 
 
 class SynsetDocumentFrequency(CollectionBasedTechnique):
     """
     Abstract class that generalizes implementations that use synsets
     """
+
     def __init__(self):
         self._synset_matrix: Optional[csr_matrix] = None
         self._synset_names: Optional[List[str]] = None
 
     def produce_single_repr(self, content_position: int) -> FeaturesBagField:
         """
         Retrieves the tf-idf values, for terms in document in the defined content_position,
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py` & `clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import re
 from sklearn.feature_extraction.text import CountVectorizer
 from typing import List, TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+    from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
     from clayrs.content_analyzer.raw_information_source import RawInformationSource
 
 from clayrs.content_analyzer.field_content_production_techniques.field_content_production_technique import \
     SynsetDocumentFrequency
 from clayrs.content_analyzer.utils.check_tokenization import check_not_tokenized
 from clayrs.utils.context_managers import get_progbar
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py` & `clayrs-0.5.1/clayrs/content_analyzer/field_content_production_techniques/tf_idf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import numpy as np
 from sklearn.feature_extraction import DictVectorizer
 from sklearn.feature_extraction.text import TfidfVectorizer
 from typing import List, Union, Mapping, Iterable, Callable, TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer.information_processor.information_processor import InformationProcessor
+    from clayrs.content_analyzer.information_processor.information_processor_abstract import InformationProcessor
     from clayrs.content_analyzer.raw_information_source import RawInformationSource
 
 from clayrs.content_analyzer.field_content_production_techniques.field_content_production_technique \
     import TfIdfTechnique
 from clayrs.content_analyzer.memory_interfaces.text_interface import KeywordIndex
 from clayrs.content_analyzer.utils.check_tokenization import check_tokenized, check_not_tokenized
 from clayrs.utils.const import logger
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/information_processor/ekphrasis.py` & `clayrs-0.5.1/clayrs/content_analyzer/information_processor/ekphrasis_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ekphrasis.classes.tokenizer import SocialTokenizer
 from ekphrasis.classes.segmenter import Segmenter
 
 from ekphrasis.classes.preprocessor import TextPreProcessor
 from ekphrasis.classes.spellcorrect import SpellCorrector
 
-from clayrs.content_analyzer.information_processor.information_processor import NLP
+from clayrs.content_analyzer.information_processor.information_processor_abstract import NLP
 from clayrs.utils.automatic_methods import autorepr
 
 with warnings.catch_warnings():
     warnings.simplefilter(action='ignore', category=FutureWarning)
     social_tokenizer_ekphrasis = SocialTokenizer(lowercase=True).tokenize
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/information_processor/information_processor.py` & `clayrs-0.5.1/clayrs/content_analyzer/information_processor/information_processor_abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from abc import ABC, abstractmethod
-from typing import List
+from typing import List, Any
+
+import torch
 
 
 class InformationProcessor(ABC):
     """
     Abstract class that generalizes data processing.
     """
 
     @abstractmethod
-    def process(self, field_data):
+    def process(self, field_data: Any):
         raise NotImplementedError
 
     @abstractmethod
     def __eq__(self, other):
         raise NotImplementedError
 
     @abstractmethod
@@ -20,22 +22,28 @@
         raise NotImplementedError
 
     @abstractmethod
     def __repr__(self):
         raise NotImplementedError
 
 
-class ImageProcessor(InformationProcessor):
+class ImageProcessor(InformationProcessor, torch.nn.Module):
     """
     Abstract class for image processing.
     """
     @abstractmethod
-    def process(self, field_data):
+    def forward(self, field_data: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError
 
+    def process(self, field_data: torch.Tensor) -> torch.Tensor:
+        return self.forward(field_data)
+
+    def __eq__(self, other):
+        return torch.nn.Module.__eq__(self, other)
+
 
 class AudioProcessor(InformationProcessor):
     """
     Abstract class for audio processing.
     """
     @abstractmethod
     def process(self, field_data):
@@ -54,38 +62,38 @@
         Args: text (str): list of str
         Returns: str sentence
         """
         string_text = ' '.join([str(elem) for elem in text])
         return string_text
 
     @staticmethod
-    def string_to_list(text) -> List[str]:
+    def string_to_list(text: str) -> List[str]:
         """
         Covert str in list of str
         Args:
             text (str): str sentence
 
         Returns List <str>: List of words
         """
         list_text = list(text.split(" "))
         return list_text
 
     @abstractmethod
-    def process(self, field_data):
+    def process(self, field_data: str):
         raise NotImplementedError
 
 
 class NLP(TextProcessor):
     """
     Class for processing a text via Natural Language Processing.
 
     """
 
     @abstractmethod
-    def process(self, field_data) -> List[str]:
+    def process(self, field_data: str) -> List[str]:
         """
         Apply on the original text the required preprocessing steps
         Args:
             field_data: text on which NLP with specified phases will be applied
 
         Returns:
             list<str>: The text, after being processed with the specified NLP pipeline,
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/information_processor/nltk.py` & `clayrs-0.5.1/clayrs/content_analyzer/information_processor/nltk_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nltk import sent_tokenize
 from nltk.tokenize.toktok import ToktokTokenizer
 from nltk.corpus import stopwords
 from nltk.stem import WordNetLemmatizer
 from nltk.corpus import wordnet
 from nltk.stem.snowball import SnowballStemmer
 
-from clayrs.content_analyzer.information_processor.information_processor import NLP
+from clayrs.content_analyzer.information_processor.information_processor_abstract import NLP
 from clayrs.content_analyzer.utils.check_tokenization import check_not_tokenized
 
 
 class NLTK(NLP):
     """
     Interface to the NLTK library for natural language processing features.
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/information_processor/spacy.py` & `clayrs-0.5.1/clayrs/content_analyzer/information_processor/spacy_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from typing import List
-import spacy
-from spacy.tokens import Token
+import warnings
 
-from clayrs.content_analyzer.information_processor.information_processor import NLP
+# spacy has a bug which prints a useless warning if pytorch cuda is installed but no gpu is detected
+with warnings.catch_warnings():
+
+    warnings.filterwarnings("ignore", message="Can't initialize NVML")
+    import spacy
+    from spacy.tokens import Token
+
+from clayrs.content_analyzer.information_processor.information_processor_abstract import NLP
 from clayrs.content_analyzer.utils.check_tokenization import check_not_tokenized
 
 
 class Spacy(NLP):
     """
     Interface to the Spacy library for natural language processing features
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py` & `clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/memory_interfaces.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/memory_interfaces/text_interface.py` & `clayrs-0.5.1/clayrs/content_analyzer/memory_interfaces/text_interface.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/ratings.py` & `clayrs-0.5.1/clayrs/recsys/recsys.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,794 +1,746 @@
 from __future__ import annotations
-import functools
-import itertools
-import os
-from collections import defaultdict
-from pathlib import Path
-from typing import Dict, Union, List, Iterable, Iterator, TYPE_CHECKING
+import abc
+from typing import Union, Dict, List, Optional, TYPE_CHECKING, Set
 
-import pandas as pd
+from abc import ABC
 
-if TYPE_CHECKING:
-    from clayrs.content_analyzer.ratings_manager.score_processor import ScoreProcessor
-    from clayrs.content_analyzer.raw_information_source import RawInformationSource
+import numpy as np
 
-from clayrs.content_analyzer.exceptions import Handler_ScoreNotFloat
-from clayrs.utils.context_managers import get_progbar
-from clayrs.utils.save_content import get_valid_filename
+if TYPE_CHECKING:
+    from clayrs.content_analyzer import Ratings
+    from clayrs.recsys.graphs.graph import FullDiGraph, UserNode
+    from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
+    from clayrs.recsys.graph_based_algorithm.graph_based_algorithm import GraphBasedAlgorithm
+    from clayrs.recsys.methodology import Methodology
+
+from clayrs.content_analyzer.ratings_manager.ratings import Rank, Prediction
+from clayrs.recsys.methodology import TestRatingsMethodology, AllItemsMethodology
+from clayrs.recsys.content_based_algorithm.exceptions import NotFittedAlg
+from clayrs.utils.const import logger
 
 
-class Interaction:
+class RecSys(ABC):
     """
-    Class which models an interaction between a user and an item
+    Abstract class for a Recommender System
 
-    Each interaction has a score (a numeric value) and an optional timestamp
+    There exists various type of recommender systems, content-based, graph-based, etc. so extend this class
+    if another type must be implemented into the framework.
+
+    Every recommender system has an algorithm which is used to compute rank/score predictions
 
     Args:
-        user_id: ID of the user
-        item_id: ID of the item
-        score: Numeric value of the interaction
-        timestamp: Optional timestamp of the interaction
+        algorithm: The algorithm used to compute rank/score prediction
     """
-    __slots__ = ('_user_id', '_item_id', '_score', '_timestamp')
 
-    def __init__(self, user_id: str, item_id: str, score: float, timestamp: str = None):
-        self._user_id = user_id
-        self._item_id = item_id
-        self._score = score
-        self._timestamp = timestamp
+    def __init__(self, algorithm: Union[ContentBasedAlgorithm, GraphBasedAlgorithm]):
+        self.__alg = algorithm
 
-    @property
-    def user_id(self):
-        """
-        Getter for the `user_id` of the interaction
-        """
-        return self._user_id
+        self._yaml_report: Dict = {}
 
     @property
-    def item_id(self):
-        """
-        Getter for the `item_id` of the interaction
-        """
-        return self._item_id
+    def algorithm(self):
+        return self.__alg
 
-    @property
-    def score(self):
-        """
-        Getter for the `score` of the interaction
-        """
-        return self._score
+    @abc.abstractmethod
+    def rank(self, test_set: Ratings, n_recs: int = 10) -> Rank:
+        raise NotImplementedError
 
-    @property
-    def timestamp(self):
-        """
-        Getter for the `timestamp` of the interaction. Could be `None`
-        """
-        return self._timestamp
+    @abc.abstractmethod
+    def predict(self, test_set: Ratings) -> Prediction:
+        raise NotImplementedError
 
-    def __str__(self):
-        if self.timestamp is not None:
-            string = f"(user_id: {self.user_id}, item_id: {self.item_id}, score: {self.score}," \
-                     f" timestamp: {self.timestamp})"
-        else:
-            string = f"(user_id: {self.user_id}, item_id: {self.item_id}, score: {self.score})"
 
-        return string
+class ContentBasedRS(RecSys):
+    """
+    Class for recommender systems which use the items' content in order to make predictions,
+    some algorithms may also use users' content, so it's an optional parameter.
 
-    def __repr__(self):
-        return f"Interaction(user_id={self.user_id}, item_id={self.item_id}, score={self.score}, " \
-               f"timestamp={self.timestamp})"
+    Every *CBRS* differ from each other based the algorithm used.
 
-    def __eq__(self, other):
-        if isinstance(other, Interaction):
-            timestamp_equal = (self.timestamp is None and other.timestamp is None) or \
-                              (self.timestamp == other.timestamp)
+    Examples:
 
-            return self.user_id == other.user_id and self.item_id == other.item_id and \
-                   self.score == other.score and timestamp_equal
-        else:
-            return False
+        In case you perform a splitting of the dataset which returns a single train and test set (e.g. HoldOut
+        technique):
 
-    def __hash__(self):
-        return hash(self.user_id + self.item_id + str(self.score) + str(self.timestamp))
+        ```python title="Single split train"
+        from clayrs import recsys as rs
+        from clayrs import content_analyzer as ca
 
+        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
 
-class Ratings:
-    """
-    Class responsible of importing an interaction frame into the framework
+        [train], [test] = rs.HoldOutPartitioning().split_all(original_rat)
 
-    **If** the source file contains users, items and ratings in this order,
-    no additional parameters are needed, **otherwise** the mapping must be explicitly specified using:
+        alg = rs.CentroidVector()  # any cb algorithm
 
-    * **'user_id'** column,
-    * **'item_id'** column,
-    * **'score'** column
+        cbrs = rs.ContentBasedRS(alg, train, items_path)
 
-    The *score* column can also be processed: in case you would like to consider as score the sentiment of a textual
-    review, or maybe normalizing all scores in $[0, 1]$ range. Check the example below for more
+        rank = cbrs.fit_rank(test, n_recs=10)
+        ```
 
-    Examples:
+        In case you perform a splitting of the dataset which returns a multiple train and test sets (KFold technique):
 
-        ```title="CSV raw source"
-        user_id,item_id,rating,timestamp,review
-        u1,i1,4,00112,good movie
-        u2,i1,3,00113,an average movie
-        u2,i32,2,00114,a bad movie
-        ```
+        ```python title="Multiple split train"
+        from clayrs import recsys as rs
+        from clayrs import content_analyzer as ca
+
+        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
+
+        train_list, test_list = rs.KFoldPartitioning(n_splits=5).split_all(original_rat)
+
+        alg = rs.CentroidVector()  # any cb algorithm
 
-        As you can see the user id column, item id column and score column are the first three column and are already in
-        sequential order, so no additional parameter is required to the Ratings class:
+        for train_set, test_set in zip(train_list, test_list):
 
-        >>> import clayrs.content_analyzer as ca
-        >>> ratings_raw_source = ca.CSVFile('ratings.csv')
-        >>> # add timestamp='timestamp' to the following if
-        >>> # you want to load also the timestamp
-        >>> ratings = ca.Ratings(ratings_raw_source)
-
-        In case columns in the raw source are not in the above order you must specify an appropriate mapping via
-        positional index (useful in case your raw source doesn't have a header) or via column ids:
-
-        >>> # (mapping by index) EQUIVALENT:
-        >>> ratings = ca.Ratings(
-        >>> ca.CSVFile('ratings.csv'),
-        >>> user_id_column=0,  # (1)
-        >>> item_id_column=1,  # (2)
-        >>> score_column=2  # (3)
-        >>> )
-
-        1. First column of raw source is the column containing all user ids
-        2. Second column of raw source is the column containing all item ids
-        3. Third column of raw source is the column containing all the scores
-
-        >>> # (mapping by column name) EQUIVALENT:
-        >>> ratings = ca.Ratings(
-        >>> ca.CSVFile('ratings.csv'),
-        >>> user_id_column='user_id',  # (1)
-        >>> item_id_column='item_id',  # (2)
-        >>> score_column='rating'  # (3)
-        >>> )
-
-        1. The column with id 'user_id' of raw source is the column containing all user ids
-        2. The column with id 'item_id' of raw source is the column containing all item ids
-        3. The column with id 'rating' of raw source is the column containing all the scores
-
-
-        In case you would like to use the sentiment of the `review` column of the above raw source as score column,
-        simply specify the appropriate `ScoreProcessor` object
-
-        >>> ratings_raw_source = ca.CSVFile('ratings.csv')
-        >>> ratings = ca.Ratings(ratings_raw_source,
-        >>>                      score_column='review',
-        >>>                      score_processor=ca.TextBlobSentimentAnalysis())
+            cbrs = rs.ContentBasedRS(alg, train_set, items_path)
+            rank_to_append = cbrs.fit_rank(test_set)
+
+            result_list.append(rank_to_append)
+        ```
+
+        `result_list` will contain recommendation lists for each split
 
     Args:
-        source: Source containing the raw interaction frame
-        user_id_column: Name or positional index of the field of the raw source representing *users* column
-        item_id_column: Name or positional index of the field of the raw source representing *items* column
-        score_column: Name or positional index of the field of the raw source representing *score* column
-        timestamp_column: Name or positional index of the field of the raw source representing *timesamp* column
-        score_processor: `ScoreProcessor` object which will process the `score_column` accordingly. Useful if you want
-            to perform sentiment analysis on a textual column or you want to normalize all scores in $[0, 1]$ range
+        algorithm: the content based algorithm that will be used in order to
+            rank or make score prediction
+        train_set: a Ratings object containing interactions between users and items
+        items_directory: the path of the items serialized by the Content Analyzer
+        users_directory: the path of the users serialized by the Content Analyzer
     """
 
-    def __init__(self, source: RawInformationSource,
-                 user_id_column: Union[str, int] = 0,
-                 item_id_column: Union[str, int] = 1,
-                 score_column: Union[str, int] = 2,
-                 timestamp_column: Union[str, int] = None,
-                 score_processor: ScoreProcessor = None):
+    def __init__(self,
+                 algorithm: ContentBasedAlgorithm,
+                 train_set: Ratings,
+                 items_directory: str,
+                 users_directory: str = None):
 
-        self._ratings_dict = self._import_ratings(source, user_id_column, item_id_column, score_column,
-                                                  timestamp_column, score_processor)
+        super().__init__(algorithm)
+        self.__train_set = train_set
+        self.__items_directory = items_directory
+        self.__users_directory = users_directory
+        self.fit_alg = None
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def user_id_column(self) -> list:
+    def algorithm(self) -> ContentBasedAlgorithm:
         """
-        Getter for the user id column. This will return the user column "as is", so it will contain duplicate users.
-        Use set(user_id_column) to get all
-        unique users
-
-        Returns:
-            Users column with duplicates
+        The content based algorithm chosen
         """
-        return [interaction.user_id for interaction in self]
+        alg: ContentBasedAlgorithm = super().algorithm
+        return alg
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def item_id_column(self) -> list:
+    def train_set(self) -> Ratings:
         """
-        Getter for the user id column. This will return the item column "as is", so it will contain duplicate items.
-        Use set(item_id_column) to get all unique users
-
-        Returns:
-            Items column with duplicates
+        The train set of the Content Based RecSys
         """
-        return [interaction.item_id for interaction in self]
+        return self.__train_set
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def score_column(self) -> list:
+    def items_directory(self) -> str:
         """
-        Getter for the score column. This will return the score column "as is".
-
-        Returns:
-            Score column
+        Path of the serialized items by the Content Analyzer
         """
-        return [interaction.score for interaction in self]
+        return self.__items_directory
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def timestamp_column(self) -> list:
+    def users_directory(self) -> str:
+        """
+        Path of the serialized users by the Content Analyzer
         """
-        Getter for the timestamp column. This will return the score column "as is". If no timestamp is present then an
-        empty list is returned
+        return self.__users_directory
+
+    def fit(self, num_cpus: int = 1):
+        """
+        Method which will fit the algorithm chosen for each user in the train set passed in the constructor
+
+        If the algorithm can't be fit for some users, a warning message is printed showing the number of users
+        for which the alg couldn't be fit
+
+        Args:
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        Returns:
-            Timestamp column or empty list if no timestamp is present
         """
-        return [interaction.timestamp for interaction in self if interaction.timestamp is not None]
+        self.fit_alg = self.algorithm.fit(train_set=self.train_set,
+                                          items_directory=self.items_directory,
+                                          num_cpus=num_cpus)
 
-    @Handler_ScoreNotFloat
-    def _import_ratings(self, source: RawInformationSource,
-                        user_column: Union[str, int],
-                        item_column: Union[str, int],
-                        score_column: Union[str, int],
-                        timestamp_column: Union[str, int],
-                        score_processor: ScoreProcessor):
-        ratings_dict = defaultdict(list)
+        return self
 
-        with get_progbar(source) as pbar:
+    def rank(self, test_set: Ratings, n_recs: Optional[int] = 10, user_list: Union[List[str], List[int]] = None,
+             methodology: Optional[Methodology] = TestRatingsMethodology(),
+             num_cpus: int = 1) -> Rank:
 
-            pbar.set_description(desc="Importing ratings")
-            for row in pbar:
+        """
+        Method used to calculate ranking for all users in test set or all users in `user_list` parameter.
+        You must first call the `fit()` method ***before*** you can compute the ranking.
+        The `user_list` parameter could contain users with their string id or with their mapped integer
 
-                user_id = self._get_field_data(user_column, row)
-                item_id = self._get_field_data(item_column, row)
-                score = self._get_field_data(score_column, row)
-                timestamp = None
+        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
+        Otherwise, the rank will contain all unrated items of the particular users.
+        By default the ***top-10*** ranking is computed for each user
 
-                if score_processor is not None:
-                    score = score_processor.fit(score)
-                else:
-                    score = float(score)
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
 
-                if timestamp_column is not None:
-                    timestamp = self._get_field_data(timestamp_column, row)
+        If the algorithm was not fit for some users, they will be skipped and a warning message is printed showing the
+        number of users for which the alg couldn't produce a ranking
 
-                ratings_dict[user_id].append(Interaction(user_id, item_id, score, timestamp))
+        Args:
+            test_set: Ratings object which represents the ground truth of the split considered
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user. Default is 10 (top-10 for each user
+                will be computed)
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        # re-hashing
-        return dict(ratings_dict)
+        Raises:
+            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
 
-    def get_user_interactions(self, user_id: str, head: int = None) -> List[Interaction]:
+        Returns:
+            Rank object containing recommendation lists for all users of the test set or for all users in `user_list`
         """
-        Method which returns a list of `Interaction` objects for a single user, one for each interaction of the user.
-        Then you can easily iterate and extract useful information using list comprehension
 
-        Examples:
+        if self.fit_alg is None:
+            raise NotFittedAlg("Algorithm not fit! You must call the fit() method first, or fit_rank().")
 
-            So if the rating frame is the following:
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
 
-            ```
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u1      | i2      |     3 |
-            | u2      | i5      |     1 |
-            +---------+---------+-------+
-            ```
+        all_users = test_set.unique_user_idx_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, str):
+                all_users = self.train_set.user_map.convert_seq_str2int(all_users)
 
-            >>> rating_frame.get_user_interactions('u1')
-            [Interaction(user_id='u1', item_id='i1', score=4),
-            Interaction(user_id='u1', item_id='i2', score=3)]
+        all_users = set(all_users)
 
-            So you could easily extract all the ratings that a user has given for example:
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-            >>> [interaction.score for interaction in rating_frame.get_user_interactions('u1')]
-            [4, 3]
+        methodology.setup(self.train_set, test_set)
 
-            If you only want the first $k$ interactions of the user, set `head=k`. The interactions returned are the
-            first $k$ according to their order of appearance in the rating frame:
+        rank = self.algorithm.rank(self.fit_alg, self.train_set, test_set,
+                                   user_idx_list=all_users,
+                                   items_directory=self.items_directory, n_recs=n_recs,
+                                   methodology=methodology, num_cpus=num_cpus)
 
-            >>> rating_frame.get_user_interactions('u1', head=1)
-            [Interaction(user_id='u1', item_id='i1', score=4)]
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        rank = [uir_rank for uir_rank in rank if len(uir_rank) != 0]
 
-        Args:
-            user_id: User for which interactions must be extracted
-            head: Integer which will cut the list of interactions of the user returned. The interactions returned are
-                the first $k$ according to their order of appearance
+        # can't vstack when rank is empty
+        if len(rank) == 0:
+            rank = Rank.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return rank
 
-        Returns:
-            List of Interaction objects of a single user
+        rank = Rank.from_uir(np.vstack(rank), user_map=test_set.user_map, item_map=test_set.item_map)
 
-        """
-        return self._ratings_dict[user_id][:head]
+        self._yaml_report = {'mode': 'rank', 'n_recs': repr(n_recs), 'methodology': repr(methodology)}
 
-    def filter_ratings(self, user_list: Iterable[str]) -> Ratings:
+        return rank
+
+    def predict(self, test_set: Ratings, user_list: List = None,
+                methodology: Union[Methodology, None] = TestRatingsMethodology(),
+                num_cpus: int = 1) -> Prediction:
         """
-        Method which will filter the rating frame by keeping only interactions of users appearing in the `user_list`.
-        This method will return a new `Ratings` object without changing the original
-
-        Examples:
-
-            ```title="Starting Rating object"
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u1      | i2      |     3 |
-            | u2      | i5      |     1 |
-            +---------+---------+-------+
-            ```
-
-            >>> rating_frame.filter_ratings(['u1'])
-
-            ```title="Returned Rating object"
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u1      | i2      |     3 |
-            +---------+---------+-------+
-            ```
+        Method used to calculate score predictions for all users in test set or all users in `user_list` parameter.
+        You must first call the `fit()` method ***before*** you can compute score predictions.
+        The `user_list` parameter could contain users with their string id or with their mapped integer
 
-        Args:
-            user_list: List of user ids that will be present in the filtered `Ratings` object
+        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
 
-        Returns
-            The filtered Ratings object which contains only interactions of selected users
-        """
-        filtered_ratings_generator = ((user, self._ratings_dict[user]) for user in user_list)
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be considered for score
+        prediction
+
+        If the algorithm was not fit for some users, they will be skipped and a warning message is printed showing the
+        number of users for which the alg couldn't produce a ranking
+
+        Args:
+            test_set: Ratings object which represents the ground truth of the split considered
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        return self.from_dict(filtered_ratings_generator)
+        Raises:
+            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
 
-    def take_head_all(self, head: int) -> Ratings:
+        Returns:
+            Prediction object containing score prediction lists for all users of the test set or for all users in
+                `user_list`
         """
-        Method which will retain only $k$ interactions for each user. The $k$ interactions retained are the first which
-        appears in the rating frame.
 
-        This method will return a new `Ratings` object without changing the original
+        if self.fit_alg is None:
+            raise NotFittedAlg("Algorithm not fit! You must call the fit() method first, or fit_rank().")
 
-        Examples:
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
 
-            ```title="Starting Rating object"
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u1      | i2      |     3 |
-            | u2      | i5      |     1 |
-            | u2      | i6      |     2 |
-            +---------+---------+-------+
-            ```
+        all_users = test_set.unique_user_idx_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, str):
+                all_users = self.train_set.user_map.convert_seq_str2int(all_users)
 
-            >>> rating_frame.take_head_all(head=1)
+        all_users = set(all_users)
 
-            ```title="Returned Rating object"
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u2      | i5      |     1 |
-            +---------+---------+-------+
-            ```
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-        Args:
-            head: The number of interactions to retain for each user
+        methodology.setup(self.train_set, test_set)
 
-        Returns:
-            The filtered Ratings object which contains only first $k$ interactions for each user
-        """
+        pred = self.algorithm.predict(self.fit_alg, self.train_set, test_set,
+                                      user_idx_list=all_users,
+                                      items_directory=self.items_directory,
+                                      methodology=methodology, num_cpus=num_cpus)
 
-        ratings_cut_generator = ((user_id, user_ratings[:head])
-                                 for user_id, user_ratings in
-                                 zip(self._ratings_dict.keys(), self._ratings_dict.values()))
-
-        return self.from_dict(ratings_cut_generator)
-
-    # @Handler_ScoreNotFloat
-    # def add_score_column(self, score_column: Union[str, int], column_name: str,
-    #                      score_processor: ScoreProcessor = None):
-    #
-    #     col_to_add = [self._get_field_data(score_column, row) for row in self._source]
-    #
-    #     if score_processor:
-    #         col_to_add = score_processor.fit(col_to_add)
-    #     else:
-    #         col_to_add = [float(score) for score in col_to_add]
-    #
-    #     self._ratings_frame[column_name] = col_to_add
-    #
-    #     start_ratings_user = 0
-    #     for user_id, user_ratings in zip(self._ratings_dict.keys(), self._ratings_dict.values()):
-    #         first_range_val = start_ratings_user
-    #         second_range_val = start_ratings_user + len(user_ratings)
-    #
-    #         score_to_add = col_to_add[first_range_val:second_range_val]
-    #         new_ratings = [rating_tuple + (added_score,) for rating_tuple, added_score in
-    #                        zip(user_ratings, score_to_add)]
-    #         self._ratings_dict[user_id] = new_ratings
-    #
-    #         start_ratings_user += len(user_ratings)
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        pred = [uir_pred for uir_pred in pred if len(uir_pred) != 0]
 
-    def to_dataframe(self) -> pd.DataFrame:
-        """
-        Method which will convert the `Rating` object to a `pandas DataFrame object`.
+        # can't vstack when pred is empty
+        if len(pred) == 0:
+            pred = Prediction.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return pred
 
-        The returned DataFrame object will contain the 'user_id', 'item_id' and 'score' column and optionally the
-        'timestamp' column, if at least one interaction has a timestamp.
+        pred = Prediction.from_uir(np.vstack(pred), user_map=test_set.user_map, item_map=test_set.item_map)
 
-        Returns:
-            The rating frame converted to a pandas DataFrame with 'user_id', 'item_id', 'score' column and optionally
-            the 'timestamp' column
+        self._yaml_report = {'mode': 'score_prediction', 'methodology': repr(methodology)}
 
+        return pred
+
+    def fit_rank(self, test_set: Ratings, n_recs: int = 10, user_list: List[str] = None,
+                 methodology: Union[Methodology, None] = TestRatingsMethodology(),
+                 save_fit: bool = False, num_cpus: int = 1) -> Rank:
         """
-        will_be_frame = {'user_id': self.user_id_column,
-                         'item_id': self.item_id_column,
-                         'score': self.score_column}
+        Method used to both fit and calculate ranking for all users in test set or all users in `user_list`
+        parameter.
+        The Recommender System will first be fit for each user in the `test_set` parameter or for each
+        user inside the `user_list` parameter: the `user_list` parameter could contain users with their string id or
+        with their mapped integer
 
-        if len(self.timestamp_column) != 0:
-            will_be_frame['timestamp'] = self.timestamp_column
+        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
+        Otherwise, the rank will contain all unrated items of the particular users.
+        By default the ***top-10*** ranking is computed for each user
 
-        return pd.DataFrame(will_be_frame)
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
 
-    def to_csv(self, output_directory: str = '.', file_name: str = 'ratings_frame', overwrite: bool = False):
-        """
-        Method which will save the `Ratings` object to a `csv` file
+        If the algorithm couldn't be fit for some users, they will be skipped and a warning message is printed showing
+        the number of users for which the alg couldn't produce a ranking
 
-        Args:
-            output_directory: directory which will contain the csv file
-            file_name: Name of the csv_file
-            overwrite: If set to True and a csv file exists in the same output directory with the same file name, it
-                will be overwritten
-        """
-        Path(output_directory).mkdir(parents=True, exist_ok=True)
-
-        file_name = get_valid_filename(output_directory, file_name, 'csv', overwrite)
-
-        frame = self.to_dataframe()
-        frame.to_csv(os.path.join(output_directory, file_name), index=False, header=True)
-
-    @staticmethod
-    def _get_field_data(field_name: Union[str, int], row: Dict):
-        try:
-            if isinstance(field_name, str):
-                data = row[field_name]
-            else:
-                row_keys = list(row.keys())
-                key = row_keys[field_name]
-                data = row[key]
-
-        except KeyError:
-            raise KeyError("Column {} not found in the raw source".format(field_name))
-        except IndexError:
-            raise IndexError("Column index {} not present in the raw source".format(field_name))
-
-        return str(data)
-
-    @classmethod
-    def from_dataframe(cls, interaction_frame: pd.DataFrame,
-                       user_column: Union[str, int] = 0,
-                       item_column: Union[str, int] = 1,
-                       score_column: Union[str, int] = 2,
-                       timestamp_column: Union[str, int] = None) -> Ratings:
-        """
-        Class method which allows to instantiate a `Ratings` object by using an existing pandas DataFrame
-
-        **If** the pandas DataFrame contains users, items and ratings in this order,
-        no additional parameters are needed, **otherwise** the mapping must be explicitly specified using:
-
-        * **'user_id'** column,
-        * **'item_id'** column,
-        * **'score'** column
-
-        Check documentation of the `Ratings` class for examples on mapping columns explicitly, the functioning is the
-        same
-
-        Examples:
-
-            >>> ratings_df = pd.DataFrame({'user_id': ['u1', 'u1', 'u1'],
-            >>>                            'item_id': ['i1', 'i2', 'i3'],
-            >>>                            'score': [4, 3, 3])
-            >>> Ratings.from_dataframe(ratings_df)
+        With the `save_fit` parameter you can decide if you want that you recommender system remains *fit* even after
+        the complete execution of this method, in case you want to compute ranking with other methodologies, or
+        with a different `n_recs` parameter. Be mindful since it can be memory-expensive, thus by default this behaviour
+        is disabled
 
         Args:
-            interaction_frame: pandas DataFrame which represents the original interactions frame
-            user_column: Name or positional index of the field of the DataFrame representing *users* column
-            item_column: Name or positional index of the field of the DataFrame representing *items* column
-            score_column: Name or positional index of the field of the DataFrame representing *score* column
-            timestamp_column: Name or positional index of the field of the raw source representing *timesamp* column
+            test_set: Ratings object which represents the ground truth of the split considered
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user. Default is 10 (top-10 for each user
+                will be computed)
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            save_fit: Boolean value which let you choose if the Recommender System should remain fit even after the
+                complete execution of this method. Default is False
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
+
+        Raises:
+            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
 
         Returns:
-            `Ratings` object instantiated thanks to an existing Pandas DataFrame
+            Rank object containing recommendation lists for all users of the test set or for all users in `user_list`
         """
 
-        def get_value_row_df(row, column, dtype):
-            try:
-                if isinstance(column, str):
-                    value = row[column]
-                else:
-                    # it's an int, so we get the column id and then we get the corresponding value in the row
-                    key_dict = interaction_frame.columns[column]
-                    value = row[key_dict]
-            except (KeyError, IndexError) as e:
-                if isinstance(e, KeyError):
-                    raise KeyError(f"Column {column} not found in interaction frame!")
-                else:
-                    raise IndexError(f"Column {column} not found in interaction frame!")
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
+
+        all_users = test_set.unique_user_idx_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, str):
+                all_users = self.train_set.user_map.convert_seq_str2int(all_users)
 
-            return dtype(value) if value is not None else None
+        all_users = set(all_users)
 
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(Ratings, obj).__init__()  # Don't forget to call any polymorphic base class initializers
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-        ratings_dict = defaultdict(list)
+        methodology.setup(self.train_set, test_set)
 
-        if not interaction_frame.empty:
-            for row in interaction_frame.to_dict(orient='records'):
-                user_id = get_value_row_df(row, user_column, str)
-                item_id = get_value_row_df(row, item_column, str)
-                score = get_value_row_df(row, score_column, float)
-                timestamp = get_value_row_df(row, timestamp_column, str) if timestamp_column is not None else None
+        fit_alg, rank = self.algorithm.fit_rank(self.train_set, test_set, user_idx_list=all_users,
+                                                items_directory=self.items_directory, n_recs=n_recs,
+                                                methodology=methodology, num_cpus=num_cpus, save_fit=save_fit)
 
-                ratings_dict[user_id].append(Interaction(user_id, item_id, score, timestamp))
+        self.fit_alg = fit_alg
 
-        obj._ratings_dict = dict(ratings_dict)
-        return obj
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        rank = [uir_rank for uir_rank in rank if len(uir_rank) != 0]
 
-    @classmethod
-    def from_list(cls, interaction_list: Union[List[Interaction], Iterator]) -> Ratings:
+        # can't vstack when rank is empty
+        if len(rank) == 0:
+            rank = Rank.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return rank
+
+        rank = Rank.from_uir(np.vstack(rank), user_map=test_set.user_map, item_map=test_set.item_map)
+
+        self._yaml_report = {'mode': 'rank', 'n_recs': repr(n_recs), 'methodology': repr(methodology)}
+
+        return rank
+
+    def fit_predict(self, test_set: Ratings, user_list: List = None,
+                    methodology: Union[Methodology, None] = TestRatingsMethodology(),
+                    save_fit: bool = False, num_cpus: int = 1) -> Prediction:
         """
-        Class method which allows to instantiate a `Ratings` object by using an existing list containing `Interaction`
-        objects or its generator
+        Method used to both fit and calculate score prediction for all users in test set or all users in `user_list`
+        parameter.
+        The Recommender System will first be fit for each user in the `test_set` parameter or for each
+        user inside the `user_list` parameter: the `user_list` parameter could contain users with their string id or
+        with their mapped integer
 
-        Examples:
+        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
 
-            >>> interactions_list = [Interaction('u1', 'i1', 5), Interaction('u2', 'i1', 4)]
-            >>> Ratings.from_list(interactions_list)
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be considered for score
+        prediction
+
+        If the algorithm couldn't be fit for some users, they will be skipped and a warning message is printed showing
+        the number of users for which the alg couldn't produce a ranking
+
+        With the `save_fit` parameter you can decide if you want that you recommender system remains *fit* even after
+        the complete execution of this method, in case you want to compute ranking/score prediction with other
+        methodologies, or with a different `n_recs` parameter. Be mindful since it can be memory-expensive,
+        thus by default this behaviour is disabled
 
         Args:
-            interaction_list: List containing `Interaction` objects or its generator
+            test_set: Ratings object which represents the ground truth of the split considered
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            save_fit: Boolean value which let you choose if the Recommender System should remain fit even after the
+                complete execution of this method. Default is False
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
         Returns:
-            `Ratings` object instantiated thanks to an existing interaction list
+            Prediction object containing score prediction lists for all users of the test set or for all users in
+                `user_list`
         """
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(Ratings, obj).__init__()  # Don't forget to call any polymorphic base class initializers
 
-        ratings_dict = defaultdict(list)
-        for interaction in interaction_list:
-            ratings_dict[interaction.user_id].append(interaction)
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
 
-        obj._ratings_dict = dict(ratings_dict)
-        return obj
+        all_users = test_set.unique_user_idx_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, str):
+                all_users = self.train_set.user_map.convert_seq_str2int(all_users)
 
-    @classmethod
-    def from_dict(cls, interaction_dict: Union[Dict[str, List[Interaction]], Iterator]) -> Ratings:
-        """
-        Class method which allows to instantiate a `Ratings` object by using an existing dictionary containing
-        user_id as keys and lists of `Interaction` objects as value
+        all_users = set(all_users)
 
-        Examples:
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-            >>> interactions_dict = {'u1': [Interaction('u1', 'i2', 4), Interaction('u1', 'i3', 3)],
-            >>>                      'u2': [Interaction('u2', 'i2', 5)]}
-            >>> Ratings.from_dict(interactions_dict)
+        methodology.setup(self.train_set, test_set)
 
-        Args:
-            interaction_dict: Dictionary containing user_id as keys and lists of `Interaction` objets as values
-                or its generator
+        fit_alg, pred = self.algorithm.fit_predict(self.train_set, test_set, user_idx_list=all_users,
+                                                   items_directory=self.items_directory,
+                                                   methodology=methodology, num_cpus=num_cpus, save_fit=save_fit)
 
-        Returns:
-            `Ratings` object instantiated thanks to an existing dictionary
-        """
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(Ratings, obj).__init__()  # Don't forget to call any polymorphic base class initializers
+        self.fit_alg = fit_alg
+
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        pred = [uir_pred for uir_pred in pred if len(uir_pred) != 0]
+
+        # can't vstack when pred is empty
+        if len(pred) == 0:
+            pred = Prediction.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return pred
 
-        obj._ratings_dict = dict(interaction_dict)
-        return obj
+        pred = Prediction.from_uir(np.vstack(pred), user_map=test_set.user_map, item_map=test_set.item_map)
 
-    def __len__(self):
-        # all columns have same length, so only one is needed in order
-        # to check what is the length
-        return len(self.user_id_column)
+        self._yaml_report = {'mode': 'score_prediction', 'methodology': repr(methodology)}
 
-    def __str__(self):
-        return str(self.to_dataframe())
+        return pred
 
     def __repr__(self):
-        return repr(self._ratings_dict)
+        return f"ContentBasedRS(algorithm={self.algorithm}, train_set={self.train_set}, " \
+               f"items_directory={self.items_directory}, users_directory={self.users_directory})"
 
-    def __iter__(self):
-        """
-        The `Ratings` object can be iterated over and each iteration will return an `Interaction` object
 
-        Examples:
+class GraphBasedRS(RecSys):
+    """
+    Class for recommender systems which use a graph in order to make predictions
 
-            ```title="Rating object to iterate"
-            +---------+---------+-------+
-            | user_id | item_id | score |
-            +---------+---------+-------+
-            | u1      | i1      |     4 |
-            | u2      | i5      |     1 |
-            +---------+---------+-------+
-            ```
+    Every GBRS differ from each other based the algorithm used.
 
-            >>> # for simplicity we stop after the first iteration
-            >>> for interaction in ratings:
-            >>>     first_interaction = interaction
-            >>>     break
-            >>> first_interaction
-            Interaction('u1', 'i1', 4)
-        """
-        yield from itertools.chain.from_iterable(self._ratings_dict.values())
+    Examples:
 
+        In case you perform a splitting of the dataset which returns a single train and test set (e.g. HoldOut
+        technique):
 
-class RatingsLowMemory:
+        ```python title="Single split train"
+        from clayrs import recsys as rs
+        from clayrs import content_analyzer as ca
 
-    def __init__(self, source: RawInformationSource,
-                 user_id_column: Union[str, int] = 0,
-                 item_id_column: Union[str, int] = 1,
-                 score_column: Union[str, int] = 2,
-                 timestamp_column: Union[str, int] = None,
-                 score_processor: ScoreProcessor = None):
+        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
 
-        rat = pd.DataFrame(source, dtype=str)
-        self._ratings_dict = self._import_ratings(rat, user_id_column, item_id_column, score_column,
-                                                  timestamp_column, score_processor)
+        [train], [test] = rs.HoldOutPartitioning().split_all(original_rat)
 
-    @property
-    @functools.lru_cache(maxsize=128)
-    def user_id_column(self) -> list:
-        return self._ratings_dict.index.get_level_values('user_id').tolist()
+        alg = rs.NXPageRank()  # any gb algorithm
+
+        graph = rs.NXBipartiteGraph(original_rat)
+
+        # remove from the graph interaction of the test set
+        for user, item in zip(test.user_id_column, test.item_id_column):
+            user_node = rs.UserNode(user)
+            item_node = rs.ItemNode(item)
+
+            graph.remove_link(user_node, item_node)
+
+        gbrs = rs.GraphBasedRS(alg, graph)
+
+        rank = gbrs.rank(test, n_recs=10)
+        ```
+
+        In case you perform a splitting of the dataset which returns a multiple train and test sets (KFold technique):
+
+        ```python title="Multiple split train"
+        from clayrs import recsys as rs
+        from clayrs import content_analyzer as ca
+
+        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
+
+        train_list, test_list = rs.KFoldPartitioning(n_splits=5).split_all(original_rat)
+
+        alg = rs.NXPageRank()  # any gb algorithm
+
+        for train_set, test_set in zip(train_list, test_list):
+
+            graph = rs.NXBipartiteGraph(original_rat)
+
+            # remove from the graph interaction of the test set
+            for user, item in zip(test_set.user_id_column, test_set.item_id_column):
+                user_node = rs.UserNode(user)
+                item_node = rs.ItemNode(item)
+
+                graph.remove_link(user_node, item_node)
+
+            gbrs = rs.GraphBasedRS(alg, graph)
+            rank_to_append = gbrs.rank(test_set)
+
+            result_list.append(rank_to_append)
+        ```
+
+        `result_list` will contain recommendation lists for each split
+
+    Args:
+        algorithm: the graph based algorithm that will be used in order to
+            rank or make score prediction
+        graph: A graph which models interactions of users and items
+    """
+
+    def __init__(self,
+                 algorithm: GraphBasedAlgorithm,
+                 graph: FullDiGraph):
+
+        self.__graph = graph
+        super().__init__(algorithm)
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def item_id_column(self) -> list:
-        return self._ratings_dict.index.get_level_values('item_id').tolist()
+    def users(self) -> Set[UserNode]:
+        """
+        Set of UserNode objects for each user of the graph
+        """
+        return self.__graph.user_nodes
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def score_column(self) -> list:
-        return self._ratings_dict['score'].tolist()
+    def graph(self) -> FullDiGraph:
+        """
+        The graph containing interactions
+        """
+        return self.__graph
 
     @property
-    @functools.lru_cache(maxsize=128)
-    def timestamp_column(self) -> list:
-        timestamp_list = self._ratings_dict['timestamp'].tolist()
-        return timestamp_list if all(timestamp is not None for timestamp in timestamp_list) else []
-
-    @Handler_ScoreNotFloat
-    def _import_ratings(self, rat: pd.DataFrame,
-                        user_column: Union[str, int],
-                        item_column: Union[str, int],
-                        score_column: Union[str, int],
-                        timestamp_column: Union[str, int],
-                        score_processor: ScoreProcessor):
+    def algorithm(self) -> GraphBasedAlgorithm:
         """
-        Imports the ratings from the source and stores in a dataframe
+        The graph based algorithm chosen
+        """
+        alg: GraphBasedAlgorithm = super().algorithm
+        return alg
 
-        Returns:
-            ratings_frame: pd.DataFrame
+    def rank(self, test_set: Ratings, n_recs: int = 10, user_list: List[str] = None,
+             methodology: Union[Methodology, None] = TestRatingsMethodology(),
+             num_cpus: int = 1) -> Rank:
         """
-        if isinstance(user_column, int):
-            user_column = rat.columns[user_column]
-        if isinstance(item_column, int):
-            item_column = rat.columns[item_column]
-        if isinstance(score_column, int):
-            score_column = rat.columns[score_column]
-        if isinstance(timestamp_column, int):
-            timestamp_column = rat.columns[timestamp_column]
-        elif timestamp_column is None:
-            rat['timestamp'] = None
-            timestamp_column = 'timestamp'
+        Method used to calculate ranking for all users in test set or all users in `user_list` parameter.
+        The `user_list` parameter could contain users with their string id or with their mapped integer
 
-        index = pd.MultiIndex.from_tuples(zip(rat[user_column].values, rat[item_column].values),
-                                          names=["user_id", "item_id"])
+        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
+        Otherwise, the rank will contain all unrated items of the particular users.
+        By default the ***top-10*** ranking is computed for each user
 
-        rat = rat[[score_column, timestamp_column]].set_index(index)
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
 
-        rat.columns = ['score', 'timestamp']
+        If the algorithm couldn't produce a ranking for some users, they will be skipped and a warning message is
+        printed showing the number of users for which the alg couldn't produce a ranking
 
-        rat['score'] = pd.to_numeric(rat['score'])
+        Args:
+            test_set: Ratings object which represents the ground truth of the split considered
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user. Default is 10 (top-10 for each user
+                will be computed)
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        return rat
+        Returns:
+            Rank object containing recommendation lists for all users of the test set or for all users in `user_list`
+        """
 
-    def get_user_interactions(self, user_id: str, head: int = None):
-        user_rat = self._ratings_dict.loc[user_id][:head]
+        train_set = self.graph.to_ratings(user_map=test_set.user_map, item_map=test_set.item_map)
 
-        user_rat = [Interaction(user_id, index_item, row[0], row[1])
-                    for index_item, row in zip(user_rat.index, user_rat.values)]
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
 
-        return user_rat
+        # in the graph recsys, each graph algorithm works with strings,
+        # so in case we should convert int to strings
+        all_users = test_set.unique_user_id_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, int):
+                all_users = train_set.user_map.convert_seq_int2str(all_users)
 
-    def filter_ratings(self, user_list: Iterable[str]):
-        filtered_df = self._ratings_dict.loc[
-            (self._ratings_dict.index.get_level_values('user_id').isin(set(user_list)))]
+        all_users = set(all_users)
 
-        filtered_df = filtered_df.reset_index(drop=False)
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-        return self.from_dataframe(filtered_df, user_column='user_id',
-                                   item_column='item_id',
-                                   score_column='score',
-                                   timestamp_column='timestamp')
+        methodology.setup(train_set, test_set)
 
-    def take_head_all(self, head: int):
+        rank = self.algorithm.rank(self.graph, train_set, test_set, all_users, n_recs, methodology, num_cpus)
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        rank = [uir_rank for uir_rank in rank if len(uir_rank) != 0]
 
-        filtered_df = self._ratings_dict.groupby(level='user_id').head(head)
+        # can't vstack when rank is empty
+        if len(rank) == 0:
+            rank = Rank.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return rank
 
-        filtered_df = filtered_df.reset_index(drop=False)
+        rank = np.vstack(rank)
 
-        return self.from_dataframe(filtered_df, user_column='user_id',
-                                   item_column='item_id',
-                                   score_column='score',
-                                   timestamp_column='timestamp')
+        # convert back strings and Nodes object to ints
+        rank_users_idx = train_set.user_map.convert_seq_str2int(rank[:, 0])
+        rank_items_idx = train_set.item_map.convert_seq_str2int([item_node.value for item_node in rank[:, 1]])
+        rank[:, 0] = rank_users_idx
+        rank[:, 1] = rank_items_idx
+        rank = rank.astype(np.float64)
 
-    @classmethod
-    def from_dataframe(cls, interaction_frame: pd.DataFrame,
-                       user_column: Union[str, int] = 0,
-                       item_column: Union[str, int] = 1,
-                       score_column: Union[str, int] = 2,
-                       timestamp_column: Union[str, int] = None):
+        rank = Rank.from_uir(rank, user_map=test_set.user_map, item_map=test_set.item_map)
 
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(RatingsLowMemory, obj).__init__()  # Don't forget to call any polymorphic base class initializers
+        if len(rank) == 0:
+            logger.warning("No items could be ranked for any users! Remember that items to rank must be present "
+                           "in the graph.\n"
+                           "Try changing methodology!")
 
-        ratings_dict = cls._import_ratings(obj, interaction_frame, user_column, item_column, score_column,
-                                           timestamp_column, None)
+        elif len(rank.unique_user_id_column) != len(all_users):
+            logger.warning(f"No items could be ranked for users {all_users - set(rank.user_id_column)}\n"
+                           f"No nodes to rank for them found in the graph. Try changing methodology! ")
 
-        obj._ratings_dict = ratings_dict
-        return obj
+        self._yaml_report = {'graph': repr(self.graph), 'mode': 'rank', 'n_recs': repr(n_recs),
+                             'methodology': repr(methodology)}
 
-    @classmethod
-    def from_list(cls, interaction_list: List[Interaction]):
+        return rank
 
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(RatingsLowMemory, obj).__init__()  # Don't forget to call any polymorphic base class initializers
+    def predict(self, test_set: Ratings, user_list: List[str] = None,
+                methodology: Union[Methodology, None] = TestRatingsMethodology(),
+                num_cpus: int = 1) -> Prediction:
+        """
+        Method used to calculate score predictions for all users in test set or all users in `user_list` parameter.
+        The `user_list` parameter could contain users with their string id or with their mapped integer
 
-        user_column_iterator = (interaction.user_id for interaction in interaction_list)
-        item_column_iterator = (interaction.item_id for interaction in interaction_list)
+        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
 
-        index = pd.MultiIndex.from_tuples(zip(user_column_iterator, item_column_iterator),
-                                          names=["user_id", "item_id"])
+        Via the `methodology` parameter you can perform different candidate item selection. By default, the
+        `TestRatingsMethodology()` is used: so for each user items in its test set only will be considered for score
+        prediction
 
-        score_timestamp_iterator = ({'score': interaction.score, 'timestamp': interaction.timestamp}
-                                    for interaction in interaction_list)
+        If the algorithm couldn't perform score prediction for some users, they will be skipped and a warning message is
+        printed showing the number of users for which the alg couldn't produce a score prediction
 
-        rat = pd.DataFrame(score_timestamp_iterator, index=index)
+        Args:
+            test_set: Ratings object which represents the ground truth of the split considered
+            user_list: List of users for which you want to compute score prediction. If None, the ranking
+                will be computed for all users of the `test_set`. The list should contain user id as strings or user ids
+                mapped to their integers
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        obj._ratings_dict = rat
-        return obj
+        Returns:
+            Prediction object containing score prediction lists for all users of the test set or for all users in
+                `user_list`
+        """
 
-    @classmethod
-    def from_dict(cls, interaction_dict: Dict[str, List[Interaction]]):
-        obj = cls.__new__(cls)  # Does not call __init__
-        super(RatingsLowMemory, obj).__init__()  # Don't forget to call any polymorphic base class initializers
+        train_set = self.graph.to_ratings(user_map=test_set.user_map, item_map=test_set.item_map)
 
-        obj._ratings_dict = dict(interaction_dict)
-        return obj
+        logger.info("Don't worry if it looks stuck at first")
+        logger.info("First iterations will stabilize the estimated remaining time")
 
-    def __iter__(self):
-        yield from itertools.chain.from_iterable(self.get_user_interactions(user_id)
-                                                 for user_id in
-                                                 self._ratings_dict.index.get_level_values('user_id').unique())
+        # in the graph recsys, each graph algorithm works with strings,
+        # so in case we should convert int to strings
+        all_users = test_set.unique_user_id_column
+        if user_list is not None:
+            all_users = np.array(user_list)
+            if np.issubdtype(all_users.dtype, int):
+                all_users = train_set.user_map.convert_seq_int2str(all_users)
 
-    def __len__(self):
-        return len(self._ratings_dict)
+        all_users = set(all_users)
 
+        if methodology is None:
+            methodology = AllItemsMethodology()
 
-# Aliases for the Ratings class
+        methodology.setup(train_set, test_set)
 
-class Prediction(Ratings):
-    """
-    This class is just an alias for the `Ratings` class, it has exactly same functionalities
-    """
-    pass
+        pred = self.algorithm.predict(self.graph, train_set, test_set, all_users, methodology, num_cpus)
+        # we should remove empty uir matrices otherwise vstack won't work due to dimensions mismatch
+        pred = [uir_pred for uir_pred in pred if len(uir_pred) != 0]
 
+        # can't vstack when pred is empty
+        if len(pred) == 0:
+            pred = Prediction.from_uir(np.array([]), user_map=test_set.user_map, item_map=test_set.item_map)
+            return pred
 
-class Rank(Ratings):
-    """
-    This class is just an alias for the `Ratings` class, it has exactly same functionalities
-    """
-    pass
+        pred = np.vstack(pred)
+        pred_users_idx = train_set.user_map.convert_seq_str2int(pred[:, 0])
+        pred_items_idx = train_set.item_map.convert_seq_str2int([item_node.value for item_node in pred[:, 1]])
+        pred[:, 0] = pred_users_idx
+        pred[:, 1] = pred_items_idx
+        pred = pred.astype(np.float64)
+        pred = Prediction.from_uir(pred, user_map=test_set.user_map, item_map=test_set.item_map)
+
+        self._yaml_report = {'graph': repr(self.graph), 'mode': 'score_prediction', 'methodology': repr(methodology)}
+
+        return pred
+
+    def __repr__(self):
+        return f"GraphBasedRS(algorithm={self.algorithm}, graph={self.graph})"
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/score_processor.py` & `clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/score_processor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py` & `clayrs-0.5.1/clayrs/content_analyzer/ratings_manager/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/raw_information_source.py` & `clayrs-0.5.1/clayrs/content_analyzer/raw_information_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,27 @@
     Abstract Class that generalizes the acquisition of raw descriptions of the contents
     from one of the possible raw sources.
 
     Args:
         encoding: define the type of encoding of data stored in the source (example: "utf-8")
     """
 
-    def __init__(self, encoding: str):
+    def __init__(self, file_path: str, encoding: str):
+        self.__file_path = file_path
         self.__encoding = encoding
 
     @property
     def encoding(self):
         return self.__encoding
 
     @property
+    def file_path(self):
+        return self.__file_path
+
+    @property
     @abstractmethod
     def representative_name(self):
         raise NotImplementedError
 
     @abstractmethod
     def __iter__(self) -> Iterator[Dict[str, str]]:
         """
@@ -72,54 +77,53 @@
 
     Args:
         file_path: path of the dat file
         encoding: define the type of encoding of data stored in the source (example: "utf-8")
     """
 
     def __init__(self, file_path: str, encoding: str = "utf-8"):
-        super().__init__(encoding)
-        self.__file_path = file_path
+        super().__init__(file_path, encoding)
 
     @property
     def representative_name(self) -> str:
         """
         Method which returns a meaningful name for the raw source.
 
         In this case it's simply the file name + its extension
 
         Returns:
             The representative name for the raw source
         """
         # file name with extension
-        file_name = os.path.basename(self.__file_path)
+        file_name = os.path.basename(self.file_path)
 
         return file_name
 
     def __iter__(self) -> Iterator[Dict[str, str]]:
-        with open(self.__file_path, encoding=self.encoding) as f:
+        with open(self.file_path, encoding=self.encoding) as f:
             for line in f:
                 line_dict = {}
                 fields = line.split('::')
                 for i, field in enumerate(fields):
                     field = field.strip("\n\t\r")
                     line_dict[str(i)] = field
 
                 yield line_dict
 
     def __len__(self):
-        with open(self.__file_path, newline='', encoding=self.encoding) as dat_file:
+        with open(self.file_path, newline='', encoding=self.encoding) as dat_file:
             total_length = sum(1 for _ in dat_file)
 
             return total_length
 
     def __str__(self):
         return "DATFile"
 
     def __repr__(self):
-        return f'DATFile(encoding={self.__encoding}, file_path={self.__file_path})'
+        return f'DATFile(encoding={self.__encoding}, file_path={self.file_path})'
 
 
 class JSONFile(RawInformationSource):
     """
     Wrapper for a JSON file. This class is able to read from a JSON file where each "row" is a dictionary-like object
     inside a list
 
@@ -140,47 +144,46 @@
 
     Args:
         file_path: path of the dat file
         encoding: define the type of encoding of data stored in the source (example: "utf-8")
     """
 
     def __init__(self, file_path: str, encoding: str = "utf-8"):
-        super().__init__(encoding)
-        self.__file_path = file_path
+        super().__init__(file_path, encoding)
 
     @property
     def representative_name(self) -> str:
         """
         Method which returns a meaningful name for the raw source.
 
         In this case it's simply the file name + its extension
 
         Returns:
             The representative name for the raw source
         """
         # file name with extension
-        file_name = os.path.basename(self.__file_path)
+        file_name = os.path.basename(self.file_path)
 
         return file_name
 
     def __iter__(self) -> Iterator[Dict[str, str]]:
-        with open(self.__file_path, encoding=self.encoding) as j:
+        with open(self.file_path, encoding=self.encoding) as j:
             all_lines = json.load(j, parse_int=str, parse_float=str)
             for line in all_lines:
                 yield line
 
     def __len__(self):
-        with open(self.__file_path, encoding=self.encoding) as j:
+        with open(self.file_path, encoding=self.encoding) as j:
             return len(json.load(j))
 
     def __str__(self):
         return "JSONFile"
 
     def __repr__(self):
-        return f'JSONFile(encoding={self.__encoding}, file_path={self.__file_path})'
+        return f'JSONFile(encoding={self.__encoding}, file_path={self.file_path})'
 
 
 class CSVFile(RawInformationSource):
     r"""
     Wrapper for a CSV file. This class is able to read from a CSV file where each entry is separated by the a certain
     separator (`,` by default). So by using this class you can also read TSV file for examples, by specifying
     `separator='\t'`.
@@ -223,58 +226,57 @@
         separator: Character which separates each entry. By default is a comma (`,`), but in case you need to read from
             a TSV file simply change this parameter to `\t`
         has_header: Boolean value which specifies if the file has an header or not. Default is True
         encoding: Define the type of encoding of data stored in the source (example: "utf-8")
     """
 
     def __init__(self, file_path: str, separator: str = ',', has_header: bool = True, encoding: str = "utf-8-sig"):
-        super().__init__(encoding)
-        self.__file_path = file_path
+        super().__init__(file_path, encoding)
         self.__has_header = has_header
         self.__separator = separator
 
     @property
     def representative_name(self) -> str:
         """
         Method which returns a meaningful name for the raw source.
 
         In this case it's simply the file name + its extension
 
         Returns:
             The representative name for the raw source
         """
         # file name with extension
-        file_name = os.path.basename(self.__file_path)
+        file_name = os.path.basename(self.file_path)
 
         return file_name
 
     def __iter__(self) -> Iterator[Dict[str, str]]:
-        with open(self.__file_path, newline='', encoding=self.encoding) as csv_file:
+        with open(self.file_path, newline='', encoding=self.encoding) as csv_file:
             if self.__has_header:
                 reader = csv.DictReader(csv_file, quoting=csv.QUOTE_MINIMAL, delimiter=self.__separator)
             else:
                 reader = csv.DictReader(csv_file, quoting=csv.QUOTE_MINIMAL, delimiter=self.__separator)
                 reader.fieldnames = [str(i) for i in range(len(reader.fieldnames))]
                 csv_file.seek(0)
 
             yield from reader
 
     def __len__(self):
-        with open(self.__file_path, newline='', encoding=self.encoding) as csv_file:
+        with open(self.file_path, newline='', encoding=self.encoding) as csv_file:
             total_length = sum(1 for _ in csv_file)
             if self.__has_header:
                 total_length -= 1
 
             return total_length
 
     def __str__(self):
         return "CSVFile"
 
     def __repr__(self):
-        return f'CSVFile(file_path={self.__file_path}, separator={self.__separator}, has_header={self.__has_header}, ' \
+        return f'CSVFile(file_path={self.file_path}, separator={self.__separator}, has_header={self.__has_header}, ' \
                f'encoding={self.encoding})'
 
 
 class SQLDatabase(RawInformationSource):
     """
     Wrapper for a SQL database.
 
@@ -310,15 +312,15 @@
 
     def __init__(self, host: str,
                  username: str,
                  password: str,
                  database_name: str,
                  table_name: str,
                  encoding: str = "utf-8"):
-        super().__init__(encoding)
+        super().__init__('', encoding)
         self.__host: str = host
         self.__username: str = username
         self.__password: str = password
         self.__database_name: str = database_name
         self.__table_name: str = table_name
 
         conn = mysql.connector.connect(host=self.__host,
```

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/utils/check_tokenization.py` & `clayrs-0.5.1/clayrs/content_analyzer/utils/check_tokenization.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/content_analyzer/utils/id_merger.py` & `clayrs-0.5.1/clayrs/content_analyzer/utils/id_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     there is content whose id is composed by values coming from more than one field.
 
     Args:
         id_values (List<str>): List containing one or more ids
 
     Returns:
         id_merged (str): String in which the values contained in the list given in input are
-        merged
+            merged
     """
     if type(id_values) == str or type(id_values) == int:
         return str(id_values)
     elif type(id_values) == list:
         id_merged = ""
         for i in range(len(id_values)):
             id_merged += str(id_values[i])
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/eval_model.py` & `clayrs-0.5.1/clayrs/evaluation/eval_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
-from typing import List, Union, Tuple, TYPE_CHECKING
+from typing import List, Union, Tuple, TYPE_CHECKING, Optional
 
+import numpy as np
 import pandas as pd
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.ratings_manager.ratings import Prediction, Rank, Ratings
     from clayrs.evaluation.metrics.metrics import Metric
 
 from clayrs.evaluation.eval_pipeline_modules.metric_evaluator import MetricEvaluator
@@ -102,15 +103,15 @@
         Append a metric to the metric list that will be used to evaluate recommendation lists
 
         Args:
             metric: Metric to append to the metric list
         """
         self._metric_list.append(metric)
 
-    def fit(self, user_id_list: list = None) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    def fit(self, user_id_list: Optional[List[str]] = None) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
         This method performs the actual evaluation of the recommendation frames passed as input in the constructor of
         the class
 
         In case you want to perform evaluation for selected users, specify their ids parameter of this method.
         Otherwise, all users in the recommendation frames will be considered in the evaluation process
 
@@ -124,31 +125,48 @@
             >>>         metric_list=[eva.Precision(), eva.Recall()]
             >>> )
             >>> em.fit(selected_users)
 
         The method returns two pandas DataFrame: one containing ***system results*** for every metric in the metric
         list, one containing ***users results*** for every metric eligible
 
+        Args:
+            user_id_list: list of string ids for the users to consider in the evaluation (note that only string ids are
+                accepted and not their mapped integers)
+
         Returns:
             The first DataFrame contains the **system result** for every metric inside the metric_list
 
             The second DataFrame contains every **user results** for every metric eligible inside the metric_list
         """
         logger.info('Performing evaluation on metrics chosen')
 
-        pred_list = self._pred_list
-        truth_list = self._truth_list
+        final_pred_list = []
+        final_truth_list = []
 
+        # if user id list is passed, convert it to int if necessary and append the new ratings filtered with
+        # only the users of interest
         if user_id_list is not None:
-            user_id_list_set = set([str(user_id) for user_id in user_id_list])
 
-            pred_list = [pred.filter_ratings(user_id_list_set) for pred in self._pred_list]
-            truth_list = [truth.filter_ratings(user_id_list_set) for truth in self._truth_list]
+            for pred, truth in zip(self._pred_list, self._truth_list):
+
+                split_users = user_id_list
+                split_truth_users = set(truth.user_map.convert_seq_str2int(split_users))
+                split_pred_users = set(pred.user_map.convert_seq_str2int(split_users))
+
+                final_pred_list.append(pred.filter_ratings(list(split_pred_users)))
+                final_truth_list.append(truth.filter_ratings(list(split_truth_users)))
+
+        # otherwise the original lists are kept
+        else:
+
+            final_pred_list = self._pred_list
+            final_truth_list = self._truth_list
 
-        sys_result, users_result = MetricEvaluator(pred_list, truth_list).eval_metrics(self.metric_list)
+        sys_result, users_result = MetricEvaluator(final_pred_list, final_truth_list).eval_metrics(self.metric_list)
 
         # we save the sys result for report yaml
         self._yaml_report_result = sys_result.to_dict(orient='index')
 
         return sys_result, users_result
 
     def __repr__(self):
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py` & `clayrs-0.5.1/clayrs/evaluation/eval_pipeline_modules/metric_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,33 +56,43 @@
         It returns two Pandas DataFrame, the first one containing system results on all metrics specified, the second
         one containing each users results for every metric eligible
 
         Args:
             metric_list (List[Metric]): List of metric on which recommendations need to be evaluated
 
         Returns:
-            Two pandas DataFrame, the first will contain the system result for every metric specified inside the metric
-            list, the second one will contain every user results for every metric eligible
+            The first DataFrame will contain the system result for every metric specified inside the metric list,
+
+            The second DataFrame will contain every user results for every metric eligible
         """
 
         frames_to_concat_users = []
         frames_to_concat_system = []
 
         with get_progbar(metric_list) as pbar:
 
             for metric in pbar:
                 pbar.set_description(desc=f"Performing {metric}")
 
                 metric_result_list = []
 
                 for pred, truth in zip(self._pred_list, self._truth_list):
                     if len(pred) != 0 and len(truth) != 0:
-                        user_id_valid = set(pred.user_id_column)
-                        # Remove from truth users of which we do not have predictions
-                        truth = truth.filter_ratings(user_id_valid)
+
+                        # users can be different between predictions and truth, we only consider those
+                        # who are in both
+                        common_user_ids = list(
+                            set(pred.unique_user_id_column).intersection(set(truth.unique_user_id_column))
+                        )
+
+                        prediction_user_idxs = pred.user_map.convert_seq_str2int(common_user_ids)
+                        truth_user_idxs = truth.user_map.convert_seq_str2int(common_user_ids)
+
+                        pred = pred.filter_ratings(prediction_user_idxs)
+                        truth = truth.filter_ratings(truth_user_idxs)
 
                         metric_result = metric.perform(Split(pred, truth))
 
                         metric_result_list.append(metric_result)
 
                 # if in future results for each fold for each user
                 # set index as from_id and concat axis = 1
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/metrics/classification_metrics.py` & `clayrs-0.5.1/clayrs/evaluation/metrics/classification_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 from abc import abstractmethod
-from typing import List, Set, Callable, TYPE_CHECKING
+from typing import Callable, TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-    from clayrs.recsys.partitioning import Split
+    from clayrs.evaluation.eval_pipeline_modules.metric_evaluator import Split
 
-from clayrs.evaluation.metrics.metrics import Metric
+from clayrs.evaluation.metrics.metrics import Metric, handler_different_users
 
 
 class ClassificationMetric(Metric):
     """
     Abstract class that generalize classification metrics.
     A classification metric uses confusion matrix terminology (true positive, false positive, etc.) to classify each
     item predicted
@@ -44,51 +43,61 @@
     def sys_avg(self):
         return self.__avg
 
     @property
     def precision(self):
         return self.__precision
 
+    @handler_different_users
     def perform(self, split: Split) -> pd.DataFrame:
         # This method will calculate for every split true positive, false positive, true negative, false negative items
         # so that every metric must simply implement the method _calc_metric(...).
         # Thanks to polymorphism, everything will work without changing this main method
 
         pred = split.pred
         truth = split.truth
 
         split_result = {'user_id': [], str(self): []}
         sys_confusion_matrix = np.array([[0, 0],
                                          [0, 0]], dtype=np.int32)
 
-        for user in set(truth.user_id_column):
-            user_predictions = pred.get_user_interactions(user)
-            user_truth = truth.get_user_interactions(user)
+        # users in truth and pred of the split to evaluate must be the same!
+        user_idx_truth = truth.unique_user_idx_column
+        user_idx_pred = pred.user_map.convert_seq_str2int(truth.unique_user_id_column)
+
+        for uidx_pred, uidx_truth in zip(user_idx_pred, user_idx_truth):
+            user_predictions_indices = pred.get_user_interactions(uidx_pred, as_indices=True)
+            user_truth_indices = truth.get_user_interactions(uidx_truth, as_indices=True)
+
+            user_truth_scores = truth.score_column[user_truth_indices]
+            user_truth_items = truth.item_id_column[user_truth_indices]
 
             relevant_threshold = self.relevant_threshold
             if relevant_threshold is None:
-                relevant_threshold = np.nanmean([truth_interaction.score
-                                                 for truth_interaction in user_truth])
+                relevant_threshold = np.nanmean(user_truth_scores)
 
-            user_truth_relevant_items = set([truth_interaction.item_id for truth_interaction in user_truth
-                                             if truth_interaction.score >= relevant_threshold])
+            user_predictions_items = pred.item_id_column[user_predictions_indices]
+            user_truth_relevant_items = user_truth_items[np.where(user_truth_scores >= relevant_threshold)]
 
             # If basically the user has not provided a rating to any items greater than the threshold,
             # then we don't consider it since it's not fault of the system
             if len(user_truth_relevant_items) != 0:
-                metric_user, user_confusion_matrix = self._perform_single_user(user_predictions,
+                metric_user, user_confusion_matrix = self._perform_single_user(user_predictions_items,
                                                                                user_truth_relevant_items)
 
                 sys_confusion_matrix += user_confusion_matrix
             else:
                 metric_user = np.nan
 
-            split_result['user_id'].append(user)
+            # temporarily append user_idx, later convert to user id
+            split_result['user_id'].append(uidx_truth)
             split_result[str(self)].append(metric_user)
 
+        split_result['user_id'] = list(truth.user_map.convert_seq_int2str(split_result['user_id']))
+
         # trick to check for nan values, if all values are nan then an exception is thrown
         if all(user_result != user_result for user_result in split_result[str(self)]):
             raise ValueError("No user has a rating above the given threshold! Try lower it")
 
         sys_metric = -1
         if self.sys_avg == 'micro':
             sys_metric = self._calc_metric(sys_confusion_matrix)
@@ -105,15 +114,15 @@
         """
         Private method that must be implemented by every metric which must specify how to use the confusion matrix
         terminology in order to compute the metric
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _perform_single_user(self, user_prediction_items: List[Interaction], user_truth_items: Set[str]):
+    def _perform_single_user(self, user_prediction_items: np.ndarray, user_truth_items: np.ndarray):
         raise NotImplementedError
 
 
 class Precision(ClassificationMetric):
     r"""
     The Precision metric is calculated as such for the **single user**:
 
@@ -156,18 +165,17 @@
                f"precision={self.precision})"
 
     def _calc_metric(self, confusion_matrix: np.ndarray):
         tp = confusion_matrix[0, 0]
         fp = confusion_matrix[0, 1]
         return self.precision((tp + fp) and tp / (tp + fp) or 0)  # safediv between tp and (tp + fp)
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        tp = len([prediction_interaction for prediction_interaction in user_prediction
-                  if prediction_interaction.item_id in user_truth_relevant_items])
-        fp = len(user_prediction) - tp
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        tp = len(np.intersect1d(user_predictions_items, user_truth_relevant_items))
+        fp = len(user_predictions_items) - tp
 
         # we do not compute the full confusion matrix for the user
         useful_confusion_matrix_user = np.array([[tp, fp],
                                                  [0, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -219,19 +227,18 @@
     def __str__(self):
         return "Precision@{} - {}".format(self.k, self.sys_avg)
 
     def __repr__(self):
         return f"PrecisionAtK(k={self.k}, relevant_threshold={self.relevant_threshold}, sys_average={self.sys_avg}, " \
                f"precision={self.precision})"
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        user_prediction_cut = user_prediction[:self.k]
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        user_prediction_cut = user_predictions_items[:self.k]
 
-        tp = len([prediction_interaction for prediction_interaction in user_prediction_cut
-                  if prediction_interaction.item_id in user_truth_relevant_items])
+        tp = len(np.intersect1d(user_prediction_cut, user_truth_relevant_items))
         fp = len(user_prediction_cut) - tp
 
         useful_confusion_matrix_user = np.array([[tp, fp],
                                                  [0, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -275,20 +282,19 @@
     def __str__(self):
         return "R-Precision - {}".format(self.sys_avg)
 
     def __repr__(self):
         return f"RPrecision(relevant_threshold={self.relevant_threshold}, sys_average={self.sys_avg}, " \
                f"precision={self.precision})"
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
         r = len(user_truth_relevant_items)
-        user_prediction_cut = user_prediction[:r]
+        user_prediction_cut = user_predictions_items[:r]
 
-        tp = len([prediction_interaction for prediction_interaction in user_prediction_cut
-                  if prediction_interaction.item_id in user_truth_relevant_items])
+        tp = len(np.intersect1d(user_prediction_cut, user_truth_relevant_items))
         fp = len(user_prediction_cut) - tp
 
         useful_confusion_matrix_user = np.array([[tp, fp],
                                                  [0, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -337,17 +343,16 @@
                f"precision={self.precision})"
 
     def _calc_metric(self, confusion_matrix: np.ndarray):
         tp = confusion_matrix[0, 0]
         fn = confusion_matrix[1, 0]
         return self.precision((tp + fn) and tp / (tp + fn) or 0)  # safediv between tp and (tp + fn)
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        tp = len([prediction_interaction for prediction_interaction in user_prediction
-                  if prediction_interaction.item_id in user_truth_relevant_items])
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        tp = len(np.intersect1d(user_predictions_items, user_truth_relevant_items))
         fn = len(user_truth_relevant_items) - tp
 
         useful_confusion_matrix_user = np.array([[tp, 0],
                                                  [fn, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -399,19 +404,18 @@
     def __str__(self):
         return "Recall@{} - {}".format(self.k, self.sys_avg)
 
     def __repr__(self):
         return f"RecallAtK(k={self.k}, relevant_threshold={self.relevant_threshold}, sys_average={self.sys_avg}, " \
                f"precision={self.precision})"
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        user_prediction_cut = user_prediction[:self.k]
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        user_prediction_cut = user_predictions_items[:self.k]
 
-        tp = len([prediction_interaction for prediction_interaction in user_prediction_cut
-                  if prediction_interaction.item_id in user_truth_relevant_items])
+        tp = len(np.intersect1d(user_prediction_cut, user_truth_relevant_items))
         fn = len(user_truth_relevant_items) - tp
 
         useful_confusion_matrix_user = np.array([[tp, 0],
                                                  [fn, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -485,18 +489,17 @@
         num = prec * reca
         den = (beta_2 * prec) + reca
 
         fbeta = self.precision((1 + beta_2) * (den and num / den or 0))  # safediv between num and den
 
         return fbeta
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        tp = len([prediction_interaction for prediction_interaction in user_prediction
-                  if prediction_interaction.item_id in user_truth_relevant_items])
-        fp = len(user_prediction) - tp
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        tp = len(np.intersect1d(user_predictions_items, user_truth_relevant_items))
+        fp = len(user_predictions_items) - tp
         fn = len(user_truth_relevant_items) - tp
 
         useful_confusion_matrix_user = np.array([[tp, fp],
                                                  [fn, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
 
@@ -559,19 +562,18 @@
     def __str__(self):
         return "F{}@{} - {}".format(self.beta, self.k, self.sys_avg)
 
     def __repr__(self):
         return f"FMeasureAtK(k={self.k}, beta={self.beta}, relevant_threshold={self.relevant_threshold}, " \
                f"sys_average={self.sys_avg}, precision={self.precision})"
 
-    def _perform_single_user(self, user_prediction: List[Interaction], user_truth_relevant_items: Set[str]):
-        user_prediction_cut = user_prediction[:self.k]
+    def _perform_single_user(self, user_predictions_items: np.ndarray, user_truth_relevant_items: np.ndarray):
+        user_prediction_cut = user_predictions_items[:self.k]
 
-        tp = len([prediction_interaction for prediction_interaction in user_prediction_cut
-                  if prediction_interaction.item_id in user_truth_relevant_items])
+        tp = len(np.intersect1d(user_prediction_cut, user_truth_relevant_items))
         fp = len(user_prediction_cut) - tp
         fn = len(user_truth_relevant_items) - tp
 
         useful_confusion_matrix_user = np.array([[tp, fp],
                                                  [fn, 0]], dtype=np.int32)
 
         return self._calc_metric(useful_confusion_matrix_user), useful_confusion_matrix_user
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/metrics/error_metrics.py` & `clayrs-0.5.1/clayrs/evaluation/metrics/error_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,89 @@
 from __future__ import annotations
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 import pandas as pd
 import numpy as np
+import numpy_indexed as npi
 from sklearn.metrics import mean_absolute_error, mean_squared_error
 
 if TYPE_CHECKING:
     from clayrs.recsys.partitioning import Split
 
-from clayrs.evaluation.metrics.metrics import Metric
+from clayrs.evaluation.metrics.metrics import Metric, handler_different_users
 
 
 class ErrorMetric(Metric):
     """
     Abstract class for error metrics.
     An Error Metric evaluates 'how wrong' the recommender system was in predicting a rating
     """
 
+    @handler_different_users
     def perform(self, split: Split) -> pd.DataFrame:
         pred = split.pred
         truth = split.truth
 
         split_result = {'user_id': [], str(self): []}
 
-        for user in set(truth.user_id_column):
-            user_predictions = pred.get_user_interactions(user)
-            user_truth = truth.get_user_interactions(user)
-
-            # this will contain as key item id and as value the score in the truth of the user
-            items_scores_truth = {truth_interaction.item_id: truth_interaction.score for truth_interaction in user_truth}
-
-            # [(pred_score, truth_score), (pred_score, truth_score), ...]
-            zipped_score_list = [(pred_interaction.score, items_scores_truth.get(pred_interaction.item_id))
-                                 for pred_interaction in user_predictions
-                                 if items_scores_truth.get(pred_interaction.item_id) is not None]
-
-            if len(zipped_score_list) != 0:
-                pred_score_list = [zipped_tuple[0] for zipped_tuple in zipped_score_list]
-                truth_score_list = [zipped_tuple[1] for zipped_tuple in zipped_score_list]
-                result = self._calc_metric(pred_score_list, truth_score_list)
+        # users in truth and pred of the split to evaluate must be the same!
+        user_idx_truth = truth.unique_user_idx_column
+        user_idx_pred = pred.user_map.convert_seq_str2int(truth.unique_user_id_column)
+
+        for uidx_pred, uidx_truth in zip(user_idx_pred, user_idx_truth):
+            user_predictions_idxs = pred.get_user_interactions(uidx_pred, as_indices=True)
+            user_truth_idxs = truth.get_user_interactions(uidx_truth, as_indices=True)
+
+            user_truth_items = truth.item_id_column[user_truth_idxs]
+
+            user_prediction_items = pred.item_id_column[user_predictions_idxs]
+            user_prediction_scores = pred.score_column[user_predictions_idxs]
+
+            idx_truth_in_pred = npi.indices(user_prediction_items, user_truth_items, missing=-1)
+            idx_truth_not_in_pred = np.where(idx_truth_in_pred == -1)
+
+            user_pred_common_idxs = np.delete(idx_truth_in_pred, idx_truth_not_in_pred)
+            user_truth_common_idxs = np.delete(user_truth_idxs, idx_truth_not_in_pred)
+
+            common_truth_scores = truth.score_column[user_truth_common_idxs]
+            common_prediction_scores = user_prediction_scores[user_pred_common_idxs]
+
+            if len(common_prediction_scores) != 0:
+                result = self._calc_metric(common_truth_scores, common_prediction_scores)
             else:
                 result = np.nan
 
-            split_result['user_id'].append(user)
+            split_result['user_id'].append(uidx_truth)
             split_result[str(self)].append(result)
 
+        split_result['user_id'] = list(truth.user_map.convert_seq_int2str(split_result['user_id']))
+
         split_result['user_id'].append('sys')
         split_result[str(self)].append(np.nanmean(split_result[str(self)]))
 
         return pd.DataFrame(split_result)
 
     @abstractmethod
     def _calc_metric(self, truth_scores: list, pred_scores: list):
         """
         Private method that must be implemented by every error metric specifying how to calculate the metric
-        for a single user given a Series of ratings taken from the ground truth and a Series of ratings predicted by the
+        for a single user given a list of ratings taken from the ground truth and a list of ratings predicted by the
         recommender system.
 
-        Both Series must be in relation 1 to 1 between each other, meaning that if row 1 of the 'truth_scores' parameter
+        Both lists must be in relation 1 to 1 between each other, meaning that if row 1 of the 'truth_scores' parameter
         contains the rating of the 'iPhone' item, row 1 of the 'pred_scores' parameter must contain the predicted rating
-        of the 'iPhone' item, so both Series must be ordered in the same manner and must be filtered in order to exclude
+        of the 'iPhone' item, so both lists must be ordered in the same manner and must be filtered in order to exclude
         items which are in the ground truth of the user but are not predicted, as well as items which are predicted
         but aren't present in the ground truth. Debug the unittest cases for examples
 
         Args:
-            truth_scores (pd.Series): Pandas Series which contains rating of the user taken from its ground truth. Has a
+            truth_scores: list which contains rating of the user taken from its ground truth. Has a
                 1 to 1 relationship with the 'pred_scores' Series
-            pred_scores (pd.Series): Pandas Series which contains rating predicted by the recommender system. Has a
+            pred_scores: list which contains rating predicted by the recommender system. Has a
                 1 to 1 relationship with the 'truth_scores' Series
         """
         raise NotImplementedError
 
 
 class MSE(ErrorMetric):
     r"""
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/metrics/fairness_metrics.py` & `clayrs-0.5.1/clayrs/evaluation/metrics/fairness_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,24 +67,28 @@
             pop_by_items: popularity for each label ('label', 'popularity')
             group: (optional) the set of users (user_id)
 
         Returns:
             Python dictionary containing as keys each user id and as values the average popularity of each user
         """
         if group is None:
-            group = set(data.user_id_column)
+            group = data.unique_user_id_column
+            group_int = data.unique_user_idx_column
+        else:
+            group_int = data.user_map.convert_seq_str2int(list(group))
+
+        avg_pop_by_users = []
+
+        for user_idx in group_int:
+            user_interactions_rows = data.get_user_interactions(user_idx, as_indices=True)
+            user_items = data.item_id_column[user_interactions_rows]
+
+            avg_pop_by_users.append(get_avg_pop(user_items, pop_by_items))
 
-        list_by_user = {
-            user: [interaction.item_id for interaction in data.get_user_interactions(user)]
-            for user in group
-        }
-        avg_pop_by_users = {
-            user: get_avg_pop(list_by_user[user], pop_by_items)
-            for user in group
-        }
+        avg_pop_by_users = dict(zip(group, avg_pop_by_users))
 
         return avg_pop_by_users
 
     @staticmethod
     def split_user_in_groups(score_frame: Ratings, groups: Dict[str, float],
                              pop_items: Set[str]) -> Dict[str, Set[str]]:
         r"""
@@ -119,15 +123,15 @@
                 the rest of the users are considered in a 'default_diverse' group
             pop_items: set of most popular *item_id* labels
 
         Returns:
             A python dictionary containing as keys each group name and as values the set of *user_id* belonging to
                 the particular group.
         """
-        num_of_users = len(set(score_frame.user_id_column))
+        num_of_users = len(score_frame.unique_user_id_column)
         if num_of_users < len(groups):
             raise NotEnoughUsers("You can't split in {} groups {} users! "
                                  "Try reducing number of groups".format(len(groups), num_of_users))
 
         for percentage_chosen in groups.values():
             if not 0 < percentage_chosen <= 1:
                 raise ValueError('Incorrect percentage! Valid percentage range: 0 < percentage <= 1')
@@ -210,32 +214,43 @@
             # The above formula, with all weights equal to 1 simplifies to:
             return (n + 1 - 2 * np.sum(cumx) / cumx[-1]) / n
 
         predictions = split.pred
 
         score_dict = {'user_id': [], str(self): []}
 
+        prediction_items = predictions.item_id_column
         if self.__top_n is not None:
-            predictions = itertools.chain.from_iterable([predictions.get_user_interactions(user_id, self.__top_n)
-                                                         for user_id in set(predictions.user_id_column)])
 
-        coun = Counter([prediction.item_id for prediction in predictions])
+            prediction_items = []
+
+            for user_idx in predictions.unique_user_idx_column:
+                user_interactions_indices = predictions.get_user_interactions(user_idx,
+                                                                              head=self.__top_n,
+                                                                              as_indices=True)
+
+                user_items = predictions.item_id_column[user_interactions_indices]
+                prediction_items.append(user_items)
+
+            prediction_items = itertools.chain.from_iterable(prediction_items)
+
+        coun = Counter(prediction_items)
 
         result = gini(list(coun.values()))
 
         score_dict['user_id'].append('sys')
         score_dict[str(self)].append(result)
 
         return pd.DataFrame(score_dict)
 
 
 class PredictionCoverage(FairnessMetric):
     r"""
     The Prediction Coverage metric measures in percentage how many distinct items are being recommended in relation
-    to all available items. It's a system wide metric, so only its result it will be returned and not those of every
+    to all available items. It's a system wise metric, so only its result it will be returned and not those of every
     user.
     The metric is calculated as such:
 
     $$
     Prediction Coverage_{sys} = (\frac{|I_p|}{|I|})\cdot100
     $$
 
@@ -272,27 +287,25 @@
 
         Args:
             pred: Ratings object containing recommendation lists of all users
 
         Returns:
             Set of distinct items that have been recommended that also appear in the catalog
         """
-        catalog = self.catalog
-        pred_items = set(pred.item_id_column)
-        return pred_items.intersection(catalog)
+        pred_items = set(pred.unique_item_id_column)
+        return pred_items.intersection(self.catalog)
 
     def perform(self, split: Split) -> pd.DataFrame:
         prediction = {'user_id': [], str(self): []}
-        catalog = {str(item) for item in self.__catalog}  # cast to string in case user is not careful
 
         pred = split.pred
 
         covered_items = self._get_covered(pred)
 
-        percentage = (len(covered_items) / len(catalog)) * 100
+        percentage = (len(covered_items) / len(self.__catalog)) * 100
         coverage_percentage = np.round(percentage, 2)
 
         prediction['user_id'].append('sys')
         prediction[str(self)].append(coverage_percentage)
 
         return pd.DataFrame(prediction)
 
@@ -362,42 +375,44 @@
 
         return name
 
     def __repr__(self):
         return f'CatalogCoverage(catalog={self.catalog}, top_n={self.__top_n}, k={self.__k})'
 
     def _get_covered(self, pred: Ratings):
-        catalog = self.catalog
-
-        if self.__top_n is not None:
-            pred = list(itertools.chain.from_iterable([pred.get_user_interactions(user_id, self.__top_n)
-                                                       for user_id in set(pred.user_id_column)]))
 
         # IF k is passed, then we choose randomly k users and calc catalog coverage
         # based on their predictions. We check that k is < n_user since if it's the equal
         # or it's greater, then all predictions generated for all user must be used
-        if self.__k is not None and self.__k < len(pred):
-            user_list = list(set([interaction_pred.user_id for interaction_pred in pred]))
+        user_list = pred.unique_user_idx_column
+        if self.__k is not None and self.__k < len(pred.unique_user_id_column):
 
-            sampling = random.choices(user_list, k=self.__k)
-            predicted_items = set([interaction_pred.item_id
-                                   for interaction_pred in pred if interaction_pred.user_id in sampling])
-            covered_items = predicted_items.intersection(catalog)
-        else:
-            predicted_items = set([interaction_pred.item_id for interaction_pred in pred])
-            covered_items = predicted_items.intersection(catalog)
+            user_list = random.choices(user_list, k=self.__k)
+
+        prediction_items = []
+
+        for user_idx in user_list:
+            user_interactions_indices = pred.get_user_interactions(user_idx,
+                                                                   head=self.__top_n,
+                                                                   as_indices=True)
+
+            user_items = pred.item_id_column[user_interactions_indices]
+            prediction_items.append(user_items)
+
+        prediction_items = list(itertools.chain.from_iterable(prediction_items))
+        covered_items = set(prediction_items).intersection(self.catalog)
 
         return covered_items
 
 
 class DeltaGap(GroupFairnessMetric):
     r"""
     The Delta GAP (Group Average popularity) metric lets you compare the average popularity "requested" by one or
     multiple groups of users and the average popularity "obtained" with the recommendation given by the recsys.
-    It's a system wide metric and results of every group will be returned.
+    It's a system wise metric and results of every group will be returned.
 
     It is calculated as such:
 
     $$
     \Delta GAP = \frac{recs_GAP - profile_GAP}{profile_GAP}
     $$
 
@@ -536,15 +551,15 @@
 
         split_result = defaultdict(list)
         split_result['user_id'] = ['sys']
 
         for group_name in splitted_user_groups:
 
             # we don't consider users of the group for which we do not have any recommendation
-            valid_group = splitted_user_groups[group_name].intersection(predictions.user_id_column)
+            valid_group = splitted_user_groups[group_name].intersection(set(predictions.unique_user_id_column))
 
             if len(valid_group) == 0:
                 logger.warning(f"Group {group_name} won't be considered in the DeltaGap since no recs is available "
                                f"for any user of said group!")
                 continue
 
             # Computing avg pop by users recs for delta gap
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/metrics/plot_metrics.py` & `clayrs-0.5.1/clayrs/evaluation/metrics/plot_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
             valid_group = splitted_user_groups[group_name].intersection(predictions.user_id_column)
 
             if len(valid_group) == 0:
                 logger.warning(f"Group {group_name} won't be considered in the DeltaGap since no recs is available "
                                f"for any user of said group!")
                 continue
 
+            valid_group = predictions.user_map.convert_seq_str2int(list(valid_group))
             profile_group_ratings = split_user_profile.filter_ratings(user_list=valid_group)
             pred_group_recommendations = predictions.filter_ratings(user_list=valid_group)
 
             profile_pop_ratios = pop_ratio_by_user(profile_group_ratings, most_pop_items)
             recs_pop_ratios = pop_ratio_by_user(pred_group_recommendations, most_pop_items)
 
             profile_pop_ratios = list(profile_pop_ratios.values())
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/statistical_test.py` & `clayrs-0.5.1/clayrs/evaluation/statistical_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import List
 
 import pandas as pd
+import numpy as np
 from scipy.stats import ttest_ind, ranksums
 
 
 class StatisticalTest(ABC):
     """
     Abstract class for Statistical Test.
 
     Every statistical test have to identify common users if the user
     chooses to pass us a df. The method stat_test_results is implemented
     differently for each statistical test you decide to do.
     """
+
+    def __init__(self, *user_id_column):
+        self.user_id_column = list(user_id_column) if user_id_column else None
+
     @staticmethod
-    def _common_users(df1, df2, column_list) -> pd.DataFrame:
+    def _common_users(df1, user_id_df1, df2, user_id_df2, column_list) -> pd.DataFrame:
         """
         Method called by the statistical test in case of use of df.
         Common users are searched for meaningful comparison.
         """
-        # we need to also extract the user_id column, that's why we append 'user_id'
-        column_list.append('user_id')
 
-        df1 = df1[column_list]
-        df2 = df2[column_list]
+        column_list_df1 = set(column_list)
+        column_list_df1.add(user_id_df1)
+        column_list_df2 = set(column_list)
+        column_list_df2.add(user_id_df2)
+
+        df1 = df1[column_list_df1]
+        df2 = df2[column_list_df2]
 
-        common_rows = pd.merge(df1, df2, how="inner", on=['user_id'])
+        common_rows = pd.merge(df1, df2, how="inner", left_on=user_id_df1, right_on=user_id_df2)
 
         return common_rows
 
     @abstractmethod
     def perform(self, users_metric_results: list) -> pd.DataFrame:
         """
         Abstract method in which must be specified how to calculate Statistical test
@@ -65,46 +73,94 @@
         Args:
             df_list: List containing DataFrames with several metrics to compare, preferably metrics computed for each
                 user. One DataFrame corresponds to one learning schema
 
         Returns:
             A Pandas DataFrame where each combination of learning schemas are compared in pair. The first value of each
                 cell is the ***statistic***, the second is the ***p-value***
-
         """
 
-        # we consider the 'user_id' index as a column
-        df_list = [df.reset_index() if 'user_id' not in df.columns else df for df in df_list]
+        user_id_column = self.user_id_column
+        if user_id_column is None:
+            user_id_column = ["user_id" for _ in range(len(df_list))]
+        elif len(user_id_column) == 1:
+            user_id_column = [self.user_id_column[0] for _ in range(len(df_list))]
+        elif len(user_id_column) != len(df_list):
+            raise ValueError("You must either specify a single user_id column for all dataframes or a different "
+                             "user_id column for each DataFrame passed!")
+
+        # if the user id column is the index we consider it as an additional column
+        df_list_reset = []
+        for user_id_col, df in zip(user_id_column, df_list):
+            if user_id_col not in df.columns:
+                if user_id_col == df.index.name:
+                    df = df.reset_index()
+                else:
+                    raise KeyError(f"Column {user_id_col} not present neither in the columns nor as index!")
+
+            df_list_reset.append(df)
+
+        data = defaultdict(lambda: defaultdict(dict))
 
-        final_result = defaultdict(list)
+        # this will contain metrics that are in common at least by two system
+        global_metrics = set()
 
         n_system_evaluated = 1
-        while len(df_list) != 0:
-            df1 = df_list.pop(0)
-            for i, other_df in enumerate(df_list, start=n_system_evaluated + 1):
+        while len(df_list_reset) != 0:
+            df1 = df_list_reset.pop(0)
+            user_id_col1 = user_id_column.pop(0)
+            for i, (user_id_col2, other_df) in enumerate(zip(user_id_column, df_list_reset),
+                                                         start=n_system_evaluated + 1):
+
                 common_metrics = [column for column in df1.columns
-                                  if column != 'user_id' and column in other_df.columns]
+                                  if column != user_id_col1 and column in other_df.columns]
 
-                common_rows = self._common_users(df1, other_df, list(common_metrics))
+                common_rows = self._common_users(df1, user_id_col1, other_df, user_id_col2, common_metrics)
 
-                final_result["Systems evaluated"].append((f"system_{n_system_evaluated}", f"system_{i}"))
                 for metric in common_metrics:
 
+                    global_metrics.add(metric)
                     # drop nan values since otherwise test may behave unexpectedly
                     metric_rows = common_rows[[f"{metric}_x", f"{metric}_y"]].dropna()
 
                     score_system1 = metric_rows[f"{metric}_x"]
                     score_system2 = metric_rows[f"{metric}_y"]
 
-                    single_metric_result = self._perform_test(score_system1, score_system2)
-                    final_result[metric].append(single_metric_result)
+                    statistic, pvalue = self._perform_test(score_system1, score_system2)
+
+                    data[(f"system_{n_system_evaluated}", f"system_{i}")][str(metric)]["statistic"] = statistic
+                    data[(f"system_{n_system_evaluated}", f"system_{i}")][str(metric)]["pvalue"] = pvalue
 
             n_system_evaluated += 1
 
-        return pd.DataFrame(final_result).set_index("Systems evaluated")
+        # index will contain (sys1, sys2), (sys1, sys3), ... tuples
+        # formatted_data will be in the form
+        # {(NDCG, "statistic"): [..., ..., ..., ...], (NDCG, "pvalue"): [..., ..., ..., ...],
+        #  (Precision, "statistic"): [..., ..., ..., ...], (Precision, "pvalue"): [..., ..., ..., ...],
+        #  ...}
+        index = []
+        formatted_data = defaultdict(list)
+        for df_index_row, df_data_row in data.items():
+            index.append(df_index_row)
+
+            for metric_column in global_metrics:
+                stat, pval = np.nan, np.nan
+
+                stat_pval_dict = df_data_row.get(metric_column)
+                if stat_pval_dict is not None:
+                    stat = stat_pval_dict["statistic"]
+                    pval = stat_pval_dict["pvalue"]
+
+                formatted_data[(metric_column, "statistic")].append(stat)
+                formatted_data[(metric_column, "pvalue")].append(pval)
+
+        res = pd.DataFrame(formatted_data, index=index)
+        res.index.rename("sys_pair", inplace=True)
+
+        return res
 
     @abstractmethod
     def _perform_test(self, score_metric_system1: list, score_metric_system2: list):
         """
         Abstract method in which must be specified how to calculate the paired statistical test
         """
         raise NotImplementedError
```

### Comparing `clayrs-0.4.1/clayrs/evaluation/utils.py` & `clayrs-0.5.1/clayrs/evaluation/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Args:
         original_ratings: `Ratings` object used to compute popularity for each item
 
     Returns:
         Python dictionary containing popularity computed for each item in the `original_ratings` parameter
     """
-    n_users = len(set(original_ratings.user_id_column))
+    n_users = len(original_ratings.unique_user_id_column)
 
     pop_by_item = {item_id: count / n_users for item_id, count in Counter(original_ratings.item_id_column).items()}
 
     return pop_by_item
 
 
 def get_most_popular_items(pop_by_item: Dict, top_n_percentage: float = 0.2) -> Set[str]:
@@ -63,27 +63,29 @@
         score_frame: `Ratings` object used to compute popularity ratio for each user
         most_pop_items: set of most popular 'item_id' labels
 
     Returns:
         Python dictionary containing as keys each user id and as value the popularity ratio of each user
     """
     # Splitting users by popularity
-    users = set(score_frame.user_id_column)
+    users_idxs = score_frame.unique_user_idx_column
 
-    popularity_ratio_by_user = {}
+    popularity_ratios = []
 
-    for user in users:
+    for user_idx in users_idxs:
         # filters by the current user and returns all the items he has rated
-        user_ratings = score_frame.get_user_interactions(user)
-        rated_items = set([user_interaction.item_id for user_interaction in user_ratings])
+        user_ratings_idxs = score_frame.get_user_interactions(user_idx, as_indices=True)
+        rated_items = set(score_frame.item_id_column[user_ratings_idxs])
         # intersects rated_items with popular_items
         popular_rated_items = rated_items.intersection(most_pop_items)
         popularity_ratio = len(popular_rated_items) / len(rated_items)
 
-        popularity_ratio_by_user[user] = popularity_ratio
+        popularity_ratios.append(popularity_ratio)
+
+    popularity_ratio_by_user = dict(zip(score_frame.unique_user_id_column, popularity_ratios))
 
     return popularity_ratio_by_user
 
 
 def get_avg_pop(items: List, pop_by_item: Dict) -> float:
     """
     Get the average popularity of the given items list
```

### Comparing `clayrs-0.4.1/clayrs/recsys/__init__.py` & `clayrs-0.5.1/clayrs/recsys/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from . import content_based_algorithm
 from . import graph_based_algorithm
 from . import graphs
 
 from .content_based_algorithm import *
 from .graph_based_algorithm import *
 from .graphs import *
+from .visual_based_algorithm import *
 from .recsys import ContentBasedRS, GraphBasedRS
 from .partitioning import KFoldPartitioning, HoldOutPartitioning, BootstrapPartitioning
 from .methodology import TestRatingsMethodology, TestItemsMethodology, TrainingItemsMethodology, AllItemsMethodology
 from .experiment import ContentBasedExperiment, GraphBasedExperiment
```

### Comparing `clayrs-0.4.1/clayrs/recsys/algorithm.py` & `clayrs-0.5.1/clayrs/recsys/algorithm.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/centroid_vector/centroid_vector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,237 +1,253 @@
 from __future__ import annotations
 from collections import defaultdict
 from typing import List, Union, Optional, TYPE_CHECKING
 import numpy as np
+from scipy import sparse
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.content_representation.content import Content
     from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
         CombiningTechnique
     from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
     from clayrs.recsys.content_based_algorithm.centroid_vector.similarities import Similarity
+    from clayrs.content_analyzer import Ratings
 
 from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
     Centroid
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
+from clayrs.recsys.content_based_algorithm.content_based_algorithm import PerUserCBAlgorithm
 from clayrs.recsys.content_based_algorithm.exceptions import NoRatedItems, OnlyNegativeItems, \
     NotPredictionAlg, EmptyUserRatings
 
 
-class CentroidVector(ContentBasedAlgorithm):
+class CentroidVector(PerUserCBAlgorithm):
     """
     Class that implements a centroid-like recommender. It first gets the centroid of the items that the user liked.
     Then computes the similarity between the centroid and the item of which the ranking score must be predicted.
     It's a ranking algorithm, so it can't do score prediction
 
     *   It computes the centroid vector of the features of items *liked by the user*
     *   It computes the similarity between the centroid vector and the items of which the ranking score must be
     predicted
 
     The items liked by a user are those having a rating higher or equal than a specific **threshold**.
     If the threshold is not specified, the average score of all items liked by the user is used.
 
     Examples:
-        * Interested in only a field representation, CosineSimilarity as similarity,
-        $threshold = 3$ (Every item with rating $>= 3$ will be considered as positive)
+        * Interested in only a field representation, `CosineSimilarity` as similarity,
+        `threshold` $= 3$ (Every item with rating $>= 3$ will be considered as positive)
 
         >>> from clayrs import recsys as rs
         >>> alg = rs.CentroidVector({"Plot": 0}, rs.CosineSimilarity(), 3)
 
-        * Interested in multiple field representations of the items, CosineSimilarity as similarity,
-        $threshold = None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
+        * Interested in multiple field representations of the items, `CosineSimilarity` as similarity,
+        `threshold` $= None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
 
         >>> alg = rs.CentroidVector(
         >>>                      item_field={"Plot": [0, "tfidf"],
         >>>                                  "Genre": [0, 1],
         >>>                                  "Director": "doc2vec"},
         >>>                      similarity=rs.CosineSimilarity(),
         >>>                      threshold=None)
 
         !!! info
 
-            After instantiating the CentroidVector algorithm, pass it in the initialization of
+            After instantiating the `CentroidVector` algorithm, pass it in the initialization of
             a CBRS and the use its method to calculate ranking for single user or multiple users:
 
             Examples:
                  
                 >>> cbrs = rs.ContentBasedRS(algorithm=alg, ...)
                 >>> cbrs.fit_rank(...)
                 >>> # ...
 
     Args:
         item_field: dict where the key is the name of the field
             that contains the content to use, value is the representation(s) id(s) that will be
             used for the said item. The value of a field can be a string or a list,
             use a list if you want to use multiple representations for a particular field.
-        similarity: Kind of similarity to use
+        similarity: `Similarity` object which handles how similarities between unseen items and centroid vector of
+            positive items of the active user is computed
         threshold: Threshold for the ratings. If the rating is greater than the threshold, it will be considered
-            as positive. If the threshold is not specified, the average score of all items liked by the user is used.
-        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used but they are in a
-            matrix form instead of a single vector (e.g. when WordEmbedding representations must be used you have one
+            as positive. If the threshold is not specified, the average score of all items rated by the user is used.
+        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used, but they are in a
+            matrix form instead of a single vector (e.g. WordEmbedding representations have one
             vector for each word). By default, the `Centroid` of the rows of the matrix is computed
     """
     __slots__ = ('_similarity', '_emb_combiner', '_centroid', '_positive_rated_list')
 
     def __init__(self, item_field: dict, similarity: Similarity, threshold: float = None,
                  embedding_combiner: CombiningTechnique = Centroid()):
         super().__init__(item_field, threshold)
 
         self._similarity = similarity
         self._emb_combiner = embedding_combiner
         self._centroid: Optional[np.ndarray] = None
         self._positive_rated_list: Optional[List] = None
 
-    def process_rated(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict):
+    def process_rated(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict):
         """
-        Function that extracts features from positive rated items ONLY!
+        Function that extracts features from positive rated items ONLY of a user
         The extracted features will be used to fit the algorithm (build the centroid).
 
-        Features extracted will be stored in a private attributes of the class.
+        Features extracted will be stored in a private attribute of the class.
+
+        IF there are no rated items available locally or if there are only negative
+        items, an exception is thrown.
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user (the user for which we must fit the algorithm)
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
+
+        Raises:
+            EmptyUserRatings: Exception raised when the user does not appear in the train set
+            NoRatedItems: Exception raised when there isn't any item available locally
+                rated by the user
+            OnlyNegativeitems: Exception raised when there are only negative items available locally
+                for the user (Items that the user disliked)
         """
         # a list since there could be duplicate interaction (eg bootstrap partitioning)
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        rated_items_id = train_ratings.item_map.convert_seq_int2str(uir_user[:, 1].astype(int))
+
+        # a list since there could be duplicate interaction (eg bootstrap partitioning)
         items_scores_dict = defaultdict(list)
-        for interaction in user_ratings:
-            items_scores_dict[interaction.item_id].append(interaction.score)
+
+        for item_id, score in zip(rated_items_id, uir_user[:, 2]):
+            items_scores_dict[item_id].append(score)
 
         items_scores_dict = dict(sorted(items_scores_dict.items()))  # sort dictionary based on key for reproducibility
 
-        # Load rated items from the path
+        # Create list of all the available items that are useful for the user
         loaded_rated_items: List[Union[Content, None]] = available_loaded_items.get_list([item_id
-                                                                                          for item_id in
-                                                                                          items_scores_dict.keys()])
+                                                                                          for item_id
+                                                                                          in rated_items_id])
 
         # If threshold wasn't passed in the constructor, then we take the mean rating
         # given by the user as its threshold
         threshold = self.threshold
         if threshold is None:
-            threshold = self._calc_mean_user_threshold(user_ratings)
+            threshold = np.nanmean(uir_user[:, 2])
 
         # we extract feature of each POSITIVE item sorted based on its key: IMPORTANT for reproducibility!!
         # otherwise the matrix we feed to sklearn will have input item in different rows each run!
         positive_rated_list = []
         for item in loaded_rated_items:
             if item is not None:
 
-                score_assigned = map(float, items_scores_dict[item.content_id])
+                score_assigned = items_scores_dict[item.content_id]
 
                 for score in score_assigned:
                     if score >= threshold:
                         positive_rated_list.append(self.extract_features_item(item))
 
-        if len(user_ratings) == 0:
+        if len(uir_user) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_id = user_ratings[0].user_id
         if len(loaded_rated_items) == 0 or (loaded_rated_items.count(None) == len(loaded_rated_items)):
-            raise NoRatedItems("User {} - No rated items available locally!".format(user_id))
+            raise NoRatedItems("User {} - No rated items available locally!".format(user_idx))
         if len(positive_rated_list) == 0:
             raise OnlyNegativeItems("User {} - There are only negative items available locally!")
 
         self._positive_rated_list = positive_rated_list
 
-    def fit(self):
+    def fit_single_user(self):
         """
-        The fit process for the CentroidVector consists in calculating the centroid of the features
-        of the positive items ONLY.
+        The fit process for the CentroidVector consists in computing the centroid for the active user of the features
+        of its positive items ONLY.
 
         This method uses extracted features of the positive items stored in a private attribute, so
         `process_rated()` must be called before this method.
 
         The built centroid will also be stored in a private attribute.
         """
-        positive_rated_features_fused = self.fuse_representations(self._positive_rated_list, self._emb_combiner,
-                                                                  as_array=True)
-        self._centroid = positive_rated_features_fused.mean(axis=0)
+        positive_rated_features_fused = self.fuse_representations(self._positive_rated_list, self._emb_combiner)
+        # reshape make the centroid bidimensional of shape (1, h) needed to compute faster similarities
+
+        self._centroid = positive_rated_features_fused.mean(axis=0).reshape(1, -1)
+
+        # we maintain original representation
+        if isinstance(positive_rated_features_fused, sparse.csr_matrix):
+            self._centroid = sparse.csr_matrix(self._centroid)
 
         # we delete variable used to fit since will no longer be used
         self._positive_rated_list = None
 
-    def predict(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-                filter_list: List[str] = None) -> List[Interaction]:
+    def predict_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                            filter_list: List[str]) -> np.ndarray:
         """
         CentroidVector is not a score prediction algorithm, calling this method will raise
         the `NotPredictionAlg` exception!
 
         Raises:
             NotPredictionAlg: exception raised since the CentroidVector algorithm is not a score prediction algorithm
         """
         raise NotPredictionAlg("CentroidVector is not a Score Prediction Algorithm!")
 
-    def rank(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-             recs_number: int = None, filter_list: List[str] = None) -> List[Interaction]:
+    def rank_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                         recs_number: Optional[int], filter_list: List[str]) -> np.ndarray:
         """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
+        Rank the top-n recommended items for the active user, where the top-n items to rank are controlled by the
+        `recs_number` and `filter_list` parameter:
+
+        * the former one is self-explanatory, the second is a list of items
+        represented with their string ids. Must be necessarily strings and not their mapped integer since items are
+        serialized following their string representation!
+
+        If `recs_number` is `None`, all ranked items will be returned
 
-        One can specify which items must be ranked with the `filter_list` parameter,
-        in this case ONLY items in the `filter_list` parameter will be ranked.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, **ALL** unrated items will be ranked.
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
-            filter_list (list): list of the items to rank, if None all unrated items for the user will be ranked
+            filter_list: list of the items to rank. Should contain string item ids
 
         Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
+            uir matrix for a single user containing user and item idxs (integer representation) with the ranked score
+                as third dimension sorted in a decreasing order
         """
-        try:
-            user_id = user_ratings[0].user_id
-        except IndexError:
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        if len(uir_user) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_seen_items = set([interaction.item_id for interaction in user_ratings])
-
         # Load items to predict
-        if filter_list is None:
-            items_to_predict = available_loaded_items.get_list([item_id for item_id in available_loaded_items
-                                                                if item_id not in user_seen_items])
-        else:
-            items_to_predict = available_loaded_items.get_list(filter_list)
+        items_to_predict = available_loaded_items.get_list(filter_list)
 
         # Extract features of the items to predict
-        id_items_to_predict = []
+        idx_items_to_predict = []
         features_items_to_predict = []
         for item in items_to_predict:
             if item is not None:
-                id_items_to_predict.append(item.content_id)
+                idx_items_to_predict.append(item.content_id)
                 features_items_to_predict.append(self.extract_features_item(item))
 
-        if len(id_items_to_predict) > 0:
-            # Calculate predictions, they are the similarity of the new items with the centroid vector
-            features_fused = self.fuse_representations(features_items_to_predict, self._emb_combiner, as_array=True)
-            similarities = [self._similarity.perform(self._centroid, item) for item in features_fused]
-        else:
-            similarities = []
-
-        # Build the item_score dict (key is item_id, value is rank score predicted)
-        # and order the keys in descending order
-        item_score_dict = dict(zip(id_items_to_predict, similarities))
-        ordered_item_ids = sorted(item_score_dict, key=item_score_dict.get, reverse=True)
-
-        # we only save the top-n items_ids corresponding to top-n recommendations
-        # (if recs_number is None ordered_item_ids will contain all item_ids as the original list)
-        ordered_item_ids = ordered_item_ids[:recs_number]
+        if len(idx_items_to_predict) == 0:
+            return np.array([])  # if no item to predict, empty rank is returned
+
+        idx_items_to_predict = train_ratings.item_map.convert_seq_str2int(idx_items_to_predict)
+
+        # Calculate predictions, they are the similarity of the new items with the centroid vector
+        features_fused = self.fuse_representations(features_items_to_predict, self._emb_combiner)
+        similarities = self._similarity.perform(self._centroid, features_fused).reshape(-1)  # 2d to 1d
+
+        sorted_scores_idxs = np.argsort(similarities)[::-1][:recs_number]
+        sorted_items = np.array(idx_items_to_predict)[sorted_scores_idxs]
+        sorted_scores = similarities[sorted_scores_idxs]
 
         # we construct the output data
-        rank_interaction_list = [Interaction(user_id, item_id, item_score_dict[item_id])
-                                 for item_id in ordered_item_ids]
+        uir_rank = np.array([[user_idx, item_idx, score]
+                             for item_idx, score in zip(sorted_items, sorted_scores)])
 
-        return rank_interaction_list
+        return uir_rank
 
     def __str__(self):
         return "CentroidVector"
 
     def __repr__(self):
         return f'CentroidVector(item_field={self.item_field}, ' \
                f'similarity={self._similarity}, ' \
                f'threshold={self.threshold}, ' \
-               f'embedding_combiner={self._emb_combiner})'
+               f'embedding_combiner={self._emb_combiner})'
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,257 +1,292 @@
 from __future__ import annotations
 from collections import defaultdict
-from typing import List, Union, Optional, TYPE_CHECKING
+from typing import List, Optional, Set, TYPE_CHECKING
+import re
+import numpy as np
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer import Content
-    from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
-        CombiningTechnique
-    from clayrs.recsys.content_based_algorithm.classifier.classifiers import Classifier
-    from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
-
-from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
-    Centroid
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
-from clayrs.recsys.content_based_algorithm.exceptions import NoRatedItems, OnlyPositiveItems, \
-    OnlyNegativeItems, NotPredictionAlg, EmptyUserRatings
+    from clayrs.content_analyzer.ratings_manager.ratings import Ratings
 
+from clayrs.recsys.content_based_algorithm.content_based_algorithm import PerUserCBAlgorithm
+from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsIndex
+from clayrs.recsys.content_based_algorithm.exceptions import NotPredictionAlg, OnlyNegativeItems, EmptyUserRatings
 
-class ClassifierRecommender(ContentBasedAlgorithm):
+
+class IndexQuery(PerUserCBAlgorithm):
     """
-    Class that implements recommendation through a specified `Classifier`.
-    It's a ranking algorithm so it can't do score prediction.
+    Class for the search engine recommender using an index.
+    It firsts builds a query using the representation(s) specified of the positive items, then uses the mentioned query
+    to do an actual search inside the index: every item will have a score of "closeness" in relation to the
+    query, we use this score to rank every item.
+
+    Just be sure to use textual representation(s) to build a significant query and to make a significant search!
 
     Examples:
-        * Interested in only a field representation, DecisionTree classifier from sklearn,
-        $threshold = 3$ (Every item with rating score $>= 3$ will be considered as *positive*)
+
+        * Interested in only a field representation, classic tfidf similarity,
+        `threshold` $= 3$ (Every item with rating $>= 3$ will be considered as positive)
 
         >>> from clayrs import recsys as rs
-        >>> alg = rs.ClassifierRecommender({"Plot": 0}, rs.SkDecisionTree(), 3)
+        >>> alg = rs.IndexQuery({"Plot": 0}, threshold=3)
 
-        * Interested in only a field representation, KNN classifier with custom parameters from sklearn,
-        $threshold = 3$ (Every item with rating score $>= 3$ will be considered as positive)
+        * Interested in multiple field representations of the items, BM25 similarity,
+        `threshold` $= None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
 
-        >>> alg = rs.ClassifierRecommender({"Plot": 0}, rs.SkKNN(n_neighbors=3), 0)
+        >>> alg = rs.IndexQuery(
+        >>>                     item_field={"Plot": [0, "original_text"],
+        >>>                                 "Genre": [0, 1],
+        >>>                                 "Director": "preprocessed_text"},
+        >>>                     classic_similarity=False,
+        >>>                     threshold=3)
 
-        * Interested in multiple field representations of the items, KNN classifier with custom parameters from
-        sklearn, $threshold = None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
-
-        >>> alg = ClassifierRecommender(
-        >>>                             item_field={"Plot": [0, "tfidf"],
-        >>>                                         "Genre": [0, 1],
-        >>>                                         "Director": "doc2vec"},
-        >>>                             classifier=rs.SkKNN(n_neighbors=3),
-        >>>                             threshold=None)
 
         !!! info
 
-            After instantiating the ClassifierRecommender algorithm, pass it in the initialization of
+            After instantiating the IndexQuery algorithm, pass it in the initialization of
             a CBRS and the use its method to calculate ranking for single user or multiple users:
 
             Examples:
 
                 >>> cbrs = rs.ContentBasedRS(algorithm=alg, ...)
                 >>> cbrs.fit_rank(...)
                 >>> # ...
 
-
     Args:
-        item_field (dict): dict where the key is the name of the field
+        item_field: dict where the key is the name of the field
             that contains the content to use, value is the representation(s) id(s) that will be
-            used for the said item. The value of a field can be a string or a list,
-            use a list if you want to use multiple representations for a particular field.
-        classifier (Classifier): classifier that will be used. Can be one object of the Classifier class.
+            used for the said item, just BE SURE to use textual representation(s). The value of a field can be a string
+            or a list, use a list if you want to use multiple representations for a particular field.
+        classic_similarity: True if you want to use the classic implementation of tfidf in Whoosh,
+            False if you want BM25F
         threshold: Threshold for the ratings. If the rating is greater than the threshold, it will be considered
-            as positive. If the threshold is not specified, the average score of all items liked by the user is used.
-        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used but they are in a
-            matrix form instead of a single vector (e.g. when WordEmbedding representations must be used you have one
-            vector for each word). By default the `Centroid` of the rows of the matrix is computed
+            as positive. If the threshold is not specified, the average score of all items rated by the user is used.
     """
-    __slots__ = ('_classifier', '_embedding_combiner', '_labels', '_items_features')
+    __slots__ = ('_string_query', '_scores', '_positive_user_docs', '_classic_similarity')
 
-    def __init__(self, item_field: dict, classifier: Classifier, threshold: float = None,
-                 embedding_combiner: CombiningTechnique = Centroid()):
+    def __init__(self, item_field: dict, classic_similarity: bool = True, threshold: float = None):
         super().__init__(item_field, threshold)
-        self._classifier = classifier
-        self._embedding_combiner = embedding_combiner
-        self._labels: Optional[list] = None
-        self._items_features: Optional[list] = None
+        self._string_query: Optional[str] = None
+        self._scores: Optional[list] = None
+        self._positive_user_docs: Optional[dict] = None
+        self._classic_similarity: bool = classic_similarity
 
-    def process_rated(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict):
+    def _get_representations(self, index_representations: dict):
         """
-        Function that extracts features from rated item and labels them.
-        The extracted features will be later used to fit the classifier.
+        Private method which extracts representation(s) chosen from all representations codified for the items
+        extracted from the index
+
+        Args:
+            index_representations: representations for an item extracted from the index
+        """
+
+        def find_valid(pattern: str):
+            field_index_retrieved = [field_index for field_index in index_representations
+                                     if re.match(pattern, field_index)]
+
+            if len(field_index_retrieved) == 0:
+                raise KeyError("Id {} not found for the field {}".format(id, k))
+            elif len(field_index_retrieved) > 1:
+                raise ValueError("This shouldn't happen! Duplicate fields?")
+            else:
+                valid = field_index_retrieved[0]
+
+            return valid
+
+        representations_valid = {}
+        for k in self.item_field:
+            for id in self.item_field[k]:
+                # every representation for an item is codified like this: plot#0#tfidf
+                if isinstance(id, str):
+                    pattern = "^{}#.+#{}$".format(k, id)
+                else:
+                    # the id passed it's a int
+                    pattern = "^{}#{}.*$".format(k, id)
+
+                valid_key = find_valid(pattern)
+                representations_valid[valid_key] = index_representations[valid_key]
 
-        Features and labels will be stored in private attributes of the class.
+        return representations_valid
 
-        IF there are no rated_items available locally or if there are only positive/negative
+    def _load_available_contents(self, index_path: str, items_to_load: set = None):
+        return LoadedContentsIndex(index_path)
+
+    def process_rated(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsIndex):
+        """
+        Function that extracts features from positive rated items ONLY of a user
+        The extracted features will be used to fit the algorithm (build the query).
+
+        Features extracted will be stored in private attributes of the class.
+
+        IF there are no rated items available locally or if there are only positive/negative
         items, an exception is thrown.
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user (the user for which we must fit the algorithm)
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
 
         Raises:
-            NoRatedItems: Exception raised when there isn't any item available locally
-                rated by the user
-            OnlyPositiveItems: Exception raised when there are only positive items available locally
-                for the user (Items that the user liked)
+            EmptyUserRatings: Exception raised when the user does not appear in the train set
             OnlyNegativeitems: Exception raised when there are only negative items available locally
                 for the user (Items that the user disliked)
         """
+
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        rated_items_id = train_ratings.item_map.convert_seq_int2str(uir_user[:, 1].astype(int))
+
         # a list since there could be duplicate interaction (eg bootstrap partitioning)
         items_scores_dict = defaultdict(list)
-        for interaction in user_ratings:
-            items_scores_dict[interaction.item_id].append(interaction.score)
 
-        items_scores_dict = dict(sorted(items_scores_dict.items()))  # sort dictionary based on key for reproducibility
+        for item_id, score in zip(rated_items_id, uir_user[:, 2]):
+            items_scores_dict[item_id].append(score)
 
-        # Load rated items from the path
-        loaded_rated_items: List[Union[Content, None]] = available_loaded_items.get_list([item_id
-                                                                                          for item_id
-                                                                                          in items_scores_dict.keys()])
+        items_scores_dict = dict(sorted(items_scores_dict.items()))  # sort dictionary based on key for reproducibility
 
         threshold = self.threshold
         if threshold is None:
-            threshold = self._calc_mean_user_threshold(user_ratings)
+            threshold = np.nanmean(uir_user[:, 2])
 
-        # Assign label and extract features from the rated items
-        labels = []
-        items_features = []
+        # Initializes positive_user_docs which is a list that has tuples with document_id as first element and
+        # a dictionary as second. The dictionary value has the name of the field as key
+        # and its contents as value. By doing so we obtain the data of the fields while
+        # also storing information regarding the field and the document where it was
+        scores = []
+        positive_user_docs = []
 
-        # we extract feature of each item sorted based on its key: IMPORTANT for reproducibility!!
-        # otherwise the matrix we feed to sklearn will have input item in different rows each run!
-        for item in loaded_rated_items:
-            if item is not None:
+        ix = available_loaded_items.get_contents_interface()
 
-                score_assigned = map(float, items_scores_dict[item.content_id])
+        # we extract feature of each item sorted based on its key: IMPORTANT for reproducibility!!
+        # we must convert keys (which are strings) to the respective int idx to build the uir
+        for (item_id, (item_idx, score_list)) in zip(rated_items_id, items_scores_dict.items()):
 
-                for score in score_assigned:
-                    items_features.append(self.extract_features_item(item))
+            score_assigned = map(float, score_list)
 
-                    if score >= threshold:
-                        labels.append(1)
-                    else:
-                        labels.append(0)
+            for score in score_assigned:
+                if score >= threshold:
+                    # {item_id: {"item": item_dictionary, "score": item_score}}
+                    item_query = ix.query(item_id, results_number=1, classic_similarity=self._classic_similarity)
+                    if len(item_query) != 0:
+                        item = item_query.pop(item_id).get('item')
+                        scores.append(score)
+                        positive_user_docs.append((item_idx, self._get_representations(item)))
 
-        if len(user_ratings) == 0:
+        if len(uir_user[:, 1]) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_id = user_ratings[0].user_id
-        if len(items_features) == 0:
-            raise NoRatedItems("User {} - No rated item available locally!".format(user_id))
-        if 0 not in labels:
-            raise OnlyPositiveItems("User {} - There are only positive items available locally!".format(user_id))
-        elif 1 not in labels:
-            raise OnlyNegativeItems("User {} - There are only negative items available locally!".format(user_id))
+        if len(positive_user_docs) == 0:
+            raise OnlyNegativeItems(f"User {user_idx} - There are no rated items available locally or there are only "
+                                    f"negative items available locally!")
 
-        self._labels = labels
-        self._items_features = items_features
+        self._positive_user_docs = positive_user_docs
+        self._scores = scores
 
-    def fit(self):
+    def fit_single_user(self):
         """
-        Fit the classifier specified in the constructor with the features and labels
-        extracted with the `process_rated()` method.
+        The fit process for the IndexQuery consists in building a query using the features of the positive items ONLY
+        (items that the user liked). The terms relative to these 'positive' items are boosted by the
+        rating he/she/it gave.
+
+        This method uses extracted features of the positive items stored in a private attribute, so
+        `process_rated()` must be called before this method.
+
+        The built query will also be stored in a private attribute.
+        """
+        # For each field of each document one string (containing the name of the field and the data in it)
+        # is created and added to the query.
+        # Also each part of the query that refers to a document
+        # is boosted by the score given by the user to said document
+        string_query = "("
+        for (doc_id, doc_data), score in zip(self._positive_user_docs, self._scores):
+            string_query += "("
+            for field_name in doc_data:
+                if field_name == 'content_id':
+                    continue
+                word_list = doc_data[field_name].split()
+                string_query += field_name + ":("
+                for term in word_list:
+                    string_query += term + " "
+                string_query += ") "
+            string_query += ")^" + str(score) + " "
+        string_query += ") "
+
+        self._string_query = string_query
 
-        It uses private attributes to fit the classifier, so `process_rated()` must be called
-        before this method.
+    def _build_mask_list(self, user_seen_items: Set[str], filter_list: List[str]):
         """
-        # Fuse the input if there are dicts, multiple representation, etc.
-        fused_features = self.fuse_representations(self._items_features, self._embedding_combiner)
+        Private function that calculate the mask query and the filter query for whoosh to use:
 
-        self._classifier.fit(fused_features, self._labels)
+        - The mask query is needed to ignore items already rated by the user
+        - The filter query is needed to predict only items present in the filter_list
 
-        # we delete variables used to fit since will no longer be used
-        self._items_features = None
-        self._labels = None
+        If in the filter list there are items already rated by the user, those are excluded in the
+        mask query so that the prediction for those items can be calculated
 
-    def predict(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-                filter_list: List[str] = None) -> List[Interaction]:
+        Args:
+            user_seen_items: set of items present in the user profile
+            filter_list: list of the items to predict, if None all unrated items will be predicted
+        """
+        masked_list = [item for item in user_seen_items if item not in filter_list]
+
+        return masked_list
+
+    def predict_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsIndex,
+                            filter_list: List[str]) -> np.ndarray:
         """
-        ClassifierRecommender is not a score prediction algorithm, calling this method will raise
-        the `NotPredictionAlg` exception!
+        IndexQuery is not a Prediction Score Algorithm, so if this method is called,
+        a NotPredictionAlg exception is raised
 
         Raises:
-            NotPredictionAlg: exception raised since the CentroidVector algorithm is not a score prediction algorithm
+            NotPredictionAlg: exception raised since the IndexQuery algorithm is not a score prediction algorithm
         """
-        raise NotPredictionAlg("ClassifierRecommender is not a Score Prediction Algorithm!")
+        raise NotPredictionAlg("IndexQuery is not a Score Prediction Algorithm!")
 
-    def rank(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-             recs_number: int = None, filter_list: List[str] = None) -> List[Interaction]:
+    def rank_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsIndex,
+                         recs_number: Optional[int], filter_list: List[str]) -> np.ndarray:
         """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
+        Rank the top-n recommended items for the active user, where the top-n items to rank are controlled by the
+        `recs_number` and `filter_list` parameter:
 
-        One can specify which items must be ranked with the `filter_list` parameter,
-        in this case ONLY items in the `filter_list` parameter will be ranked.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, **ALL** unrated items will be ranked.
+        * the former one is self-explanatory, the second is a list of items
+        represented with their string ids. Must be necessarily strings and not their mapped integer since items are
+        serialized following their string representation!
+
+        If `recs_number` is `None`, all ranked items will be returned
+
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
-            filter_list (list): list of the items to rank, if None all unrated items for the user will be ranked
+            filter_list: list of the items to rank. Should contain string item ids
 
         Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
+            uir matrix for a single user containing user and item idxs (integer representation) with the ranked score
+                as third dimension sorted in a decreasing order
         """
-        try:
-            user_id = user_ratings[0].user_id
-        except IndexError:
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        if len(uir_user) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_seen_items = set([interaction.item_id for interaction in user_ratings])
+        user_seen_items = train_ratings.item_map.convert_seq_int2str(uir_user[:, 1].astype(int))
+        mask_list = self._build_mask_list(user_seen_items, filter_list)
+
+        ix = available_loaded_items.get_contents_interface()
+        score_docs = ix.query(self._string_query, recs_number, mask_list, filter_list, self._classic_similarity)
 
-        # Load items to predict
-        if filter_list is None:
-            items_to_predict = available_loaded_items.get_list([item_id
-                                                                for item_id in available_loaded_items
-                                                                if item_id not in user_seen_items])
-        else:
-            items_to_predict = available_loaded_items.get_list(filter_list)
-
-        # Extract features of the items to predict
-        id_items_to_predict = []
-        features_items_to_predict = []
-        for item in items_to_predict:
-            if item is not None:
-                id_items_to_predict.append(item.content_id)
-                features_items_to_predict.append(self.extract_features_item(item))
-
-        if len(id_items_to_predict) > 0:
-            # Fuse the input if there are dicts, multiple representation, etc.
-            fused_features_items_to_pred = self.fuse_representations(features_items_to_predict, self._embedding_combiner)
-
-            class_prob = self._classifier.predict_proba(fused_features_items_to_pred)
-        else:
-            class_prob = []
-
-        # for each item we extract the probability that the item is liked (class 1)
-        score_labels = (prob[1] for prob in class_prob)
-
-        # Build the item_score dict (key is item_id, value is rank score predicted)
-        # and order the keys in descending order
-        item_score_dict = dict(zip(id_items_to_predict, score_labels))
-        ordered_item_ids = sorted(item_score_dict, key=item_score_dict.get, reverse=True)
-
-        # we only save the top-n items_ids corresponding to top-n recommendations
-        # (if recs_number is None ordered_item_ids will contain all item_ids as the original list)
-        ordered_item_ids = ordered_item_ids[:recs_number]
+        # we must convert keys (which are strings) to the respective int idx to build the uir
+        score_list_idxs = train_ratings.item_map.convert_seq_str2int(list(score_docs.keys()))
 
         # we construct the output data
-        rank_interaction_list = [Interaction(user_id, item_id, item_score_dict[item_id])
-                                 for item_id in ordered_item_ids]
+        uir_rank = np.array([[user_idx, item_idx, score_docs[item_id]['score']]
+                             for item_idx, item_id in zip(score_list_idxs, score_docs)])
 
-        return rank_interaction_list
+        return uir_rank
 
     def __str__(self):
-        return "ClassifierRecommender"
+        return "IndexQuery"
 
     def __repr__(self):
-        return f'ClassifierRecommender(item_field={self.item_field}, ' \
-               f'classifier={self._classifier}, ' \
-               f'threshold={self.threshold}, ' \
-               f'embedding_combiner={self._embedding_combiner})'
+        return f'IndexQuery(item_field={self.item_field}, classic_similarity={self._classic_similarity}, ' \
+               f'threshold={self.threshold})'
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/classifiers.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py` & `clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,298 +1,320 @@
 from __future__ import annotations
-import abc
-from copy import deepcopy
-from itertools import chain
-from typing import List, TYPE_CHECKING
-import pandas as pd
-
-from scipy import sparse
-from sklearn.exceptions import NotFittedError
-from sklearn.feature_extraction import DictVectorizer
-from sklearn.utils.validation import check_is_fitted
-import numpy as np
-
-if TYPE_CHECKING:
-    from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
-        CombiningTechnique
-    from clayrs.content_analyzer.ratings_manager.ratings import Interaction, Prediction, Rank
-    from clayrs.content_analyzer.content_representation.content import Content
-    from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsInterface
+from collections.abc import Iterable
+from typing import List, Set, Union, Dict, TYPE_CHECKING
 
+from clayrs.utils.const import logger
 
-from clayrs.recsys.algorithm import Algorithm
+if TYPE_CHECKING:
+    from clayrs.content_analyzer import Ratings, Content
+    from clayrs.recsys.graphs.graph import Node
 
 from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
+from clayrs.recsys.graphs.nx_implementation.nx_bipartite_graphs import NXBipartiteGraph
+from clayrs.recsys.graphs.graph import TripartiteDiGraph, ItemNode, UserNode
+from clayrs.recsys.graphs.graph import PropertyNode
+from clayrs.utils.context_managers import get_progbar
 
 
-class ContentBasedAlgorithm(Algorithm):
+# Multiple Inheritance so that we will use NXBipartite as its proper father class (we'll its __init__ method)
+# and TripartiteDiGraph as its interface
+class NXTripartiteGraph(NXBipartiteGraph, TripartiteDiGraph):
     """
-    Abstract class for the content-based algorithms
+    Class that implements a Tripartite graph through networkx library.
 
-    Every Content Based Algorithm base its prediction (let it be score prediction or ranking) on representations
-    serialized by the Content Analyzer. It can be used a single representation or multiple ones for a single field or
-    multiple ones
+    !!! info
+
+        A *Tripartite Graph* is a graph which supports *User* nodes, *Item* nodes and *Property* nodes, but the latter
+        can only be linked to *Item* nodes.
+        If you need maximum flexibility, consider using a Full Graph
+
+    It creates a graph from an initial Rating object.
+
+    Consider the following matrix representation of the Rating object
+    ```
+        +------+-----------+-------+
+        | User |   Item    | Score |
+        +------+-----------+-------+
+        | u1   | Tenet     |     4 |
+        | u2   | Inception |     5 |
+        | ...  | ...       |   ... |
+        +------+-----------+-------+
+    ```
+
+    The graph will be created with the following interactions:
+
+    ```
+                 4
+            u1 -----> Tenet
+                 5
+            u2 -----> Inception
+    ```
+
+    where `u1` and `u2` become *User nodes* and `Tenet` and `Inception` become *Item nodes*,
+    with the edge weighted depending on the score given
+
+    If the `link_label` parameter is specified, then each link between users and items will be labeled with the label
+    specified (e.g. `link_label='score'`):
+
+    ```
+            (4, 'score')
+        u1 -------------> Tenet
+            (5, 'score')
+        u2 -------------> Inception
+    ```
+
+    Then the framework tries to load 'Tenet' and 'Inception' from the `item_contents_dir` if it is specified and if
+    succeeds, adds in the graph their loaded properties as specified in the `item_exo_properties` parameter.
+
+    !!! info "Load exogenous properties"
+
+        In order to load properties in the graph, we must specify where items are serialized and ***which
+        properties to add***:
+
+        *   If *item_exo_properties* is specified as a **set**, then the graph will try to load **all properties**
+        from **said exogenous representation**
+
+        ```python
+        {'my_exo_id'}
+        ```
+
+        *   If *item_exo_properties* is specified as a **dict**, then the graph will try to load **said properties**
+        from **said exogenous representation**
+
+        ```python
+        {'my_exo_id': ['my_prop1', 'my_prop2']]}
+        ```
 
     Args:
-    item_field (dict): dict where the key is the name of the field
-        that contains the content to use, value is the representation(s) id(s) that will be
-        used for the said item. The value of a field can be a string or a list,
-        use a list if you want to use multiple representations for a particular field.
-    threshold (float): Threshold for the ratings. Some algorithms use this threshold in order to
-        separate positive items from the negative ones, others may use only ratings that are >= than this
-        threshold. See the documentation of the algorithm used for more
-    """
-    __slots__ = ('item_field', 'threshold', '_transformer')
+        source_frame: The initial Ratings object needed to create the graph
+        item_exo_properties: Set or Dict which contains representations to load from items. Use a `Set` if you want
+            to load all properties from specific representations, or use a `Dict` if you want to choose which properties
+            to load from specific representations
+        item_contents_dir: The path containing items serialized with the Content Analyzer
+        link_label: If specified, each link will be labeled with the given label. Default is None
 
-    def __init__(self, item_field: dict, threshold: float):
-        self.item_field: dict = self._bracket_representation(item_field)
-        self.threshold: float = threshold
-        self._transformer = DictVectorizer(sparse=False, sort=False)
+    """
 
-    @staticmethod
-    def _bracket_representation(item_field: dict):
-        """
-        Private method that brackets every representation in case the user passed a string
-        instead of a list.
+    def __init__(self, source_frame: Ratings = None,
+                 item_exo_properties: Union[Dict, set] = None,
+                 item_contents_dir: str = None,
+                 link_label: str = None):
 
-        EXAMPLE::
-            > item_field = {'Plot': 0, 'Genre': ['tfidf', 1]}
-            > print(_bracket_representation(item_field))
+        NXBipartiteGraph.__init__(self, source_frame, link_label)
 
-            > {'Plot': [0], 'Genre': ['tfidf', 1]}
+        if item_exo_properties and not item_contents_dir:
+            logger.warning("`item_exo_properties` parameter set but `item_contents_dir` is None! "
+                           "No property will be loaded")
+        elif not item_exo_properties and item_contents_dir:
+            logger.warning("`item_contents_dir` parameter set but `item_exo_properties` is None! "
+                           "No property will be loaded")
 
-        Args:
-            item_field (dict): dict that may contain values that need to be bracketed
+        if source_frame is not None and item_contents_dir is not None and item_exo_properties is not None:
+            self.add_node_with_prop([ItemNode(item_id) for item_id in source_frame.unique_item_id_column],
+                                    item_exo_properties,
+                                    item_contents_dir)
 
-        Returns:
-            The item_field passed with all values inside a list
+    @property
+    def property_nodes(self) -> Set[PropertyNode]:
         """
-        for field in item_field:
-            if not isinstance(item_field[field], list):
-                item_field[field] = [item_field[field]]
-
-        return item_field
-
-    @staticmethod
-    def _calc_mean_user_threshold(user_ratings: List[Interaction]):
-        """
-        Private method which simply calculates the average rating by the user given its ratings
+        Returns a set of all *Property nodes* in the graph
         """
-        return np.nanmean([interaction.score for interaction in user_ratings])
+        return set(node for node in self._graph.nodes if isinstance(node, PropertyNode))
 
-    def extract_features_item(self, item: Content):
+    def add_node(self, node: Union[Node, List[Node]]):
         """
-        Function that extracts the feature of a loaded item using the item_field parameter passed in the
-        constructor.
+        Adds one or multiple Node objects to the graph.
+        Since this is a Tripartite Graph, only `User Node`, `Item Node` and `Property Node` can be added!
 
-        It extracts only the chosen representations of the chosen fields in the item loaded
-        EXAMPLE:
-
-            with item_field = {'Plot': [0], 'Genre': ['tfidf', 1]}, the function will extracts
-            only the representation with '0' as internal id for the field 'Plot' and two representations
-            for the field 'Genre': one with 'tfidf' as external id and the other with 1 as internal id
+        No duplicates are allowed, but different category nodes with same id are (e.g. `ItemNode('1')` and
+        `UserNode('1')`)
 
         Args:
-            item (Content): item loaded of which we need to extract its feature
+            node: Node(s) object(s) that needs to be added to the graph
 
-        Returns:
-            A list containing all representations extracted for the item
+        Raises:
+            ValueError: Exception raised when one of the node to add to the graph is not a User, Item or Property node
         """
-        item_bag_list = []
-        if item is not None:
-            for field in self.item_field:
-                field_representations = self.item_field[field]
-
-                for representation in field_representations:
-                    item_bag_list.append(
-                        item.get_field_representation(field, representation).value
-                    )
+        if not isinstance(node, list):
+            node = [node]
 
-        return item_bag_list
+        if any(not isinstance(n, (UserNode, ItemNode, PropertyNode)) for n in node):
+            raise ValueError("You can only add UserNodes or ItemNodes to a bipartite graph!")
 
-    def fuse_representations(self, X: list, embedding_combiner: CombiningTechnique, as_array: bool = False):
-        """
-        Method which transforms the X passed vectorizing if X contains dicts and merging
-        multiple representations in a single one for every item in X.
-        So if X = [
-                    [dict, np.array, np.array]
-                        ...
-                    [dict, np.array, np.array]
-                ]
-        where every sublist contains multiple representation for a single item,
-        the function returns:
-        X = [
-                np.array,
-                ...
-                np.array
-            ]
-        Where every row is the fused representation for the item
-
-        In case np.array have different row size, every array will be transformed in a one dimensional one
-        using the parameter embedding combiner. Check all the available combining technique to know how rows of
-        a np.array can be merged into one
+        self._graph.add_nodes_from(node)
 
-        Args:
-            X (list): list that contains representations of the items
-            embedding_combiner (CombiningTechnique): combining technique in case there are multiple
-                vectors with different row size
-        Returns:
-            X fused and vectorized
+    def add_node_with_prop(self, node: Union[ItemNode, List[ItemNode]], item_exo_properties: Union[Dict, set],
+                           item_contents_dir: str,
+                           item_filename: Union[str, List[str]] = None):
         """
-        if any(not isinstance(rep, (dict, np.ndarray, (int, float), sparse.csc_matrix)) for rep in X[0]):
-            raise ValueError("You can only use representations of type: {numeric, embedding, tfidf}")
+        Adds one or multiple Node objects and its/their properties to the graph.
+        Since this is a Tripartite Graph, only `Item Node` are allowed to have properties!
 
-        # We check if there are dicts as representation in the first element of X,
-        # since the representations are the same for all elements in X we can check
-        # for dicts only in one element
-        need_vectorizer = any(isinstance(rep, dict) for rep in X[0])
-
-        if need_vectorizer:
-            # IF the transformer is not fitted then we are training the model
-            try:
-                check_is_fitted(self._transformer)
-            except NotFittedError:
-                X_dicts = [rep for item in X for rep in item if isinstance(rep, dict)]
-                self._transformer.fit(X_dicts)
-
-        # In every case, we transform the input
-        def single_item_fused_gen():
-            for item_repr_list in X:
-                single_arr = []
-                for item_repr in item_repr_list:
-                    if need_vectorizer and isinstance(item_repr, dict):
-                        item_repr = self._transformer.transform(item_repr)
-                        single_arr.append(item_repr.flatten())
-                    elif isinstance(item_repr, np.ndarray):
-                        if item_repr.ndim > 1:
-                            item_repr = embedding_combiner.combine(item_repr)
-
-                        single_arr.append(item_repr.flatten())
-                    else:
-                        # it's a float
-                        single_arr.append(item_repr)
-
-                yield single_arr
-
-        # if a representation used is a sparse matrix, then we use scipy library to concatenate
-        # otherwise, if we have all dense arrays, we use numpy. To do this check we consider the representations
-        # of the first item
-        first_arr = next(single_item_fused_gen())
-        if any(isinstance(x, sparse.csc_matrix) for x in first_arr):
-            X_vectorized = (sparse.hstack(single_arr) for single_arr in single_item_fused_gen())
-
-            X_vectorized = sparse.vstack(X_vectorized, format='csr')
-
-            if as_array is True:
-                X_vectorized = X_vectorized.toarray()
-        else:
-            X_vectorized = [np.hstack(single_arr) for single_arr in single_item_fused_gen()]
+        In order to load properties in the graph, we must specify where items are serialized and ***which
+        properties to add***:
 
-            X_vectorized = np.array(X_vectorized)
+        *   If *item_exo_properties* is specified as a **set**, then the graph will try to load **all properties**
+        from **said exogenous representation**
 
-        return X_vectorized
+        ```python
+        {'my_exo_id'}
+        ```
 
-    @abc.abstractmethod
-    def process_rated(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict):
-        """
-        Abstract method that processes rated items for the user.
+        *   If *item_exo_properties* is specified as a **dict**, then the graph will try to load **said properties**
+        from **said exogenous representation**
 
-        Every content-based algorithm processes rated items differently, it may be needed to extract features
-        from the rated items and label them, extract features only from the positive ones, etc.
+        ```python
+        {'my_exo_id': ['my_prop1', 'my_prop2']]}
+        ```
 
-        The rated items processed must be stored into a private attribute of the algorithm, later used
-        by the fit() method.
+        In case you want your node to have a different id from serialized contents, via the `item_filename` parameter
+        you can specify what is the filename of the node that you are adding, e.g.
 
-        Args:
-            user_ratings (pd.DataFrame): DataFrame containing ratings of a single user
-            available_loaded_items (LoadedContentsDict): loaded contents interface point to the items directory
-        """
-        raise NotImplementedError
+        ```
+        item_to_add = ItemNode('different_id')
 
-    @abc.abstractmethod
-    def fit(self):
-        """
-        Abstract method that fits the content-based algorithm.
-
-        Every content based algorithm has a different fit process, it may be needed to fit a classifier,
-        to build the centroid of the positive items, to build a query for the index, etc.
-
-        It must be called after the the process_rated() method since it uses private attributes calculated
-        by said method to fit the algorithm.
-
-        The fitted object will also be stored in a private attribute.
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def predict(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-                filter_list: List[str] = None) -> Prediction:
-        """
-        |  Abstract method that predicts the rating which a user would give to items
-        |  If the algorithm is not a PredictionScore Algorithm, implement this method like this:
+        # item_filename is 'item_serialized_1.xz'
 
-        def predict():
-            raise NotPredictionAlg
+        graph.add_node_with_prop(item_to_add, ..., item_filename='item_serialized_1')
+        ```
 
-        One can specify which items must be predicted with the filter_list parameter,
-        in this case ONLY items in the filter_list will be predicted.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, ALL unrated items will be predicted.
+        In case you are adding a list of nodes, you can specify the filename for each node in the list.
 
         Args:
-            user_ratings (pd.DataFrame): DataFrame containing ratings of a single user
-            available_loaded_items (LoadedContentsDict): loaded contents interface point to the items directory
-            filter_list (list): list of the items to predict, if None all unrated items will be score predicted
-        Returns:
-            pd.DataFrame: DataFrame containing one column with the items name,
-                one column with the score predicted
-        """
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def rank(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsInterface,
-             recs_number: int = None, filter_list: List[str] = None) -> Rank:
-        """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
-
-        One can specify which items must be ranked with the `filter_list` parameter,
-        in this case ONLY items in the `filter_list` parameter will be ranked.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, **ALL** unrated items will be ranked.
+            node: Node(s) object(s) that needs to be added to the graph along with their properties
+            item_exo_properties: Set or Dict which contains representations to load from items. Use a `Set` if you want
+                to load all properties from specific representations, or use a `Dict` if you want to choose which
+                properties to load from specific representations
+            item_contents_dir: The path containing items serialized with the Content Analyzer
+            item_filename: Filename(s) of the node(s) to add
+
+        Raises:
+            ValueError: Exception raised when one of the node to add to the graph with their properties is not
+                an ItemNode
+        """
+        def node_prop_link_generator():
+            for n, id in zip(progbar, item_filename):
+                item: Content = loaded_items.get(id)
+
+                if item is not None:
+                    exo_props = self._get_exo_props(item_exo_properties, item)
+
+                    single_item_prop_edges = [(n,
+                                               PropertyNode(prop_dict[prop]),
+                                               {'label': prop})
+                                              for prop_dict in exo_props for prop in prop_dict]
+
+                else:
+                    single_item_prop_edges = []
+
+                yield from single_item_prop_edges
+
+        if not isinstance(node, list):
+            node = [node]
+
+        if any(not isinstance(n, ItemNode) for n in node):
+            raise ValueError("Only item nodes can be linked to property nodes in a Tripartite Graph!")
+
+        if isinstance(item_exo_properties, set):
+            item_exo_properties = dict.fromkeys(item_exo_properties, None)
+
+        if item_filename is None:
+            item_filename = [n.value for n in node]
+
+        if not isinstance(item_filename, list):
+            item_filename = [item_filename]
+
+        loaded_items = LoadedContentsDict(item_contents_dir, contents_to_load=set(item_filename))
+        with get_progbar(node) as progbar:
+
+            progbar.set_description("Creating Item->Properties links")
+            self._graph.add_edges_from((tuple_to_add for tuple_to_add in node_prop_link_generator()))
+
+    def _get_exo_props(self, desired_exo_dict: Dict, item: Content):
+        extracted_prop = []
+        for exo_id, prop_list_desired in desired_exo_dict.items():
+            all_exo_prop: dict = item.get_exogenous_representation(exo_id).value
+            # here we filter properties if user specified only certain properties to get
+            if prop_list_desired is not None:
+                filtered_keys = all_exo_prop.keys() & set(prop_list_desired)
+                all_exo_prop = {prop: all_exo_prop[prop] for prop in filtered_keys}
+
+            # we must split eventual properties that are lists
+            # eg. {film_director: ['tarantino uri', 'nolan uri']} ->
+            # [{film_director: 'tarantino uri'}, {film_director: 'nolan uri'}]
+            prop_list_val = {prop_label: all_exo_prop[prop_label] for prop_label in all_exo_prop
+                             if isinstance(all_exo_prop[prop_label], Iterable) and
+                             not isinstance(all_exo_prop[prop_label], str)}
+            if len(prop_list_val) != 0:
+                splitted_dict = [{prop_label: prop_val} for prop_label in prop_list_val
+                                 for prop_val in prop_list_val[prop_label]]
+
+                prop_single_val = {prop_label: all_exo_prop[prop_label]
+                                   for prop_label in all_exo_prop.keys() - prop_list_val.keys()}
+
+                extracted_prop.extend(splitted_dict)
+                if len(prop_single_val) != 0:
+                    extracted_prop.append(prop_single_val)
+            else:
+                extracted_prop.append(all_exo_prop)
+
+        return extracted_prop
+
+    def add_link(self, start_node: Union[Node, List[Node]], final_node: Union[Node, List[Node]],
+                 weight: float = None, label: str = None, timestamp: str = None):
+        """
+        Creates a link connecting the `start_node` to the `final_node`. If two lists are passed, then the node in
+        position $i$ in the `start_node` list will be linked to the node in position $i$ in the `final_node` list.
+
+        If nodes to link do not exist, they will be added automatically to the graph. Please remember that since this is
+        a Tripartite Graph, only *User nodes*, *Item nodes* and *Property nodes* can be added! And *Property nodes* can
+        only be linked to *Item nodes*!
+
+        A link can be weighted with the `weight` parameter and labeled with the `label` parameter.
+        A timestamp can also be specified via `timestamp` parameter.
+        All three are optional parameters, so they are not required
 
         Args:
-            user_ratings: List of Interaction objects for a single user
-            available_loaded_items: The LoadedContents interface which contains loaded contents
-            recs_number: number of the top ranked items to return, if None all ranked items will be returned
-            filter_list (list): list of the items to rank, if None all unrated items for the user will be ranked
-
-        Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-            a single user
-        """
-        raise NotImplementedError
-
-    def _load_available_contents(self, contents_path: str, items_to_load: set = None):
-        return LoadedContentsDict(contents_path, items_to_load, only_representations=self.item_field)
-
-    def __deepcopy__(self, memo):
-        # Create a new instance
-        cls = self.__class__
-        result = cls.__new__(cls)
-
-        # Don't copy self reference
-        memo[id(self)] = result
-
-        # Don't copy the cache - if it exists
-        if hasattr(self, "_cache"):
-            memo[id(self._cache)] = self._cache.__new__(dict)
+            start_node: Single Node object or a list of Node objects. They will be the 'head' of the link, since it's a
+                directed graph
+            final_node (object): Single Node object or a list Node objects. They will be the 'tail' of the link,
+                since it's a directed graph
+            weight: weight of the link, default is None (no weight)
+            label: label of the link, default is None (no label)
+            timestamp: timestamp of the link, default is None (no timestamp)
+
+        Raises:
+            ValueError: Exception raised when Property nodes are tried to be linked with non-Item nodes
+        """
+
+        def is_not_valid_link(start_n: Node, final_n: Node):
+            return (isinstance(final_n, PropertyNode) and not isinstance(start_n, ItemNode)) or \
+                   (isinstance(start_n, PropertyNode) and not isinstance(final_n, ItemNode))
+
+        if not isinstance(start_node, list):
+            start_node = [start_node]
+
+        if not isinstance(final_node, list):
+            final_node = [final_node]
+
+        if any(is_not_valid_link(start_n, final_n) for start_n, final_n in zip(start_node, final_node)):
+            raise ValueError("Only item nodes can be linked to property nodes in a Tripartite Graph!")
+
+        self.add_node(start_node)
+        self.add_node(final_node)
+
+        not_none_dict = {}
+        if label is not None:
+            not_none_dict['label'] = label
+        if weight is not None:
+            not_none_dict['weight'] = weight
+        if timestamp is not None:
+            not_none_dict['timestamp'] = timestamp
 
-        # Get all __slots__ of the derived class
-        slots = chain.from_iterable(getattr(s, '__slots__', []) for s in self.__class__.__mro__)
+        self._graph.add_edges_from(zip(start_node, final_node),
+                                   **not_none_dict)
 
-        # Deep copy all other attributes
-        for var in slots:
-            setattr(result, var, deepcopy(getattr(self, var), memo))
+    def __str__(self):
+        return "NXTripartiteGraph"
 
-        # Return updated instance
-        return result
+    def __repr__(self):
+        return str(self)
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/contents_loader.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/contents_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,26 +41,30 @@
             if not any(self._contents_dict.values()):
                 raise FileNotFoundError(f"No contents found in {contents_path}! "
                                         f"Maybe you have misspelled the path folder?")
 
     def get_contents_interface(self):
         return self._contents_dict
 
-    def get(self, key: str, only_representations: dict = None):
+    def get(self, key: str, only_representations: dict = None, throw_away: bool = False):
         content = self._contents_dict.get(key)
         if content is None:
             content = load_content_instance(self._contents_path, key, only_representations)
-            self._contents_dict[key] = content
+            if not throw_away:
+                self._contents_dict[key] = content
 
         return content
 
-    def get_list(self, key_list: Iterable[str], only_representations: dict = None):
+    def get_list(self, key_list: Iterable[str], only_representations: dict = None, throw_away: bool = False):
         contents_to_load = set(key_list) - set(self._contents_dict.keys())
-        self._contents_dict.update({content: load_content_instance(self._contents_path, content, only_representations)
-                                    for content in contents_to_load})
+        if not throw_away:
+            self._contents_dict.update({content: load_content_instance(self._contents_path,
+                                                                       content,
+                                                                       only_representations)
+                                        for content in contents_to_load})
 
         return [self._contents_dict[content_id] for content_id in key_list]
 
     def __getitem__(self, key: str):
         return self._contents_dict[key]
 
     def __iter__(self):
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/exceptions.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/exceptions.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/index_query/index_query.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,271 +1,273 @@
+from __future__ import annotations
 from collections import defaultdict
-from typing import List, Optional
-import re
+from typing import List, Union, Optional, TYPE_CHECKING
 
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
-from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsIndex
-from clayrs.recsys.content_based_algorithm.exceptions import NotPredictionAlg, OnlyNegativeItems, EmptyUserRatings
+import numpy as np
 
+if TYPE_CHECKING:
+    from clayrs.content_analyzer import Content
+    from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
+        CombiningTechnique
+    from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
+    from clayrs.recsys.content_based_algorithm.regressor.regressors import Regressor
+    from clayrs.content_analyzer.ratings_manager.ratings import Ratings
+
+from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
+    Centroid
+from clayrs.recsys.content_based_algorithm.exceptions import NoRatedItems, EmptyUserRatings
+from clayrs.recsys.content_based_algorithm.content_based_algorithm import PerUserCBAlgorithm
 
-class IndexQuery(ContentBasedAlgorithm):
-    """
-    Class for the search engine recommender using an index.
-    It firsts builds a query using the representation(s) specified of the positive items, then uses the mentioned query
-    to do an actual search inside the index: every items will have a score of "closeness" in relation to the
-    query, we use this score to rank every item.
 
-    Just be sure to use textual representation(s) to build a significant query and to make a significant search!
+class LinearPredictor(PerUserCBAlgorithm):
+    """
+    Class that implements recommendation through a specified linear predictor.
+    It's a score prediction algorithm, so it can predict what rating a user would give to an unseen item.
+    As such, it's also a ranking algorithm (it simply ranks in descending order unseen items by the predicted rating)
 
     Examples:
 
-        * Interested in only a field representation, classic tfidf similarity,
-        $threshold = 3$ (Every item with rating $>= 3$ will be considered as positive)
+        * Interested in only a field representation, `LinearRegression` regressor from sklearn
 
         >>> from clayrs import recsys as rs
-        >>> alg = rs.IndexQuery({"Plot": 0}, threshold=3)
+        >>> alg = rs.LinearPredictor({"Plot": 0}, rs.SkLinearRegression())
 
-        * Interested in multiple field representations of the items, BM25 similarity,
-        $threshold = None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
+        * Interested in only a field representation, `Ridge` regressor from sklearn with custom parameters
 
-        >>> alg = rs.IndexQuery(
-        >>>                     item_field={"Plot": [0, "original_text"],
-        >>>                                 "Genre": [0, 1],
-        >>>                                 "Director": "preprocessed_text"},
-        >>>                     classic_similarity=False,
-        >>>                     threshold=3)
+        >>> alg = rs.LinearPredictor({"Plot": 0}, rs.SkRidge(alpha=0.8))
 
+        * Interested in multiple field representations of the items, Ridge regressor from sklearn with custom
+        parameters, `only_greater_eq` $= 2$ (Every item with rating $>= 2$ will be discarded and not considered in the
+        ranking/score prediction task)
+
+        >>> alg = rs.LinearPredictor(
+        >>>                         item_field={"Plot": [0, "tfidf"],
+        >>>                                     "Genre": [0, 1],
+        >>>                                     "Director": "doc2vec"},
+        >>>                         regressor=rs.SkRidge(alpha=0.8),
+        >>>                         only_greater_eq=2)
 
         !!! info
 
-            After instantiating the IndexQuery algorithm, pass it in the initialization of
-            a CBRS and the use its method to calculate ranking for single user or multiple users:
+            After instantiating the `LinearPredictor` algorithm, pass it in the initialization of
+            a CBRS and the use its method to predict ratings or calculate ranking for a single user or multiple users:
 
             Examples:
 
                 >>> cbrs = rs.ContentBasedRS(algorithm=alg, ...)
+                >>> cbrs.fit_predict(...)
                 >>> cbrs.fit_rank(...)
                 >>> # ...
 
     Args:
         item_field: dict where the key is the name of the field
             that contains the content to use, value is the representation(s) id(s) that will be
-            used for the said item, just BE SURE to use textual representation(s). The value of a field can be a string
-            or a list, use a list if you want to use multiple representations for a particular field.
-        classic_similarity: True if you want to use the classic implementation of tfidf in Whoosh,
-            False if you want BM25F
-        threshold: Threshold for the ratings. If the rating is greater than the threshold, it will be considered
-            as positive. If the threshold is not specified, the average score of all items liked by the user is used.
+            used for the said item. The value of a field can be a string or a list,
+            use a list if you want to use multiple representations for a particular field.
+        regressor: regressor that will be used. Can be one object of the `Regressor` class.
+        only_greater_eq: Threshold for the ratings. Only items with rating greater or equal than the
+            threshold will be considered, items with lower rating will be discarded. If None, no item will be filter out
+        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used, but they are in a
+            matrix form instead of a single vector (e.g. WordEmbedding representations have one
+            vector for each word). By default, the `Centroid` of the rows of the matrix is computed
     """
-    __slots__ = ('_string_query', '_scores', '_positive_user_docs', '_classic_similarity')
-
-    def __init__(self, item_field: dict, classic_similarity: bool = True, threshold: float = None):
-        super().__init__(item_field, threshold)
-        self._string_query: Optional[str] = None
-        self._scores: Optional[list] = None
-        self._positive_user_docs: Optional[dict] = None
-        self._classic_similarity: bool = classic_similarity
+    __slots__ = ('_regressor', '_labels', '_items_features', '_embedding_combiner')
 
-    def _get_representations(self, index_representations: dict):
-        """
-        Private method which extracts representation(s) chosen from all representations codified for the items
-        extracted from the index
+    def __init__(self, item_field: dict, regressor: Regressor, only_greater_eq: float = None,
+                 embedding_combiner: CombiningTechnique = Centroid()):
+        super().__init__(item_field, only_greater_eq)
+        self._regressor = regressor
+        self._labels: Optional[list] = None
+        self._items_features: Optional[list] = None
+        self._embedding_combiner = embedding_combiner
 
-        Args:
-            index_representations (dict): representations for an item extracted from the index
+    def process_rated(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict):
         """
-        def find_valid(pattern: str):
-            field_index_retrieved = [field_index for field_index in index_representations
-                                     if re.match(pattern, field_index)]
-
-            if len(field_index_retrieved) == 0:
-                raise KeyError("Id {} not found for the field {}".format(id, k))
-            elif len(field_index_retrieved) > 1:
-                raise ValueError("This shouldn't happen! Duplicate fields?")
-            else:
-                valid = field_index_retrieved[0]
-
-            return valid
-
-        representations_valid = {}
-        for k in self.item_field:
-            for id in self.item_field[k]:
-                # every representation for an item is codified like this: plot#0#tfidf
-                if isinstance(id, str):
-                    pattern = "^{}#.+#{}$".format(k, id)
-                else:
-                    # the id passed it's a int
-                    pattern = "^{}#{}.*$".format(k, id)
-
-                valid_key = find_valid(pattern)
-                representations_valid[valid_key] = index_representations[valid_key]
+        Function that extracts features from rated item and labels them.
+        The extracted features will be later used to fit the regressor.
 
-        return representations_valid
+        Features and labels (in this case the rating score) will be stored in private attributes of the class.
 
-    def _load_available_contents(self, index_path: str, items_to_load: set = None):
-        return LoadedContentsIndex(index_path)
-
-    def process_rated(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsIndex):
-        """
-        Function that extracts features from positive rated items ONLY!
-        The extracted features will be used to fit the algorithm (build the query).
-
-        Features extracted will be stored in private attributes of the class.
+        IF there are no rated items available locally, an exception is thrown.
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user (the user for which we must fit the algorithm)
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
+
+        Raises:
+            EmptyUserRatings: Exception raised when the user does not appear in the train set
+            NoRatedItems: Exception raised when there isn't any item available locally
+                rated by the user
         """
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        rated_items_id = train_ratings.item_map.convert_seq_int2str(uir_user[:, 1].astype(int))
+
         # a list since there could be duplicate interaction (eg bootstrap partitioning)
         items_scores_dict = defaultdict(list)
-        for interaction in user_ratings:
-            items_scores_dict[interaction.item_id].append(interaction.score)
+
+        for item_id, score in zip(rated_items_id, uir_user[:, 2]):
+            items_scores_dict[item_id].append(score)
 
         items_scores_dict = dict(sorted(items_scores_dict.items()))  # sort dictionary based on key for reproducibility
 
-        threshold = self.threshold
-        if threshold is None:
-            threshold = self._calc_mean_user_threshold(user_ratings)
-
-        # Initializes positive_user_docs which is a list that has tuples with document_id as first element and
-        # a dictionary as second. The dictionary value has the name of the field as key
-        # and its contents as value. By doing so we obtain the data of the fields while
-        # also storing information regarding the field and the document where it was
-        scores = []
-        positive_user_docs = []
-
-        ix = available_loaded_items.get_contents_interface()
-
-        # we extract feature of each item sorted based on its key: IMPORTANT for reproducibility!!
-        for item_id, score_list in items_scores_dict.items():
-
-            score_assigned = map(float, score_list)
-
-            for score in score_assigned:
-                if score >= threshold:
-                    # {item_id: {"item": item_dictionary, "score": item_score}}
-                    item_query = ix.query(item_id, results_number=1, classic_similarity=self._classic_similarity)
-                    if len(item_query) != 0:
-                        item = item_query.pop(item_id).get('item')
-                        scores.append(score)
-                        positive_user_docs.append((item_id, self._get_representations(item)))
+        # Create list of all the available items that are useful for the user
+        loaded_rated_items: List[Union[Content, None]] = available_loaded_items.get_list([item_id
+                                                                                          for item_id
+                                                                                          in rated_items_id])
+
+        # Assign label and extract features from the rated items
+        labels = []
+        items_features = []
+
+        for item in loaded_rated_items:
+            if item is not None:
+
+                score_assigned = map(float, items_scores_dict[item.content_id])
+
+                for score in score_assigned:
+                    if self.threshold is None or score >= self.threshold:
+                        items_features.append(self.extract_features_item(item))
+                        labels.append(score)
 
-        if len(user_ratings) == 0:
+        if len(uir_user[:, 1]) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_id = user_ratings[0].user_id
-        if len(positive_user_docs) == 0:
-            raise OnlyNegativeItems(f"User {user_id} - There are no rated items available locally or there are only "
-                                    f"negative items available locally!")
+        if len(items_features) == 0:
+            raise NoRatedItems("User {} - No rated item available locally!".format(user_idx))
 
-        self._positive_user_docs = positive_user_docs
-        self._scores = scores
+        self._labels = labels
+        self._items_features = items_features
 
-    def fit(self):
+    def fit_single_user(self):
         """
-        The fit process for the IndexQuery consists in building a query using the features of the positive items ONLY
-        (items that the user liked). The terms relative to these 'positive' items are boosted by the
-        rating he/she gave.
-
-        This method uses extracted features of the positive items stored in a private attribute, so
-        process_rated() must be called before this method.
+        Fit the regressor specified in the constructor with the features and labels (rating scores)
+        extracted with the `process_rated()` method.
 
-        The built query will also be stored in a private attribute.
+        It uses private attributes to fit the regressor, so `process_rated()` must be called
+        before this method.
         """
-        # For each field of each document one string (containing the name of the field and the data in it)
-        # is created and added to the query.
-        # Also each part of the query that refers to a document
-        # is boosted by the score given by the user to said document
-        string_query = "("
-        for (doc_id, doc_data), score in zip(self._positive_user_docs, self._scores):
-            string_query += "("
-            for field_name in doc_data:
-                if field_name == 'content_id':
-                    continue
-                word_list = doc_data[field_name].split()
-                string_query += field_name + ":("
-                for term in word_list:
-                    string_query += term + " "
-                string_query += ") "
-            string_query += ")^" + str(score) + " "
-        string_query += ") "
+        # Fuse the input if there are dicts, multiple representation, etc.
+        fused_features = self.fuse_representations(self._items_features, self._embedding_combiner)
+
+        self._regressor.fit(fused_features, self._labels)
 
-        self._string_query = string_query
+        # we delete variables used to fit since will no longer be used
+        self._labels = None
+        self._items_features = None
 
-    def _build_mask_list(self, user_seen_items: set, filter_list: List[str] = None):
+    def _common_prediction_process(self, user_idx: int, train_ratings: Ratings,
+                                   available_loaded_items: LoadedContentsDict, filter_list: List[str] = None):
         """
-        Private function that calculate the mask query and the filter query for whoosh to use:
+        Simple private method which encapsulate common prediction process for both the `predict()` and `rank()`
+        method, to avoid duplicate code
+        """
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        if len(uir_user) == 0:
+            raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        - The mask query is needed to ignore items already rated by the user
-        - The filter query is needed to predict only items present in the filter_list
+        # Load items to predict
+        items_to_predict = available_loaded_items.get_list(filter_list)
 
-        If in the filter list there are items already rated by the user, those are excluded in the
-        mask query so that the prediction for those items can be calculated
+        # Extract features of the items to predict
+        idx_items_to_predict = []
+        features_items_to_predict = []
+        for item in items_to_predict:
+            if item is not None:
+                # raises AttributeError if items are not present locally
+                idx_items_to_predict.append(item.content_id)
+                features_items_to_predict.append(self.extract_features_item(item))
+
+        idx_items_to_predict = train_ratings.item_map.convert_seq_str2int(idx_items_to_predict)
+
+        if len(idx_items_to_predict) > 0:
+            # Fuse the input if there are dicts, multiple representation, etc.
+            fused_features_items_to_pred = self.fuse_representations(features_items_to_predict,
+                                                                     self._embedding_combiner)
+
+            score_labels = self._regressor.predict(fused_features_items_to_pred)
+        else:
+            score_labels = []
+
+        return idx_items_to_predict, score_labels
+
+    def predict_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                            filter_list: List[str]) -> np.ndarray:
+        """
+        Predicts how much a user will like unrated items.
+
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object, and
+        is a list of items represented with their string ids. Must be necessarily strings and not their mapped integer
+        since items are serialized following their string representation!
 
         Args:
-            user_seen_items: set of items present in the user profile
-            filter_list: list of the items to predict, if None all unrated items will be predicted
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
+            available_loaded_items: The LoadedContents interface which contains loaded contents
+            filter_list: list of the items to rank. Should contain string item ids
+
+        Returns:
+            uir matrix for a single user containing user and item idxs (integer representation) with the predicted score
+                as third dimension
         """
-        masked_list = list(user_seen_items)
-        if filter_list is not None:
-            masked_list = [item for item in user_seen_items if item not in filter_list]
 
-        return masked_list
+        idx_items_to_predict, score_labels = self._common_prediction_process(user_idx, train_ratings,
+                                                                             available_loaded_items,
+                                                                             filter_list)
+        if len(score_labels) != 0:
+            # Build the output data
+            uir_pred = np.array(
+                [[user_idx, item_idx, score] for item_idx, score in zip(idx_items_to_predict, score_labels)])
+        else:
+            uir_pred = np.array([])
 
-    def predict(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsIndex,
-                filter_list: List[str] = None) -> List[Interaction]:
-        """
-        IndexQuery is not a Prediction Score Algorithm, so if this method is called,
-        a NotPredictionAlg exception is raised
+        return uir_pred
 
-        Raises:
-            NotPredictionAlg: exception raised since the CentroidVector algorithm is not a score prediction algorithm
+    def rank_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                         recs_number: Optional[int], filter_list: List[str]) -> np.ndarray:
         """
-        raise NotPredictionAlg("IndexQuery is not a Score Prediction Algorithm!")
+        Rank the top-n recommended items for the active user, where the top-n items to rank are controlled by the
+        `recs_number` and `filter_list` parameter:
 
-    def rank(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsIndex,
-             recs_number: int = None, filter_list: List[str] = None) -> List[Interaction]:
-        """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
+        * the former one is self-explanatory, the second is a list of items
+        represented with their string ids. Must be necessarily strings and not their mapped integer since items are
+        serialized following their string representation!
+
+        If `recs_number` is `None`, all ranked items will be returned
 
-        One can specify which items must be ranked with the `filter_list` parameter,
-        in this case ONLY items in the `filter_list` parameter will be ranked.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, **ALL** unrated items will be ranked.
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object
 
         Args:
-            user_ratings: List of Interaction objects for a single user
-            available_loaded_items: The LoadedContents interface which contains loaded contents. In this case it will
-                be a `LoadedContentsIndex`
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
+            available_loaded_items: The LoadedContents interface which contains loaded contents
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
-            filter_list (list): list of the items to rank, if None all unrated items for the user will be ranked
+            filter_list: list of the items to rank. Should contain string item ids
 
         Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
+            uir matrix for a single user containing user and item idxs (integer representation) with the ranked score
+                as third dimension sorted in a decreasing order
         """
-        try:
-            user_id = user_ratings[0].user_id
-        except IndexError:
-            raise EmptyUserRatings("The user selected doesn't have any ratings!")
-
-        user_seen_items = set([interaction.item_id for interaction in user_ratings])
-
-        mask_list = self._build_mask_list(user_seen_items, filter_list)
-
-        ix = available_loaded_items.get_contents_interface()
-        score_docs = ix.query(self._string_query, recs_number, mask_list, filter_list, self._classic_similarity)
 
-        # we construct the output data
-        rank_interaction_list = [Interaction(user_id, item_id, score_docs[item_id]['score'])
-                                 for item_id in score_docs]
+        # Predict the rating for the items and sort them in descending order
+        idx_items_to_predict, score_labels = self._common_prediction_process(user_idx, train_ratings,
+                                                                             available_loaded_items,
+                                                                             filter_list)
+
+        if len(score_labels) != 0:
+            sorted_scores_idxs = np.argsort(score_labels)[::-1][:recs_number]
+            sorted_items = np.array(idx_items_to_predict)[sorted_scores_idxs]
+            sorted_scores = score_labels[sorted_scores_idxs]
+
+            # we construct the output data
+            uir_rank = np.array([[user_idx, item_idx, score] for item_idx, score in zip(sorted_items, sorted_scores)])
+        else:
+            uir_rank = np.array([])
 
-        return rank_interaction_list
+        return uir_rank
 
     def __str__(self):
-        return "IndexQuery"
+        return "LinearPredictor"
 
     def __repr__(self):
-        return f'IndexQuery(item_field={self.item_field}, classic_similarity={self._classic_similarity}, ' \
-               f'threshold={self.threshold})'
+        return f'LinearPredictor(item_field={self.item_field}, regressor={self._regressor}, ' \
+               f'only_greater_eq={self.threshold}, embedding_combiner={self._embedding_combiner})'
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/linear_predictor.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/classifier/classifier_recommender.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,260 @@
 from __future__ import annotations
+
 from collections import defaultdict
 from typing import List, Union, Optional, TYPE_CHECKING
 
+import numpy as np
+
 if TYPE_CHECKING:
     from clayrs.content_analyzer import Content
     from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
         CombiningTechnique
+    from clayrs.recsys.content_based_algorithm.classifier.classifiers import Classifier
     from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
-    from clayrs.recsys.content_based_algorithm.regressor.regressors import Regressor
+    from clayrs.content_analyzer.ratings_manager.ratings import Ratings
 
 from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
     Centroid
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-from clayrs.recsys.content_based_algorithm.exceptions import NoRatedItems, EmptyUserRatings
-from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
+from clayrs.recsys.content_based_algorithm.content_based_algorithm import PerUserCBAlgorithm
+from clayrs.recsys.content_based_algorithm.exceptions import NoRatedItems, OnlyPositiveItems, \
+    OnlyNegativeItems, NotPredictionAlg, EmptyUserRatings
 
 
-class LinearPredictor(ContentBasedAlgorithm):
+class ClassifierRecommender(PerUserCBAlgorithm):
     """
-    Class that implements recommendation through a specified linear predictor.
-    It's a score prediction algorithm, so it can predict what rating a user would give to an unseen item.
-    As such, it's also a ranking algorithm (it simply ranks in descending order unseen items by the predicted rating)
+    Class that implements recommendation through a specified `Classifier` object.
+    It's a ranking algorithm, so it can't do score prediction.
 
     Examples:
-
-        * Interested in only a field representation, LinearRegression regressor from sklearn
+        * Interested in only a field representation, `DecisionTree` classifier from sklearn,
+        `threshold` $= 3$ (Every item with rating score $>= 3$ will be considered as *positive*)
 
         >>> from clayrs import recsys as rs
-        >>> alg = rs.LinearPredictor({"Plot": 0}, rs.SkLinearRegression())
+        >>> alg = rs.ClassifierRecommender({"Plot": 0}, rs.SkDecisionTree(), 3)
 
-        * Interested in only a field representation, Ridge regressor from sklearn with custom parameters
+        * Interested in only a field representation, `KNN` classifier with custom parameters from sklearn,
+        `threshold` $= 3$ (Every item with rating score $>= 3$ will be considered as positive)
 
-        >>> alg = rs.LinearPredictor({"Plot": 0}, rs.SkRidge(alpha=0.8))
+        >>> alg = rs.ClassifierRecommender({"Plot": 0}, rs.SkKNN(n_neighbors=3), 0)
 
-        * Interested in multiple field representations of the items, Ridge regressor from sklearn with custom
-        parameters, $only_greater_eq = 2$ (Every item with rating $>= 2$ will be discarded and not considered in the
-        ranking/score prediction task)
-
-        >>> alg = rs.LinearPredictor(
-        >>>                         item_field={"Plot": [0, "tfidf"],
-        >>>                                     "Genre": [0, 1],
-        >>>                                     "Director": "doc2vec"},
-        >>>                         regressor=rs.SkRidge(alpha=0.8),
-        >>>                         only_greater_eq=2)
+        * Interested in multiple field representations of the items, `KNN` classifier with custom parameters from
+        sklearn, `threshold` $= None$ (Every item with rating $>=$ mean rating of the user will be considered as positive)
+
+        >>> alg = ClassifierRecommender(
+        >>>                             item_field={"Plot": [0, "tfidf"],
+        >>>                                         "Genre": [0, 1],
+        >>>                                         "Director": "doc2vec"},
+        >>>                             classifier=rs.SkKNN(n_neighbors=3),
+        >>>                             threshold=None)
 
         !!! info
 
-            After instantiating the LinearPredictor algorithm, pass it in the initialization of
-            a CBRS and the use its method to predict ratings or calculate ranking for a single user or multiple users:
+            After instantiating the ClassifierRecommender` algorithm, pass it in the initialization of
+            a CBRS and the use its method to calculate ranking for single user or multiple users:
 
             Examples:
 
                 >>> cbrs = rs.ContentBasedRS(algorithm=alg, ...)
-                >>> cbrs.fit_predict(...)
                 >>> cbrs.fit_rank(...)
                 >>> # ...
 
+
     Args:
-        item_field: dict where the key is the name of the field
+        item_field (dict): dict where the key is the name of the field
             that contains the content to use, value is the representation(s) id(s) that will be
             used for the said item. The value of a field can be a string or a list,
             use a list if you want to use multiple representations for a particular field.
-        regressor: regressor that will be used. Can be one object of the `Regressor` class.
-        only_greater_eq: Threshold for the ratings. Only items with rating greater or equal than the
-            threshold will be considered, items with lower rating will be discarded. If None, no item will be filter out
-        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used but they are in a
-            matrix form instead of a single vector (e.g. when WordEmbedding representations must be used you have one
-            vector for each word). By default the `Centroid` of the rows of the matrix is computed
+        classifier (Classifier): classifier that will be used. Can be one object of the Classifier class.
+        threshold: Threshold for the ratings. If the rating is greater than the threshold, it will be considered
+            as positive. If the threshold is not specified, the average score of all items rated by the user is used.
+        embedding_combiner: `CombiningTechnique` used when embeddings representation must be used, but they are in a
+            matrix form instead of a single vector (e.g. WordEmbedding representations have one
+            vector for each word). By default, the `Centroid` of the rows of the matrix is computed
     """
-    __slots__ = ('_regressor', '_labels', '_items_features', '_embedding_combiner')
+    __slots__ = ('_classifier', '_embedding_combiner', '_labels', '_items_features')
 
-    def __init__(self, item_field: dict, regressor: Regressor, only_greater_eq: float = None,
+    def __init__(self, item_field: dict, classifier: Classifier, threshold: float = None,
                  embedding_combiner: CombiningTechnique = Centroid()):
-        super().__init__(item_field, only_greater_eq)
-        self._regressor = regressor
+        super().__init__(item_field, threshold)
+
+        self._classifier = classifier
+        self._embedding_combiner = embedding_combiner
         self._labels: Optional[list] = None
         self._items_features: Optional[list] = None
-        self._embedding_combiner = embedding_combiner
 
-    def process_rated(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict):
+    def process_rated(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict):
         """
         Function that extracts features from rated item and labels them.
         The extracted features will be later used to fit the classifier.
 
-        Features and labels (in this case the rating score) will be stored in private attributes of the class.
+        Features and labels will be stored in private attributes of the class.
 
-        IF there are no rated items available locally, an exception is thrown.
+        IF there are no rated items available locally or if there are only positive/negative
+        items, an exception is thrown.
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user (the user for which we must fit the algorithm)
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
 
         Raises:
+            EmptyUserRatings: Exception raised when the user does not appear in the train set
             NoRatedItems: Exception raised when there isn't any item available locally
                 rated by the user
+            OnlyPositiveItems: Exception raised when there are only positive items available locally
+                for the user (Items that the user liked)
+            OnlyNegativeitems: Exception raised when there are only negative items available locally
+                for the user (Items that the user disliked)
         """
+
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        rated_items_id = train_ratings.item_map.convert_seq_int2str(uir_user[:, 1].astype(int))
+
         # a list since there could be duplicate interaction (eg bootstrap partitioning)
         items_scores_dict = defaultdict(list)
-        for interaction in user_ratings:
-            items_scores_dict[interaction.item_id].append(interaction.score)
+
+        for item_id, score in zip(rated_items_id, uir_user[:, 2]):
+            items_scores_dict[item_id].append(score)
 
         items_scores_dict = dict(sorted(items_scores_dict.items()))  # sort dictionary based on key for reproducibility
 
         # Create list of all the available items that are useful for the user
         loaded_rated_items: List[Union[Content, None]] = available_loaded_items.get_list([item_id
                                                                                           for item_id
-                                                                                          in items_scores_dict.keys()])
+                                                                                          in rated_items_id])
+
+        threshold = self.threshold
+        if threshold is None:
+            threshold = np.nanmean(uir_user[:, 2])
 
         # Assign label and extract features from the rated items
         labels = []
         items_features = []
 
+        # we extract feature of each item sorted based on its key: IMPORTANT for reproducibility!!
+        # otherwise the matrix we feed to sklearn will have input item in different rows each run!
         for item in loaded_rated_items:
             if item is not None:
 
                 score_assigned = map(float, items_scores_dict[item.content_id])
 
                 for score in score_assigned:
-                    if self.threshold is None or score >= self.threshold:
-                        items_features.append(self.extract_features_item(item))
-                        labels.append(score)
+                    items_features.append(self.extract_features_item(item))
 
-        if len(user_ratings) == 0:
+                    if score >= threshold:
+                        labels.append(1)
+                    else:
+                        labels.append(0)
+
+        if len(uir_user[:, 1]) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        user_id = user_ratings[0].user_id
         if len(items_features) == 0:
-            raise NoRatedItems("User {} - No rated item available locally!".format(user_id))
+            raise NoRatedItems("User {} - No rated item available locally!".format(user_idx))
+        if 0 not in labels:
+            raise OnlyPositiveItems("User {} - There are only positive items available locally!".format(user_idx))
+        elif 1 not in labels:
+            raise OnlyNegativeItems("User {} - There are only negative items available locally!".format(user_idx))
 
         self._labels = labels
         self._items_features = items_features
 
-    def fit(self):
+    def fit_single_user(self):
         """
-        Fit the regressor specified in the constructor with the features and labels (rating scores)
-        extracted with the process_rated() method.
+        Fit the classifier specified in the constructor with the features and labels
+        extracted with the `process_rated()` method.
 
-        It uses private attributes to fit the classifier, so process_rated() must be called
+        It uses private attributes to fit the classifier, so `process_rated()` must be called
         before this method.
         """
         # Fuse the input if there are dicts, multiple representation, etc.
         fused_features = self.fuse_representations(self._items_features, self._embedding_combiner)
 
-        self._regressor.fit(fused_features, self._labels)
+        self._classifier.fit(fused_features, self._labels)
 
         # we delete variables used to fit since will no longer be used
-        self._labels = None
         self._items_features = None
+        self._labels = None
 
-    def _common_prediction_process(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-                                   filter_list: List[str] = None):
-
-        user_seen_items = set([interaction.item_id for interaction in user_ratings])
-
-        # Load items to predict
-        if filter_list is None:
-            items_to_predict = available_loaded_items.get_list([item_id
-                                                                for item_id in available_loaded_items
-                                                                if item_id not in user_seen_items])
-        else:
-            items_to_predict = available_loaded_items.get_list(filter_list)
+    def predict_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                            filter_list: List[str] = None) -> np.ndarray:
+        """
+        ClassifierRecommender is not a score prediction algorithm, calling this method will raise
+        the `NotPredictionAlg` exception!
 
-        # Extract features of the items to predict
-        id_items_to_predict = []
-        features_items_to_predict = []
-        for item in items_to_predict:
-            if item is not None:
-                # raises AttributeError if items are not present locally
-                id_items_to_predict.append(item.content_id)
-                features_items_to_predict.append(self.extract_features_item(item))
+        Raises:
+            NotPredictionAlg: exception raised since the ClassifierRecommender algorithm is not a
+                score prediction algorithm
+        """
+        raise NotPredictionAlg("ClassifierRecommender is not a Score Prediction Algorithm!")
 
-        if len(id_items_to_predict) > 0:
-            # Fuse the input if there are dicts, multiple representation, etc.
-            fused_features_items_to_pred = self.fuse_representations(features_items_to_predict,
-                                                                     self._embedding_combiner)
-
-            score_labels = self._regressor.predict(fused_features_items_to_pred)
-        else:
-            score_labels = []
+    def rank_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                         recs_number: Optional[int], filter_list: List[str]) -> np.ndarray:
+        """
+        Rank the top-n recommended items for the active user, where the top-n items to rank are controlled by the
+        `recs_number` and `filter_list` parameter:
 
-        return id_items_to_predict, score_labels
+        * the former one is self-explanatory, the second is a list of items
+        represented with their string ids. Must be necessarily strings and not their mapped integer since items are
+        serialized following their string representation!
 
-    def predict(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-                filter_list: List[str] = None) -> List[Interaction]:
-        """
-        Predicts how much a user will like unrated items.
+        If `recs_number` is `None`, all ranked items will be returned
 
-        One can specify which items must be predicted with the filter_list parameter,
-        in this case ONLY items in the filter_list will be predicted.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, ALL unrated items will be predicted.
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object
 
         Args:
-            user_ratings: List of Interaction objects for a single user
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
             available_loaded_items: The LoadedContents interface which contains loaded contents
-            filter_list: List of the items to predict, if None all unrated items for the user will be predicted
+            recs_number: number of the top ranked items to return, if None all ranked items will be returned
+            filter_list: list of the items to rank. Should contain string item ids
 
         Returns:
-            List of Interactions object where the 'score' attribute is the rating predicted by the algorithm
+            uir matrix for a single user containing user and item idxs (integer representation) with the ranked score
+                as third dimension sorted in a decreasing order
         """
-        try:
-            user_id = user_ratings[0].user_id
-        except IndexError:
+
+        uir_user = train_ratings.get_user_interactions(user_idx)
+        if len(uir_user) == 0:
             raise EmptyUserRatings("The user selected doesn't have any ratings!")
 
-        id_items_to_predict, score_labels = self._common_prediction_process(user_ratings, available_loaded_items,
-                                                                            filter_list)
+        # Load items to predict
+        items_to_predict = available_loaded_items.get_list(filter_list)
 
-        # Build the output data
-        pred_interaction_list = [Interaction(user_id, item_id, score)
-                                 for item_id, score in zip(id_items_to_predict, score_labels)]
+        # Extract features of the items to predict
+        idx_items_to_predict = []
+        features_items_to_predict = []
+        for item in items_to_predict:
+            if item is not None:
+                idx_items_to_predict.append(item.content_id)
+                features_items_to_predict.append(self.extract_features_item(item))
 
-        return pred_interaction_list
+        if len(idx_items_to_predict) == 0:
+            return np.array([])  # if no item to predict, empty rank is returned
 
-    def rank(self, user_ratings: List[Interaction], available_loaded_items: LoadedContentsDict,
-             recs_number: int = None, filter_list: List[str] = None) -> List[Interaction]:
-        """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
+        idx_items_to_predict = train_ratings.item_map.convert_seq_str2int(idx_items_to_predict)
 
-        One can specify which items must be ranked with the `filter_list` parameter,
-        in this case ONLY items in the `filter_list` parameter will be ranked.
-        One can also pass items already seen by the user with the filter_list parameter.
-        Otherwise, **ALL** unrated items will be ranked.
+        # Fuse the input if there are dicts, multiple representation, etc.
+        fused_features_items_to_pred = self.fuse_representations(features_items_to_predict,
+                                                                 self._embedding_combiner)
 
-        Args:
-            user_ratings: List of Interaction objects for a single user
-            available_loaded_items: The LoadedContents interface which contains loaded contents
-            recs_number: number of the top ranked items to return, if None all ranked items will be returned
-            filter_list (list): list of the items to rank, if None all unrated items for the user will be ranked
+        class_prob = self._classifier.predict_proba(fused_features_items_to_pred)
 
-        Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
-        """
-        try:
-            user_id = user_ratings[0].user_id
-        except IndexError:
-            raise EmptyUserRatings("The user selected doesn't have any ratings!")
+        # for each item we extract the probability that the item is liked (class 1)
+        sorted_scores_idxs = np.argsort(class_prob[:, 1])[::-1][:recs_number]
+        sorted_items = np.array(idx_items_to_predict)[sorted_scores_idxs]
+        sorted_scores = class_prob[:, 1][sorted_scores_idxs]
 
-        # Predict the rating for the items and sort them in descending order
-        id_items_to_predict, score_labels = self._common_prediction_process(user_ratings, available_loaded_items,
-                                                                            filter_list)
-
-        # Build the item_score dict (key is item_id, value is rank score predicted)
-        # and order the keys in descending order
-        item_score_dict = dict(zip(id_items_to_predict, score_labels))
-        ordered_item_ids = sorted(item_score_dict, key=item_score_dict.get, reverse=True)
-
-        # we only save the top-n items_ids corresponding to top-n recommendations
-        # (if recs_number is None ordered_item_ids will contain all item_ids as the original list)
-        ordered_item_ids = ordered_item_ids[:recs_number]
-
-        # we construct the output data
-        rank_interaction_list = [Interaction(user_id, item_id, item_score_dict[item_id])
-                                 for item_id in ordered_item_ids]
+        uir_rank = np.array([[user_idx, item_idx, score]
+                             for item_idx, score in zip(sorted_items, sorted_scores)])
 
-        return rank_interaction_list
+        return uir_rank
 
     def __str__(self):
-        return "LinearPredictor"
+        return "ClassifierRecommender"
 
     def __repr__(self):
-        return f'LinearPredictor(item_field={self.item_field}, regressor={self._regressor}, ' \
-               f'only_greater_eq={self.threshold}, embedding_combiner={self._embedding_combiner})'
+        return f'ClassifierRecommender(item_field={self.item_field}, ' \
+               f'classifier={self._classifier}, ' \
+               f'threshold={self.threshold}, ' \
+               f'embedding_combiner={self._embedding_combiner})'
```

### Comparing `clayrs-0.4.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/regressor/regressors.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/recsys/experiment.py` & `clayrs-0.5.1/clayrs/recsys/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import abc
 import os
 import shutil
 import sys
 from abc import ABC
 from typing import List, Union, Dict, Callable, TYPE_CHECKING, Optional
 
+import pyaml
+
+# fix circular import, for the future: move Ratings class to the RecSys module
 if TYPE_CHECKING:
     from clayrs.content_analyzer import Ratings
     from clayrs.evaluation.metrics.metrics import Metric
     from clayrs.recsys.algorithm import Algorithm
     from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
     from clayrs.recsys.graph_based_algorithm.graph_based_algorithm import GraphBasedAlgorithm
     from clayrs.recsys.partitioning import Partitioning
@@ -123,19 +126,27 @@
                 shutil.rmtree(self.output_folder)
                 os.makedirs(self.output_folder)
             else:
                 raise FileExistsError(f"Folder {self.output_folder} already present!\n"
                                       "Delete it and run the experiment again or set `overwrite_if_exists` parameter "
                                       "to True!") from None
 
+        # save user_map
+        with open(os.path.join(self.output_folder, "user_map.yml"), 'w') as yaml_file:
+            pyaml.dump(self.original_ratings.user_map.to_dict(), yaml_file, sort_dicts=False, safe=True)
+
+        # save item_map
+        with open(os.path.join(self.output_folder, "item_map.yml"), 'w') as yaml_file:
+            pyaml.dump(self.original_ratings.user_map.to_dict(), yaml_file, sort_dicts=False, safe=True)
+
         train_set_list, test_set_list = self.pt.split_all(self.original_ratings)
 
         for i, (train_set, test_set) in enumerate(zip(train_set_list, test_set_list)):
-            train_set.to_csv(self.output_folder, file_name=f"{str(self.pt)}_train_split{i}")
-            test_set.to_csv(self.output_folder, file_name=f"{str(self.pt)}_test_split{i}")
+            train_set.to_csv(self.output_folder, file_name=f"{str(self.pt)}_train_split{i}", ids_as_str=True)
+            test_set.to_csv(self.output_folder, file_name=f"{str(self.pt)}_test_split{i}", ids_as_str=True)
 
         for alg in self.algorithm_list:
 
             # Control variable that lets you skip directly to the next algorithm
             # when the NotPredictionAlg exception is raised but should be skipped
             skip_to_next_alg = False
 
@@ -308,15 +319,15 @@
                  output_folder: str = "experiment_result",
                  overwrite_if_exists: bool = False):
 
         super().__init__(original_ratings, partitioning_technique, algorithm_list, items_directory, users_directory,
                          metric_list, report, output_folder, overwrite_if_exists)
 
     def predict(self,
-                user_id_list: Optional[List[str]] = None,
+                user_id_list: Optional[Union[List[str], List[int]]] = None,
                 methodology: Optional[Methodology] = TestRatingsMethodology(),
                 num_cpus: int = 1,
                 skip_alg_error: bool = True) -> None:
         """
         Method used to perform an experiment which involves ***score predictions***.
 
         The method will first split the original ratings passed in the constructor in train and test set, then
@@ -350,30 +361,31 @@
             NotPredictionAlg: When a pure ranking algorithm is asked to perform score prediction and
                 `skip_alg_error` == False
         """
         def cb_fit_predict(split_num, alg, train_set, test_set, dirname):
             cbrs = ContentBasedRS(alg, train_set, self.items_directory)
 
             predict_alg = cbrs.fit_predict(test_set, methodology=methodology, num_cpus=num_cpus,
-                                           user_id_list=user_id_list)
+                                           user_list=user_id_list)
 
-            predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_predict_split{split_num}")
+            predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_predict_split{split_num}",
+                               ids_as_str=True)
 
             if self.report:
                 Report(output_dir=f"{self.output_folder}/{dirname}").yaml(original_ratings=self.original_ratings,
                                                                           partitioning_technique=self.pt,
                                                                           recsys=cbrs)
 
             return predict_alg
 
         self.main_experiment(cb_fit_predict, skip_alg_error=skip_alg_error)
 
     def rank(self,
              n_recs: Optional[int] = 10,
-             user_id_list: Optional[List[str]] = None,
+             user_id_list: Optional[Union[List[str], List[int]]] = None,
              methodology: Optional[Methodology] = TestRatingsMethodology(),
              num_cpus: int = 1):
         """
         Method used to perform an experiment which involves ***rankings***.
 
         The method will first split the original ratings passed in the constructor in train and test set, then
         the Recommender System will be fit for each user in the train.
@@ -395,17 +407,18 @@
                 the number of cpus will be automatically detected
 
         """
         def cb_fit_rank(split_num, alg, train_set, test_set, dirname):
             cbrs = ContentBasedRS(alg, train_set, self.items_directory)
 
             predict_alg = cbrs.fit_rank(test_set, n_recs=n_recs, methodology=methodology,
-                                        user_id_list=user_id_list, num_cpus=num_cpus)
+                                        user_list=user_id_list, num_cpus=num_cpus)
 
-            predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_rank_split{split_num}")
+            predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_rank_split{split_num}",
+                               ids_as_str=True)
 
             if self.report:
                 Report(output_dir=f"{self.output_folder}/{dirname}").yaml(original_ratings=self.original_ratings,
                                                                           partitioning_technique=self.pt,
                                                                           recsys=cbrs)
 
             return predict_alg
@@ -538,15 +551,15 @@
                          metric_list, report, output_folder, overwrite_if_exists)
 
         self.item_exo_properties = item_exo_properties
         self.user_exo_properties = user_exo_properties
         self.link_label = link_label
 
     def predict(self,
-                user_id_list: Optional[List[str]] = None,
+                user_id_list: Optional[Union[List[str], List[int]]] = None,
                 methodology: Optional[Methodology] = TestRatingsMethodology(),
                 num_cpus: int = 1,
                 skip_alg_error: bool = True):
         """
         Method used to perform an experiment which involves ***score predictions***.
 
         The method will first split the original ratings passed in the constructor in train and test set, then
@@ -591,30 +604,30 @@
 
             for user, item in zip(test_set.user_id_column, test_set.item_id_column):
                 graph.remove_link(UserNode(user), ItemNode(item))
 
             gbrs = GraphBasedRS(alg, graph)
 
             predict_alg = gbrs.predict(test_set, methodology=methodology,
-                                       num_cpus=num_cpus, user_id_list=user_id_list)
+                                       num_cpus=num_cpus, user_list=user_id_list)
 
             predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_predict_split{split_num}")
 
             if self.report:
                 Report(output_dir=f"{self.output_folder}/{dirname}").yaml(original_ratings=self.original_ratings,
                                                                           partitioning_technique=self.pt,
                                                                           recsys=gbrs)
 
             return predict_alg
 
         self.main_experiment(gb_fit_predict, skip_alg_error=skip_alg_error)
 
     def rank(self,
              n_recs: Optional[int] = 10,
-             user_id_list: Optional[List[str]] = None,
+             user_id_list: Optional[Union[List[str], List[int]]] = None,
              methodology: Optional[Methodology] = TestRatingsMethodology(),
              num_cpus: int = 1):
         """
         Method used to perform an experiment which involves ***rankings***.
 
         The method will first split the original ratings passed in the constructor in train and test set, then
         a graph will be built depending on them:
@@ -647,15 +660,15 @@
 
             for user, item in zip(test_set.user_id_column, test_set.item_id_column):
                 graph.remove_link(UserNode(user), ItemNode(item))
 
             gbrs = GraphBasedRS(alg, graph)
 
             predict_alg = gbrs.rank(test_set, n_recs=n_recs, methodology=methodology,
-                                    num_cpus=num_cpus, user_id_list=user_id_list)
+                                    num_cpus=num_cpus, user_list=user_id_list)
 
             predict_alg.to_csv(f"{self.output_folder}/{dirname}", file_name=f"rs_rank_split{split_num}")
 
             if self.report:
                 Report(output_dir=f"{self.output_folder}/{dirname}").yaml(original_ratings=self.original_ratings,
                                                                           partitioning_technique=self.pt,
                                                                           recsys=gbrs)
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py` & `clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/graph_based_algorithm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from __future__ import annotations
 import abc
-from typing import Dict, List, Set, Union, TYPE_CHECKING
+from typing import Dict, List, Set, Union, TYPE_CHECKING, Optional, Iterable
+
+import numpy as np
 
 if TYPE_CHECKING:
-    from clayrs.content_analyzer.ratings_manager.ratings import Interaction, Ratings
+    from clayrs.content_analyzer.ratings_manager.ratings import Ratings
     from clayrs.recsys.graphs.graph import UserNode, Node, Graph, BipartiteDiGraph
     from clayrs.recsys.methodology import Methodology
 
 from clayrs.recsys.graphs.graph import ItemNode
-from clayrs.recsys.methodology import TestRatingsMethodology
 from clayrs.recsys.algorithm import Algorithm
 
 
 class GraphBasedAlgorithm(Algorithm):
     """
     Abstract class for the graph-based algorithms
     """
 
     def __init__(self):
         # FUTURE WORK: this can be expanded in making the page rank keeping also PropertyNodes, etc.
         self._nodes_to_keep = {ItemNode}
 
-    def filter_result(self, graph: BipartiteDiGraph, result: Dict, filter_list: Union[List[Node], None],
+    def filter_result(self, graph: BipartiteDiGraph, result: Dict, filter_list: Union[Iterable[Node], None],
                       user_node: UserNode) -> Dict:
         """
         Method which filters and cleans the result dict based on the parameters passed
 
-        If `filter_list` parameter is not None, then the final dict will contains items and score only for items
+        If `filter_list` parameter is not None, then the final dict will contain items and score only for items
         in said `filter_list`
 
-        Otherwise if no filter list is specified, then all unrated items by the user will be returned in the final
+        Otherwise, if no filter list is specified, then all unrated items by the user will be returned in the final
         dict
 
         Args:
             graph: Directed graph which models interactions between users and items
             result: dictionary representing the result (keys are nodes and values are their score)
             filter_list: list of the items for which a ranking score/score prediction must be computed.
                 If None all unrated items for the user will be ranked/score predicted.
@@ -53,69 +54,60 @@
         else:
             extracted_profile = set(graph.get_successors(user_node))
             filtered_result = {k: result[k] for k in result.keys() if must_keep(k, extracted_profile)}
 
         return filtered_result
 
     @abc.abstractmethod
-    def predict(self, all_users: Set[str], graph: Graph, test_set: Ratings,
-                methodology: Union[Methodology, None] = TestRatingsMethodology(),
-                num_cpus: int = 1) -> List[Interaction]:
+    def predict(self, graph: Graph, train_set: Ratings, test_set: Ratings, user_id_list: Set[str],
+                methodology: Methodology, num_cpus: int) -> List[np.ndarray]:
         """
         Abstract method that predicts how much a user will like unrated items.
         If the algorithm is not a PredictionScore Algorithm, implement this method like this:
 
         ```python
         def predict():
             raise NotPredictionAlg
         ```
 
-        One can specify on which items score prediction must be performed for each user with the `filter_dict`
-        parameter, in this case every user is mapped with a list of items for which a prediction score must be computed.
-        Otherwise, for **ALL** unrated items a prediction score will be computed for each user.
-
         Args:
-            all_users: Set of user id for which a recommendation list must be generated
-            graph: A graph previously instantiated
+            graph: A graph which models interactions of users and items
+            train_set: a Ratings object containing interactions between users and items
             test_set: Ratings object which represents the ground truth of the split considered
+            user_id_list: Set of user id for which a recommendation list must be generated. Users should be represented
+                as strings rather than with their mapped integer
             methodology: `Methodology` object which governs the candidate item selection. Default is
                 `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+            num_cpus: number of processors that must be reserved for the method
 
         Returns:
-            List of Interactions object where the 'score' attribute is the rating predicted by the algorithm
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def rank(self, all_users: Set[str], graph: Graph, test_set: Ratings,
-             recs_number: int = None, methodology: Union[Methodology, None] = TestRatingsMethodology(),
-             num_cpus: int = 1) -> List[Interaction]:
+    def rank(self, graph: Graph, train_set: Ratings, test_set: Ratings, user_id_list: Set[str],
+             recs_number: Optional[int], methodology: Methodology, num_cpus: int) -> List[np.ndarray]:
         """
         Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
         All unrated items for the user will be ranked (or only items in the filter list, if specified).
 
         ```python
         def rank():
             raise NotRankingAlg
         ```
 
-        One can specify which items must be ranked for each user with the `filter_dict` parameter,
-        in this case every user is mapped with a list of items for which a ranking score must be computed.
-        Otherwise, **ALL** unrated items will be ranked for each user.
-
         Args:
-            all_users: Set of user id for which a recommendation list must be generated
-            graph: A graph previously instantiated
+            graph: A graph which models interactions of users and items
+            train_set: a Ratings object containing interactions between users and items
             test_set: Ratings object which represents the ground truth of the split considered
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
             methodology: `Methodology` object which governs the candidate item selection. Default is
                 `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+            num_cpus: number of processors that must be reserved for the method
 
         Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items sorted in a descending way w.r.t. the third dimension which is the ranked score
         """
         raise NotImplementedError
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py` & `clayrs-0.5.1/clayrs/recsys/graph_based_algorithm/page_rank/nx_page_rank.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from __future__ import annotations
-import itertools
-from typing import List, Set, Any, Union, TYPE_CHECKING, Optional
+from typing import Set, Any, TYPE_CHECKING, Optional, List
 
 import networkx as nx
 import numpy as np
 
 if TYPE_CHECKING:
     from clayrs.content_analyzer.ratings_manager.ratings import Ratings
     from clayrs.recsys.graphs import NXBipartiteGraph
     from clayrs.recsys.methodology import Methodology
 
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction
 from clayrs.recsys.graph_based_algorithm.page_rank.page_rank import PageRank
 from clayrs.recsys.graphs.graph import UserNode, ItemNode, PropertyNode
-from clayrs.recsys.methodology import TestRatingsMethodology
 from clayrs.utils.context_managers import get_iterator_parallel
 
 
 class NXPageRank(PageRank):
     r"""
     Page Rank algorithm based on the networkx implementation.
     Please note that it can only be used for instantiated NXGraphs
@@ -103,65 +100,66 @@
         # That's why we have these other variables
         self._strict_rel_items_weight = rel_items_weight == 0
         self._strict_rel_items_prop_weight = rel_items_prop_weight == 0
 
         super().__init__(personalized, relevance_threshold, rel_items_weight, rel_items_prop_weight,
                          default_nodes_weight)
 
-    def rank(self, all_users: Set[str], graph: NXBipartiteGraph, test_set: Ratings,
-             recs_number: int = None, methodology: Union[Methodology, None] = TestRatingsMethodology(),
-             num_cpus: int = 1) -> List[Interaction]:
+    def rank(self, graph: NXBipartiteGraph, train_set: Ratings, test_set: Ratings, user_id_list: Set[str],
+             recs_number: Optional[int], methodology: Methodology, num_cpus: int) -> List[np.ndarray]:
         """
-        Rank the top-n recommended items for the user. If the recs_number parameter isn't specified,
-        All unrated items for the user will be ranked (or only items in the filter list, if specified).
+        Rank the top-n recommended items for the user. If the `recs_number` parameter is set to None,
+        All unrated items for the user will be ranked among all those selected by the `methodology` parameter.
 
-        One can specify which items must be ranked for each user with the `filter_dict` parameter,
-        in this case every user is mapped with a list of items for which a ranking score must be computed.
-        Otherwise, **ALL** unrated items will be ranked for each user.
+        The train set contains basically the interactions modelled in the graph, and it is needed by the methodology
+        object
 
         Args:
-            all_users: Set of user id for which a recommendation list must be generated
-            graph: A NX graph previously instantiated
+            graph: A graph which models interactions of users and items
+            train_set: a Ratings object containing interactions between users and items
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
             test_set: Ratings object which represents the ground truth of the split considered
+            user_id_list: List of users for which you want to compute ranking. The list should contain user id as
+                strings and NOT user ids mapped to their integers
             recs_number: number of the top ranked items to return, if None all ranked items will be returned
             methodology: `Methodology` object which governs the candidate item selection. Default is
                 `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
         Returns:
-            List of Interactions object in a descending order w.r.t the 'score' attribute, representing the ranking for
-                a single user
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items sorted in a descending way w.r.t. the third dimension which is the ranked score
         """
 
-        def compute_single_rank(user_id):
+        def compute_single_rank(user_tuple):
 
             # nonlocal keyword allows to modify the score variable
             nonlocal scores
 
+            user_id, user_idx = user_tuple
             user_node = UserNode(user_id)
 
-            filter_list = None
-            if methodology is not None:
-                filter_list = set(ItemNode(item_to_rank) for item_to_rank in
-                                  methodology.filter_single(user_id, train_set, test_set))
+            filter_list = set(ItemNode(item_to_rank)
+                              for item_to_rank in
+                              train_set.item_map.convert_seq_int2str(methodology.filter_single(user_idx,
+                                                                                               train_set,
+                                                                                               test_set)))
 
             # run the pageRank
             if self._personalized is True:
 
-                user_ratings = train_set.get_user_interactions(user_id)
-                user_relevance_threshold = self._relevance_threshold or np.nanmean([interaction.score
-                                                                                    for interaction in user_ratings])
+                user_ratings = train_set.get_user_interactions(user_idx)
+                user_relevance_threshold = self._relevance_threshold or np.nanmean(user_ratings[:, 2])
 
                 pers_dict = {}
 
-                relevant_items = [ItemNode(interaction.item_id)
-                                  for interaction in user_ratings
-                                  if interaction.score >= user_relevance_threshold]
+                relevant_items = user_ratings[np.where(user_ratings[:, 2] >= user_relevance_threshold)][:, 1]
+                relevant_items = [ItemNode(item_node)
+                                  for item_node in train_set.item_map.convert_seq_int2str(relevant_items.astype(int))]
 
                 # If the prob is > 0 then add relevant nodes to personalization vector. (rel_items_weight True)
                 # But also if the prob is 0 and the user explicitly set this prob to 0, add relevant nodes to
                 # personalization vector (strict_rel_items_weight is True)
                 # But if the prob is 0 and the user set None, we will skip this and add relevant nodes with the
                 # default_nodes_weight! (rel_items_weight not True and strict_rel_items_weight not True)
                 if self._rel_items_weight or self._strict_rel_items_weight:
@@ -181,62 +179,60 @@
                         relevant_props.update(relevant_item_properties)
 
                     pers_dict.update({prop_node: self._rel_items_prop_weight / len(relevant_props)
                                       for prop_node in relevant_props})
 
                 # all nodes that are not present up until now in the personalization vector, will be added
                 # with probability 'default_nodes_weight'
-                other_nodes = nx_graph.nodes - pers_dict.keys()
+                other_nodes = networkx_graph.nodes - pers_dict.keys()
                 pers_dict.update({node: self._default_nodes_weight / len(other_nodes) for node in other_nodes})
 
-                scores = nx.pagerank(nx_graph, personalization=pers_dict, alpha=self.alpha,
+                scores = nx.pagerank(networkx_graph, personalization=pers_dict, alpha=self.alpha,
                                      max_iter=self.max_iter, tol=self.tol, nstart=self.nstart, weight=weight)
 
             # if scores is None it means this is the first time we are running normal pagerank
             # for all the other users the pagerank won't be computed again
             elif scores is None:
-                scores = nx.pagerank(nx_graph, alpha=self.alpha, max_iter=self.max_iter,
+                scores = nx.pagerank(networkx_graph, alpha=self.alpha, max_iter=self.max_iter,
                                      tol=self.tol, nstart=self.nstart, weight=weight)
 
             # clean the results removing user nodes, selected user profile and eventually properties
             user_scores = self.filter_result(graph, scores, filter_list, user_node)
 
-            # Build the item_score dict (key is item_id, value is rank score predicted)
-            # and order the keys in descending order
-            item_score_dict = dict(zip([node.value for node in user_scores.keys()], user_scores.values()))
-            ordered_item_ids = sorted(item_score_dict, key=item_score_dict.get, reverse=True)
-
-            # we only save the top-n items_ids corresponding to top-n recommendations
-            # (if recs_number is None ordered_item_ids will contain all item_ids as the original list)
-            ordered_item_ids = ordered_item_ids[:recs_number]
-
-            # we construct the output data
-            single_rank_interaction_list = [Interaction(user_id, item_id, item_score_dict[item_id])
-                                            for item_id in ordered_item_ids]
+            if len(user_scores) == 0:
+                return user_id, np.array([])  # if no item to predict, empty rank is returned
 
-            return user_id, single_rank_interaction_list
+            user_scores_arr = np.array(list(user_scores.items()))
+
+            sorted_scores_idxs = np.argsort(user_scores_arr[:, 1])[::-1][:recs_number]
+            user_scores_arr = user_scores_arr[sorted_scores_idxs]
+
+            user_col = np.full((user_scores_arr.shape[0], 1), user_id)
+            uir_rank = np.append(user_col, user_scores_arr, axis=1)
+
+            return user_id, uir_rank
 
         # scores will contain pagerank scores
         scores = None
-        all_rank_interaction_list = []
+        all_rank_uirs_list = []
         weight = 'weight' if self.weight is True else None
-        train_set = graph.to_ratings()
-        nx_graph = graph.to_networkx()
+        networkx_graph = graph.to_networkx()
+        user_idxs_list = train_set.user_map.convert_seq_str2int(list(user_id_list))
 
         with get_iterator_parallel(num_cpus,
-                                   compute_single_rank, all_users,
-                                   progress_bar=True, total=len(all_users)) as pbar:
+                                   compute_single_rank, zip(user_id_list, user_idxs_list),
+                                   progress_bar=True, total=len(user_id_list)) as pbar:
 
             pbar.set_description("Prepping rank...")
 
             for user_id, user_rank in pbar:
-                all_rank_interaction_list.append(user_rank)
+                all_rank_uirs_list.append(user_rank)
                 pbar.set_description(f"Computing rank for user {user_id}")
 
-        return list(itertools.chain.from_iterable(all_rank_interaction_list))
+        return all_rank_uirs_list
 
     def __str__(self):
         return "NXPageRank"
 
     def __repr__(self):
         return f"NXPageRank(alpha={self.alpha}, personalized={self._personalized}, max_iter={self.max_iter}, " \
                f"tol={self.tol}, nstart={self.nstart}, weight={self.weight}, " \
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py` & `clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/feature_selection_alg.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py` & `clayrs-0.5.1/clayrs/recsys/graphs/feature_selection/feature_selection_fn.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         item_target_nodes (list): List of item nodes to consider in the feature selection process: only properties
             of item nodes in this list will be "reduced"
         inplace: Boolean parameter that let you choose if changes must be performed on the original graph
             (`inplace=True`) or on its copy (`inplace=False`). Default is False
 
     Returns:
         Copy of the original graph from which the less important Property nodes (the ones having edges with less
-        important property labels) will be removed
+            important property labels) will be removed
     """
     if fs_algorithm_user is not None and user_target_nodes is None:
         user_target_nodes = graph.user_nodes
 
     if fs_algorithm_item is not None and item_target_nodes is None:
         item_target_nodes = graph.item_nodes
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graphs/graph.py` & `clayrs-0.5.1/clayrs/recsys/graphs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pickle
 import lzma
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import List, Set, Union, Iterable, Dict
 
 from clayrs.recsys.graphs.graph_metrics import GraphMetrics
-from clayrs.content_analyzer.ratings_manager.ratings import Interaction, Ratings
+from clayrs.content_analyzer.ratings_manager.ratings import Ratings
 
 
 class Node(ABC):
     """
     Abstract class that generalizes the concept of a Node
 
     The Node stores the actual value of the node in the 'value' attribute
@@ -237,25 +237,24 @@
     def get_successors(self, node: Node) -> List[Node]:
         """
         Get all successors of a node
         """
         raise NotImplementedError
 
     # will only contain users and items
-    def to_ratings(self):
+    def to_ratings(self, user_map=None, item_map=None):
 
         node_list = list(self.user_nodes)
 
-        interaction_list = [Interaction(node.value, succ.value,
-                                        float(self.get_link_data(node, succ).get('weight')))
+        interaction_list = [(node.value, succ.value, float(self.get_link_data(node, succ).get('weight')))
                             for node in node_list
                             for succ in self.get_successors(node)
                             if isinstance(succ, ItemNode) and self.get_link_data(node, succ).get('weight')]
 
-        return Ratings.from_list(interaction_list)
+        return Ratings.from_list(interaction_list, user_map=user_map, item_map=item_map)
 
 
 class TripartiteDiGraph(BipartiteDiGraph):
     """
     Abstract class that generalize the concept of a TripartiteGraph
 
     A TripartiteGraph is a Graph containing 'user', 'item' and 'property' nodes, but the latter ones
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py` & `clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,30 +67,40 @@
         self._graph = nx.DiGraph()
 
         if source_frame is not None:
             not_none_dict = {}
             if link_label is not None:
                 not_none_dict['label'] = link_label
 
-            with get_progbar(source_frame) as progbar:
+            user_column = source_frame.user_id_column
+            item_column = source_frame.item_id_column
+            score_column = source_frame.score_column
+            timestamp_column = source_frame.timestamp_column
+
+            if len(timestamp_column) != 0:
+                frame_iterator = zip(user_column, item_column, score_column, timestamp_column)
+            else:
+                frame_iterator = zip(user_column, item_column, score_column)
+
+            with get_progbar(frame_iterator, total=len(source_frame)) as progbar:
                 progbar.set_description("Creating User->Item links")
 
-                if len(source_frame.timestamp_column) != 0:
-                    edges_with_attributes_gen = ((UserNode(interaction.user_id), ItemNode(interaction.item_id),
+                if len(timestamp_column) != 0:
+                    edges_with_attributes_gen = ((UserNode(interaction[0]), ItemNode(interaction[1]),
 
                                                   # {**x, **y} merges the dicts x and y
-                                                  {**not_none_dict, **{'weight': interaction.score,
-                                                                       'timestamp': interaction.timestamp}}
+                                                  {**not_none_dict, **{'weight': interaction[2],
+                                                                       'timestamp': interaction[3]}}
                                                   )
                                                  for interaction in progbar)
                 else:
-                    edges_with_attributes_gen = ((UserNode(interaction.user_id), ItemNode(interaction.item_id),
+                    edges_with_attributes_gen = ((UserNode(interaction[0]), ItemNode(interaction[1]),
 
                                                   # {**x, **y} merges the dicts x and y
-                                                  {**not_none_dict, **{'weight': interaction.score}})
+                                                  {**not_none_dict, **{'weight': interaction[2]}})
                                                  for interaction in progbar)
 
                 self._graph.add_edges_from(edges_with_attributes_gen)
 
     @property
     def user_nodes(self) -> Set[UserNode]:
         """
@@ -256,15 +266,14 @@
         ```
 
         Args:
             node: Node for which we want to know the successors
 
         Raises:
             TypeError: Exception raised when the node it's not in the graph
-
         """
         try:
             return list(self._graph.successors(node))
         except nx.NetworkXError:
             raise TypeError("The node specified is not in the graph!")
 
     def node_exists(self, node: Node) -> bool:
```

### Comparing `clayrs-0.4.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py` & `clayrs-0.5.1/clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             logger.warning("`user_exo_properties` parameter set but `user_contents_dir` is None! "
                            "No property will be loaded")
         elif not user_exo_properties and user_contents_dir:
             logger.warning("`user_contents_dir` parameter set but `user_exo_properties` is None! "
                            "No property will be loaded")
 
         if source_frame is not None and user_contents_dir is not None and user_exo_properties is not None:
-            self.add_node_with_prop([UserNode(user_id) for user_id in set(source_frame.user_id_column)],
+            self.add_node_with_prop([UserNode(user_id) for user_id in source_frame.unique_user_id_column],
                                     user_exo_properties,
                                     user_contents_dir)
 
     def add_node(self, node: Union[Node, List[Node]]):
         """
         Adds one or multiple Node objects to the graph.
         Since this is a Full Graph, any category of node is allowed
```

### Comparing `clayrs-0.4.1/clayrs/recsys/partitioning.py` & `clayrs-0.5.1/clayrs/recsys/partitioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,139 @@
-from __future__ import annotations
 from collections import defaultdict
 
-from typing import Set, List, Tuple, TYPE_CHECKING
+from typing import Set, List, Tuple, Union
 
 import abc
 from abc import ABC
 
+import numpy as np
 from sklearn.model_selection import KFold, train_test_split
 from sklearn.utils import resample
 
-if TYPE_CHECKING:
-    from clayrs.content_analyzer.ratings_manager.ratings import Interaction
-
 from clayrs.content_analyzer.ratings_manager.ratings import Ratings
 from clayrs.utils.const import logger
 from clayrs.utils.context_managers import get_progbar
 
 
 class Partitioning(ABC):
     """
     Abstract class for partitioning technique. Each class must implement the `split_single()` method which specify how
     data for a single user will be split
 
     Args:
         skip_user_error:
-            If set to True, users for which data can't be split will be skipped and only a warning will be logged when
-            calling the `split_all()` method. Otherwise, a `ValueError` exception is raised
+            If set to True, users for which data can't be split will be skipped and only a warning will be logged at the
+            end of the split process specifying n° of users skipped. Otherwise, a `ValueError` exception is raised
     """
 
     def __init__(self, skip_user_error: bool = True):
         self.__skip_user_error = skip_user_error
 
     @property
     def skip_user_error(self):
         return self.__skip_user_error
 
     @abc.abstractmethod
     def __str__(self):
         raise NotImplementedError
 
     @abc.abstractmethod
-    def split_single(self, user_ratings: List[Interaction]) -> Tuple[List[List[Interaction]], List[List[Interaction]]]:
+    def split_single(self, uir_user: np.ndarray) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
         Abstract method in which each partitioning technique must specify how to split data for a single user
 
         Args:
-            user_ratings: List of `Interaction` objects of a single user
+            uir_user: uir matrix containing interactions of a single user
 
         Returns:
-            Two lists, where the first contains one list of `Interaction` objects for each split that will
-                constitute the *train set* of the user, the second contains one list of `Interaction` objects for each split
-                that will constitute the *test set* for the user
+            The first list contains a uir matrix for each split constituting the *train set* of the user
+
+            The second list contains a uir matrix for each split constituting the *test set* of the user
         """
         raise NotImplementedError
 
-    def split_all(self, ratings_to_split: Ratings, user_id_list: Set[str] = None) -> Tuple[List[Ratings],
-                                                                                           List[Ratings]]:
+    def split_all(self, ratings_to_split: Ratings,
+                  user_list: Union[Set[int], Set[str]] = None) -> Tuple[List[Ratings], List[Ratings]]:
         """
-        Concrete method that splits, for every user in the `ratings_to_split` parameter, the original ratings
+        Concrete method that splits, for every user in the user column of `ratings_to_split`, the original ratings
         into *train set* and *test set*.
-        If a `user_id_list` parameter is set, the method will do the splitting only for the users
-        specified inside the list.
+        If a `user_list` parameter is set, the method will do the splitting only for the users
+        specified inside the list (Users can be specified as *strings* or with their mapped *integer*).
 
         The method returns two lists:
 
         * The first contains all train set for each split (if the partitioning technique returns more than one split
         e.g. KFold)
         * The second contains all test set for each split (if the partitioning technique returns more than one split
         e.g. KFold)
 
         Obviously the two lists will have the same length, and to the *train set* in position $i$ corresponds the
         *truth set* at position $i$
 
         Args:
-            ratings_to_split: `Ratings` object which contains the interactions of the users that must be splitted
+            ratings_to_split: `Ratings` object which contains the interactions of the users that must be split
                 into *train set* and *test set*
-            user_id_list: The set of users for which splitting will be done. If set, splitting will be performed only
+            user_list: The Set of users for which splitting will be done. If set, splitting will be performed only
                 for users inside the list. Otherwise, splitting will be performed for all users in `ratings_to_split`
-                parameter
+                parameter. User can be specified with their string id or with their mapped integer
 
         Raises:
-            ValueError: if `skip_user_error=True` in the constructor and for some users splitting can't be performed
+            ValueError: if `skip_user_error=True` in the constructor and for at least one user splitting
+                can't be performed
         """
 
-        if user_id_list is None:
-            user_id_list = set(ratings_to_split.user_id_column)
+        # convert user list to list of int if necessary (strings are passed)
+        if user_list is not None:
+            all_users = np.array(list(user_list))
+            if np.issubdtype(all_users.dtype, str):
+                all_users = ratings_to_split.user_map.convert_seq_str2int(all_users)
+
+            all_users = set(all_users)
+        else:
+            all_users = set(ratings_to_split.unique_user_idx_column)
 
         # {
-        #   0: {'train': {'u1': u1_interactions_train0, 'u2': u2_interactions_train0}},
-        #       'test': {'u1': u1_interactions_test0, 'u2': u2_interactions_test0}},
+        #   0: {'train': [u1_uir, u2_uir]},
+        #       'test': [u1_uir, u2_uir]},
         #
-        #   1: {'train': {'u1': u1_interactions_train1, 'u2': u2_interactions_train1}},
-        #       'test': {'u1': u1_interactions_test1, 'u2': u2_interactions_test1}
+        #   1: {'train': [u1_uir, u2_uir]},
+        #       'test': [u1_uir, u2_uir]
         #  }
         train_test_dict = defaultdict(lambda: defaultdict(list))
+        error_count = 0
 
-        with get_progbar(user_id_list) as pbar:
+        with get_progbar(all_users) as pbar:
 
             pbar.set_description("Performing {}".format(str(self)))
-            for user_id in pbar:
-                user_ratings = ratings_to_split.get_user_interactions(user_id)
+            for user_idx in pbar:
+                user_ratings = ratings_to_split.get_user_interactions(user_idx)
                 try:
                     user_train_list, user_test_list = self.split_single(user_ratings)
                     for split_number, (single_train, single_test) in enumerate(zip(user_train_list, user_test_list)):
-                        # we set for each split the train_set and test_set of every user u1
-                        # eg.
-                        #     train_test_dict[0]['train']['u1'] = u1_interactions_train0
-                        #     train_test_dict[0]['test']['u1'] = u1_interactions_test0
-                        # train_test_dict[split_number]['train'][user_id] = single_train
-                        # train_test_dict[split_number]['test'][user_id] = single_test
-                        train_test_dict[split_number]['train'].extend(single_train)
-                        train_test_dict[split_number]['test'].extend(single_test)
+
+                        train_test_dict[split_number]['train'].append(single_train)
+                        train_test_dict[split_number]['test'].append(single_test)
 
                 except ValueError as e:
                     if self.skip_user_error:
-                        logger.warning(str(e) + "\nThe user {} will be skipped".format(user_id))
+                        error_count += 1
                         continue
                     else:
-                        raise e
+                        raise e from None
 
-        train_list = [Ratings.from_list(train_test_dict[split]['train'])
+        if error_count > 0:
+            logger.warning(f"{error_count} users will be skipped because partitioning couldn't be performed\n"
+                           f"Change this behavior by setting `skip_user_error` to True")
+
+        train_list = [Ratings.from_uir(np.vstack(train_test_dict[split]['train']),
+                                       ratings_to_split.user_map, ratings_to_split.item_map)
                       for split in train_test_dict]
 
-        test_list = [Ratings.from_list(train_test_dict[split]['test'])
+        test_list = [Ratings.from_uir(np.vstack(train_test_dict[split]['test']),
+                                      ratings_to_split.user_map, ratings_to_split.item_map)
                      for split in train_test_dict]
 
         return train_list, test_list
 
 
 class KFoldPartitioning(Partitioning):
     """
@@ -139,45 +146,45 @@
             Note that the samples within each split will not be shuffled.
         random_state:
             When `shuffle` is True, `random_state` affects the ordering of the
             indices, which controls the randomness of each fold. Otherwise, this
             parameter has no effect.
             Pass an int for reproducible output across multiple function calls.
         skip_user_error:
-            If set to True, users for which data can't be split will be skipped and only a warning will be logged when
-            calling the `split_all()` method. Otherwise, a `ValueError` exception is raised
+            If set to True, users for which data can't be split will be skipped and only a warning will be logged at the
+            end of the split process specifying n° of users skipped. Otherwise, a `ValueError` exception is raised
     """
 
     def __init__(self, n_splits: int = 2, shuffle: bool = True, random_state: int = None,
                  skip_user_error: bool = True):
         self.__kf = KFold(n_splits=n_splits, shuffle=shuffle, random_state=random_state)
 
         super(KFoldPartitioning, self).__init__(skip_user_error)
 
-    def split_single(self, user_ratings: List[Interaction]) -> Tuple[List[List[Interaction]], List[List[Interaction]]]:
+    def split_single(self, uir_user: np.ndarray) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
         Method which splits in $k$ splits both in *train set* and *test set* the ratings of a single user
 
         Args:
-            user_ratings: List of `Interaction` objects of a single user
+            uir_user: uir matrix containing interactions of a single user
 
         Returns:
-            Two lists, where the first contains one list of `Interaction` objects for each split that will
-                constitute the *train set* of the user, the second contains one list of `Interaction` objects for each split
-                that will constitute the *test set* for the user
+            The first list contains a uir matrix for each split constituting the *train set* of the user
+
+            The second list contains a uir matrix for each split constituting the *test set* of the user
         """
-        split_result = self.__kf.split(user_ratings)
+        split_result = self.__kf.split(uir_user)
 
         user_train_list = []
         user_test_list = []
+
         # split_result contains index of the ratings which must constitutes train set and test set
         for train_set_indexes, test_set_indexes in split_result:
-            user_interactions_train = [user_ratings[index] for index in train_set_indexes]
-
-            user_interactions_test = [user_ratings[index] for index in test_set_indexes]
+            user_interactions_train = uir_user[train_set_indexes]
+            user_interactions_test = uir_user[test_set_indexes]
 
             user_train_list.append(user_interactions_train)
             user_test_list.append(user_interactions_test)
 
         return user_train_list, user_test_list
 
     def __str__(self):
@@ -190,121 +197,144 @@
 
 class HoldOutPartitioning(Partitioning):
     """
     Class that performs Hold-Out partitioning
 
     Args:
         train_set_size: Should be between 0.0 and 1.0 and represent the proportion of the ratings to
-            ***hold*** in the train set for each user.
+            ***hold*** in the train set for each user. If
+            int, represents the absolute number of train samples. If None,
+            the value is automatically set to the complement of the test size.
+        test_set_size: If float, should be between 0.0 and 1.0 and represent the proportion
+            of the dataset to include in the test split. If int, represents the
+            absolute number of test samples. If None, the value is set to the
+            complement of the train size. If `train_size` is also None, it will
+            be set to 0.25.
         random_state:
             Controls the shuffling applied to the data before applying the split.
             Pass an int for reproducible output across multiple function calls.
         shuffle:
-            Whether or not to shuffle the data before splitting.
+            Whether to shuffle the data before splitting.
         skip_user_error:
-            If set to True, users for which data can't be split will be skipped and only a warning will be logged when
-            calling the `split_all()` method. Otherwise, a `ValueError` exception is raised
+            If set to True, users for which data can't be split will be skipped and only a warning will be logged at the
+            end of the split process specifying n° of users skipped. Otherwise, a `ValueError` exception is raised
     """
 
-    def __init__(self, train_set_size: float = 0.8, shuffle: bool = True, random_state: int = None,
+    def __init__(self, train_set_size: Union[float, int, None] = None, test_set_size: Union[float, int, None] = None,
+                 shuffle: bool = True, random_state: int = None,
                  skip_user_error: bool = True):
-        self._check_percentage(train_set_size)
+
+        if train_set_size is not None and train_set_size < 0:
+            raise ValueError("train_set_size must be a positive number")
+
+        if test_set_size is not None and test_set_size < 0:
+            raise ValueError("test_set_size must be a positive number")
+
+        if isinstance(train_set_size, float) and train_set_size > 1.0:
+            raise ValueError("train_set_size must be between 0.0 and 1.0")
+
+        if isinstance(test_set_size, float) and test_set_size > 1.0:
+            raise ValueError("test_set_size must be between 0.0 and 1.0")
+
+        if isinstance(train_set_size, float) and isinstance(test_set_size, float) and \
+                (train_set_size + test_set_size) > 1.0:
+            raise ValueError("train_set_size and test_set_size percentages must not sum to a value greater than 1.0")
+
         self.__train_set_size = train_set_size
-        self.__test_set_size = (1 - train_set_size)
+        self.__test_set_size = test_set_size
         self.__random_state = random_state
         self.__shuffle = shuffle
 
         super().__init__(skip_user_error)
 
-    @staticmethod
-    def _check_percentage(percentage: float):
-        if (percentage <= 0) or (percentage >= 1):
-            raise ValueError("The train set size must be a float in the (0, 1) interval")
-
-    def split_single(self, user_ratings: List[Interaction]) -> Tuple[List[List[Interaction]], List[List[Interaction]]]:
+    def split_single(self, uir_user: np.ndarray) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
-        Method which splits *train set* and *test set* the ratings of a single user by holding in the train
-        set the percentage of data specified in `train_set_size` in the constructor
+        Method which splits *train set* and *test set* the ratings of a single user by holding in the train set of the
+        user interactions accoring to the parameters set in the constructor
 
         Args:
-            user_ratings: List of `Interaction` objects of a single user
+            uir_user: uir matrix containing interactions of a single user
 
         Returns:
-            Two lists, where the first contains one list of `Interaction` objects that will
-                constitute the *train set* of the user, the second contains one list of `Interaction` objects
-                that will constitute the *test set* for the user
+            The first list contains a uir matrix for each split constituting the *train set* of the user
+
+            The second list contains a uir matrix for each split constituting the *test set* of the user
         """
-        interactions_train, interactions_test = train_test_split(user_ratings,
-                                                                 train_size=self.__train_set_size,
-                                                                 test_size=self.__test_set_size,
-                                                                 shuffle=self.__shuffle,
-                                                                 random_state=self.__random_state)
+        uir_train, uir_test = train_test_split(uir_user,
+                                               train_size=self.__train_set_size,
+                                               test_size=self.__test_set_size,
+                                               shuffle=self.__shuffle,
+                                               random_state=self.__random_state)
 
-        user_train_list = [interactions_train]
-        user_test_list = [interactions_test]
+        user_train_list = [uir_train]
+        user_test_list = [uir_test]
 
         return user_train_list, user_test_list
 
     def __str__(self):
         return "HoldOutPartitioning"
 
     def __repr__(self):
-        return f"HoldOutPartitioning(train_set_size={self.__train_set_size}, shuffle={self.__shuffle}, " \
-               f"random_state={self.__random_state}, skip_user_error={self.skip_user_error})"
+        return f"HoldOutPartitioning(train_set_size={self.__train_set_size}, test_set_size={self.__test_set_size}, " \
+               f"shuffle={self.__shuffle}, random_state={self.__random_state}, skip_user_error={self.skip_user_error})"
 
 
 class BootstrapPartitioning(Partitioning):
     """
     Class that performs Bootstrap Partitioning.
 
     The bootstrap partitioning consists in executing $n$ extractions with replacement for each user from the original
     interaction frame, where $n$ is the length of the user interactions:
 
-        * The sampled data will be part of the ***train set***
-        * All the data which is part of the original dataset but was not sampled will be part of the ***test set***
+    * The sampled data will be part of the ***train set***
+    * All the data which is part of the original dataset but was not sampled will be part of the ***test set***
 
-    The bootstrap partitioning can **change** the original data distribution, since during the extraction phase you
-    could sample the same data more than once
+    !!! info
+
+        The bootstrap partitioning can **change** the original data distribution, since during the extraction phase you
+        could sample the same data more than once
 
     Args:
         random_state:
             Controls the shuffling applied to the data before applying the split.
             Pass an int for reproducible output across multiple function calls.
         skip_user_error:
-            If set to True, users for which data can't be split will be skipped and only a warning will be logged when
-            calling the `split_all()` method. Otherwise, a `ValueError` exception is raised
+            If set to True, users for which data can't be split will be skipped and only a warning will be logged at the
+            end of the split process specifying n° of users skipped. Otherwise, a `ValueError` exception is raised
     """
 
     def __init__(self, random_state: int = None, skip_user_error: bool = True):
         super().__init__(skip_user_error)
 
         self.__random_state = random_state
 
-    def split_single(self, user_ratings: List[Interaction]) -> Tuple[List[List[Interaction]], List[List[Interaction]]]:
+    def split_single(self, uir_user: np.ndarray) -> Tuple[List[np.ndarray], List[np.ndarray]]:
         """
         Method which splits *train set* and *test set* the ratings of a single user by performing $n$ extraction with
         replacement of the user interactions, where $n$ is the number of its interactions.
         The interactions which are not sampled will be part of the *test set*
 
         Args:
-            user_ratings: List of `Interaction` objects of a single user
+            uir_user: uir matrix containing interactions of a single user
 
         Returns:
-            Two lists, where the first contains one list of `Interaction` objects that will
-                constitute the *train set* of the user, the second contains one list of `Interaction` objects
-                that will constitute the *test set* for the user
+            The first list contains a uir matrix for each split constituting the *train set* of the user
+
+            The second list contains a uir matrix for each split constituting the *test set* of the user
         """
 
-        interactions_train = resample(user_ratings,
+        interactions_train = resample(uir_user,
                                       replace=True,
-                                      n_samples=len(user_ratings),
+                                      n_samples=len(uir_user[:, 0]),
                                       random_state=self.__random_state)
 
-        interactions_test = [interaction for interaction in user_ratings
-                             if interaction not in interactions_train]
+        interactions_test = np.array([interaction
+                                      for interaction in uir_user
+                                      if not any(np.array_equal(interaction, interaction_train, equal_nan=True)
+                                                 for interaction_train in interactions_train)])
 
         user_train_list = [interactions_train]
         user_test_list = [interactions_test]
 
         if len(interactions_test) == 0:
             raise ValueError("The test set for the user is empty! Try increasing the number of its interactions!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `clayrs-0.4.1/clayrs/recsys/recsys.py` & `clayrs-0.5.1/clayrs/recsys/content_based_algorithm/content_based_algorithm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,739 +1,893 @@
 from __future__ import annotations
 import abc
 import gc
-import itertools
 from copy import deepcopy
-from typing import Union, Dict, List, Optional, TYPE_CHECKING
+from itertools import chain
+from typing import List, TYPE_CHECKING, Optional, Any, Set, Tuple, Dict, Callable
 
-from abc import ABC
+from scipy import sparse
+from sklearn.exceptions import NotFittedError
+from sklearn.feature_extraction import DictVectorizer
+from sklearn.utils.validation import check_is_fitted
+import numpy as np
+import torch
 
-if TYPE_CHECKING:
-    from clayrs.content_analyzer import Ratings
-    from clayrs.recsys.graphs.graph import FullDiGraph
-    from clayrs.recsys.content_based_algorithm.content_based_algorithm import ContentBasedAlgorithm
-    from clayrs.recsys.graph_based_algorithm.graph_based_algorithm import GraphBasedAlgorithm
-    from clayrs.recsys.methodology import Methodology
-
-from clayrs.content_analyzer.ratings_manager.ratings import Rank, Prediction
-from clayrs.recsys.methodology import TestRatingsMethodology
-from clayrs.recsys.content_based_algorithm.exceptions import UserSkipAlgFit, NotFittedAlg
+from clayrs.recsys.content_based_algorithm.exceptions import UserSkipAlgFit
+from clayrs.recsys.methodology import Methodology
 from clayrs.utils.const import logger
 from clayrs.utils.context_managers import get_iterator_parallel
 
+if TYPE_CHECKING:
+    from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.combining_technique import \
+        CombiningTechnique
+    from clayrs.content_analyzer.ratings_manager.ratings import Ratings
+    from clayrs.content_analyzer.content_representation.content import Content
 
-class RecSys(ABC):
-    """
-    Abstract class for a Recommender System
-
-    There exists various type of recommender systems, content-based, graph-based, etc. so extend this class
-    if another type must be implemented into the framework.
+from clayrs.recsys.algorithm import Algorithm
+from clayrs.recsys.content_based_algorithm.contents_loader import LoadedContentsDict
 
-    Every recommender system has an algorithm which is used to compute rank/score predictions
 
-    Args:
-        algorithm: The algorithm used to compute rank/score prediction
+class ContentBasedAlgorithm(Algorithm):
     """
+    Abstract class for the content-based algorithms
 
-    def __init__(self, algorithm: Union[ContentBasedAlgorithm, GraphBasedAlgorithm]):
-        self.__alg = algorithm
-
-        self._yaml_report: Optional[Dict] = None
-
-    @property
-    def algorithm(self):
-        return self.__alg
-
-    @abc.abstractmethod
-    def rank(self, test_set: Ratings, n_recs: int = 10) -> Rank:
-        raise NotImplementedError
-
-    @abc.abstractmethod
-    def predict(self, test_set: Ratings) -> Prediction:
-        raise NotImplementedError
-
+    Every Content Based Algorithm base its prediction (let it be score prediction or ranking) on representations
+    serialized by the Content Analyzer. It can be used a single representation or multiple ones for a single field or
+    multiple ones
 
-class ContentBasedRS(RecSys):
+    Args:
+    item_field (dict): dict where the key is the name of the field
+        that contains the content to use, value is the representation(s) id(s) that will be
+        used for the said item. The value of a field can be a string/int or a list,
+        use a list if you want to use multiple representations for a particular field.
+    threshold (float): Threshold for the ratings. Some algorithms use this threshold in order to
+        separate positive items from the negative ones, others may use only ratings that are >= than this
+        threshold. See the documentation of the algorithm used for more
     """
-    Class for recommender systems which use the items' content in order to make predictions,
-    some algorithms may also use users' content, so it's an optional parameter.
-
-    Every CBRS differ from each other based the algorithm used.
+    __slots__ = ('item_field', 'threshold', '_transformer')
 
-    Examples:
+    def __init__(self, item_field: dict, threshold: float):
+        self.item_field: dict = self._bracket_representation(item_field)
+        self.threshold: float = threshold
+        self._transformer = DictVectorizer(sparse=False, sort=False)
 
-        In case you perform a splitting of the dataset which returns a single train and test set (e.g. HoldOut
-        technique):
+    @staticmethod
+    def _bracket_representation(item_field: dict):
+        """
+        Private method that brackets every representation in case the user passed a string
+        instead of a list.
 
-        ```python title="Single split train"
-        from clayrs import recsys as rs
-        from clayrs import content_analyzer as ca
+        Examples:
 
-        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
+            >>> item_field = {'Plot': 0, 'Genre': ['tfidf', 1]}
+            >>> print(ContentBasedAlgorithm._bracket_representation(item_field))
+            {'Plot': [0], 'Genre': ['tfidf', 1]}
 
-        [train], [test] = rs.HoldOutPartitioning().split_all(original_rat)
+        Args:
+            item_field: dict that contain values that may need to be bracketed
 
-        alg = rs.CentroidVector()  # any cb algorithm
+        Returns:
+            The item_field passed with all values inside a list
+        """
+        for field in item_field:
+            if not isinstance(item_field[field], list):
+                item_field[field] = [item_field[field]]
 
-        cbrs = rs.ContentBasedRS(alg, train, items_path)
+        return item_field
 
-        rank = cbrs.fit_rank(test, n_recs=10)
-        ```
+    def extract_features_item(self, item: Content):
+        """
+        Function that extracts the feature of a loaded item using the item_field parameter passed in the
+        constructor.
 
-        In case you perform a splitting of the dataset which returns a multiple train and test sets (KFold technique):
+        It extracts only the chosen representations of the chosen fields in the item loaded
 
-        ```python title="Multiple split train"
-        from clayrs import recsys as rs
-        from clayrs import content_analyzer as ca
+        * with `item_field = {'Plot': [0], 'Genre': ['tfidf', 1]}`, the function will extract
+        only the representation with `0` as internal id for the field `Plot` and two representations
+        for the field `Genre`: one with `tfidf` as *external id* and the other with `1` as *internal id*
 
-        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
+        Args:
+            item: item loaded of which we need to extract its feature
 
-        train_list, test_list = rs.KFoldPartitioning(n_splits=5).split_all(original_rat)
+        Returns:
+            A list containing all representations extracted for the item
+        """
+        item_bag_list = []
+        if item is not None:
+            for field in self.item_field:
+                field_representations = self.item_field[field]
+
+                for representation in field_representations:
+                    item_bag_list.append(
+                        item.get_field_representation(field, representation).value
+                    )
+
+        return item_bag_list
+
+    def fuse_representations(self, X: list, embedding_combiner: CombiningTechnique, as_array: bool = False):
+        """
+        Method which transforms the X passed vectorizing if X contains dicts and merging
+        multiple representations in a single one for every item in X.
+        So if X = [
+                    [dict, np.array, np.array]
+                        ...
+                    [dict, np.array, np.array]
+                ]
+        where every sublist contains multiple representation for a single item,
+        the function returns:
+        X = [
+                np.array,
+                ...
+                np.array
+            ]
+        Where every row is the fused representation for the item
+
+        In case np.array have different row size, every array will be transformed in a one dimensional one
+        using the parameter embedding combiner. Check all the available combining technique to know how rows of
+        a np.array can be merged into one
 
-        alg = rs.CentroidVector()  # any cb algorithm
+        Args:
+            X: list that contains representations of the items
+            embedding_combiner: combining technique in case there are multiple
+                vectors with different row size
+            as_array: if True, result will always be a np.array regardless of the input (e.g. if input are scipy sparse
+                matrices, output is a scipy sparse matrix)
+        Returns:
+            X fused and vectorized
+        """
+        if any(not isinstance(rep, (dict, np.ndarray, (int, float), sparse.csc_matrix, torch.Tensor)) for rep in X[0]):
+            raise ValueError("You can only use representations of type: {numeric, embedding, tfidf}")
 
-        for train_set, test_set in zip(train_list, test_list):
+        # We check if there are dicts as representation in the first element of X,
+        # since the representations are the same for all elements in X we can check
+        # for dicts only in one element
+        need_vectorizer = any(isinstance(rep, dict) for rep in X[0])
 
-            cbrs = rs.ContentBasedRS(alg, train_set, items_path)
-            rank_to_append = cbrs.fit_rank(test_set)
+        if need_vectorizer:
+            # IF the transformer is not fitted then we are training the model
+            try:
+                check_is_fitted(self._transformer)
+            except NotFittedError:
+                X_dicts = [rep for item in X for rep in item if isinstance(rep, dict)]
+                self._transformer.fit(X_dicts)
+
+        # In every case, we transform the input
+        def single_item_fused_gen():
+            for item_repr_list in X:
+                single_arr = []
+                for item_repr in item_repr_list:
+                    if need_vectorizer and isinstance(item_repr, dict):
+                        item_repr = self._transformer.transform(item_repr).squeeze()
+
+                    elif isinstance(item_repr, np.ndarray):
+                        item_repr = item_repr.squeeze()
+                        if item_repr.ndim > 1:
+                            item_repr = embedding_combiner.combine(item_repr).squeeze()
+
+                    elif isinstance(item_repr, torch.Tensor):
+                        item_repr = item_repr.numpy().squeeze()
+
+                        if item_repr.ndim > 1:
+                            item_repr = embedding_combiner.combine(item_repr).squeeze()
+
+                    single_arr.append(item_repr)
+
+                yield single_arr
+
+        # if a representation used is a sparse matrix, then we use scipy library to concatenate
+        # otherwise, if we have all dense arrays, we use numpy. To do this check we consider the representations
+        # of the first item
+        first_arr = next(single_item_fused_gen())
+        if any(isinstance(x, sparse.csc_matrix) for x in first_arr):
+            X_vectorized = (sparse.hstack(single_arr) for single_arr in single_item_fused_gen())
+
+            X_vectorized = sparse.vstack(X_vectorized, format='csr')
+
+            if as_array is True:
+                X_vectorized = X_vectorized.toarray()
+        else:
+            X_vectorized = [np.hstack(single_arr) for single_arr in single_item_fused_gen()]
 
-            result_list.append(rank_to_append)
-        ```
+            X_vectorized = np.array(X_vectorized)
 
-        `result_list` will contain recommendation lists for each split
+        return X_vectorized
 
-    Args:
-        algorithm: the content based algorithm that will be used in order to
-            rank or make score prediction
-        train_set: a Ratings object containing interactions between users and items
-        items_directory: the path of the items serialized by the Content Analyzer
-        users_directory: the path of the users serialized by the Content Analyzer
-    """
+    @abc.abstractmethod
+    def fit(self, train_set: Ratings, items_directory: str, num_cpus: int = 0) -> Any:
+        """
+        Abstract method that fits the content-based algorithm.
 
-    def __init__(self,
-                 algorithm: ContentBasedAlgorithm,
-                 train_set: Ratings,
-                 items_directory: str,
-                 users_directory: str = None):
+        Every content based algorithm has a different fit process, it may be needed to fit a classifier for each user,
+        to build the centroid of the positive items of each user, to train a neural network for the entire system, etc.
 
-        super().__init__(algorithm)
-        self.__train_set = train_set
-        self.__items_directory = items_directory
-        self.__users_directory = users_directory
-        self._user_fit_dic = {}
+        Args:
+            train_set: Ratings object containing interactions between users and items
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            num_cpus: number of processors that must be reserved for the method
 
-    @property
-    def algorithm(self):
         """
-        The content based algorithm chosen
-        """
-        alg: ContentBasedAlgorithm = super().algorithm
-        return alg
+        raise NotImplementedError
 
-    @property
-    def train_set(self):
-        """
-        The train set of the Content Based RecSys
+    @abc.abstractmethod
+    def rank(self, fit_alg: Any, train_set: Ratings, test_set: Ratings, items_directory: str,
+             user_idx_list: Set[int], n_recs: Optional[int], methodology: Methodology,
+             num_cpus: int) -> List[np.ndarray]:
         """
-        return self.__train_set
+        Abstract method for ranking the top-n recommended items for the user.
+        If the recs_number parameter isn't specified, all ranked items will be returned
 
-    @property
-    def items_directory(self):
-        """
-        Path of the serialized items by the Content Analyzer
-        """
-        return self.__items_directory
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
 
-    @property
-    def users_directory(self):
-        """
-        Path of the serialized users by the Content Analyzer
-        """
-        return self.__users_directory
+        Remember that `user_idx_list` should contain user id mapped to their integer! Not their string representation!
 
-    def fit(self, num_cpus: int = 0):
-        """
-        Method which will fit the algorithm chosen for each user in the train set passed in the constructor
+        Args:
+            fit_alg: Result object returned by the `fit()` function of `self` (the chosen algorithm)
+            train_set: Ratings object containing interactions between users and items
+            test_set: Ratings object which represents the ground truth of the split considered
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user.
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`
+            num_cpus: number of processors that must be reserved for the method
 
-        If the algorithm can't be fit for some users, a warning message is printed
+        Returns:
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items sorted in a descending way w.r.t. the third dimension which is the ranked score
         """
-        def compute_single_fit(user_id):
-            user_train = self.train_set.get_user_interactions(user_id)
-            user_alg = deepcopy(self.algorithm)
+        raise NotImplementedError
 
-            try:
-                user_alg.process_rated(user_train, loaded_items_interface)
-                user_alg.fit()
-            except UserSkipAlgFit as e:
-                warning_message = str(e) + f"\nNo algorithm will be fitted for the user {user_id}"
-                logger.warning(warning_message)
-                user_alg = None
-
-            return user_id, user_alg
-
-        items_to_load = set(self.train_set.item_id_column)
-        all_users = set(self.train_set.user_id_column)
-        loaded_items_interface = self.algorithm._load_available_contents(self.items_directory, items_to_load)
+    @abc.abstractmethod
+    def predict(self, fit_alg: Any, train_set: Ratings, test_set: Ratings, items_directory: str,
+                user_idx_list: Set[int], methodology: Methodology,
+                num_cpus: int) -> List[np.ndarray]:
+        """
+        Abstract method that predicts the rating which a user would give to items
+        If the algorithm is not a PredictionScore Algorithm, implement this method like this:
+
+        ```python
+        def predict():
+            raise NotPredictionAlg
+        ```
 
-        with get_iterator_parallel(num_cpus,
-                                   compute_single_fit, all_users,
-                                   progress_bar=True, total=len(all_users)) as pbar:
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
 
-            pbar.set_description("Fitting algorithm")
+        Remember that `user_idx_list` should contain user id mapped to their integer! Not their string representation!
+
+        Args:
+            fit_alg: Result object returned by the `fit()` function of `self` (the chosen algorithm)
+            train_set: Ratings object containing interactions between users and items
+            test_set: Ratings object which represents the ground truth of the split considered
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`
+            num_cpus: number of processors that must be reserved for the method
 
-            for user_id, fitted_user_alg in pbar:
-                self._user_fit_dic[user_id] = fitted_user_alg
+        Returns:
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items
+        """
+        raise NotImplementedError
 
-        # we force the garbage collector after freeing loaded items
-        del loaded_items_interface
-        gc.collect()
+    @abc.abstractmethod
+    def fit_rank(self, train_set: Ratings, test_set: Ratings, items_directory: str, user_idx_list: Set[int],
+                 n_recs: Optional[int], methodology: Methodology, num_cpus: int,
+                 save_fit: bool) -> Tuple[Optional[Any], List[np.ndarray]]:
+        """
+        Method used to both fit and calculate ranking for all users in `user_idx_list` parameter.
+        The algorithm will first be fit for each user in the `user_idx_list` which should contain user id
+        mapped to their integer!
+
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
+
+        With the `save_fit` parameter you can specify if you need the function to return the algorithm fit (in case
+        you want to perform multiple calls to the `predict()` or `rank()` function). If set to True, the first value
+        returned by this function will be the fit algorithm and the second will be the list of uir matrices with
+        predictions for each user.
+        Otherwise, if `save_fit` is False, the first value returned by this function will be `None`
 
-        return self
+        Args:
+            train_set: Ratings object containing interactions between users and items
+            test_set: Ratings object which represents the ground truth of the split considered
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user.
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`
+            num_cpus: number of processors that must be reserved for the method
+            save_fit: Boolean value which let you choose if the fit algorithm should be saved and returned by this
+                function. If True, the first value returned by this function is the fit algorithm. Otherwise, the first
+                value will be None. The second value is always the list of predicted uir matrices
 
-    def rank(self, test_set: Ratings, n_recs: int = 10, user_id_list: List = None,
-             methodology: Union[Methodology, None] = TestRatingsMethodology(),
-             num_cpus: int = 1) -> Rank:
+        Returns:
+            The first value is the fit VBPR algorithm (could be None if `save_fit == False`)
 
+            The second value is a list of predicted uir matrices all sorted in a decreasing order w.r.t.
+                the ranking scores
         """
-        Method used to calculate ranking for all users in test set or all users in `user_id_list` parameter.
-        You must first call the `fit()` method before you can compute the ranking.
+        raise NotImplementedError
 
-        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
-        Otherwise, the rank will contain all unrated items of the particular users
+    @abc.abstractmethod
+    def fit_predict(self, train_set: Ratings, test_set: Ratings, items_directory: str, user_idx_list: Set[int],
+                    methodology: Methodology, num_cpus: int,
+                    save_fit: bool) -> Tuple[Optional[Any], List[np.ndarray]]:
+        """
+        Method used to both fit and calculate score prediction for all users in `user_idx_list` parameter.
+        The algorithm will first be fit for each user in the `user_idx_list` which should contain user id
+        mapped to their integer!
+
+        If the algorithm is not a PredictionScore Algorithm, implement this method like this:
+
+        ```python
+        def fit_predict():
+            raise NotPredictionAlg()
+        ```
 
-        Via the `methodology` parameter you can perform different candidate item selection. By default, the
-        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
 
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
+        With the `save_fit` parameter you can specify if you need the function to return the algorithm fit (in case
+        you want to perform multiple calls to the `predict()` or `rank()` function). If set to True, the first value
+        returned by this function will be the fit algorithm and the second will be the list of uir matrices with
+        predictions for each user.
+        Otherwise, if `save_fit` is False, the first value returned by this function will be `None`
 
         Args:
+            train_set: Ratings object containing interactions between users and items
             test_set: Ratings object which represents the ground truth of the split considered
-            n_recs: Number of the top items that will be present in the ranking of each user.
-                If `None` all candidate items will be returned for the user
-            user_id_list: List of users for which you want to compute the ranking. If None, the ranking will be computed
-                for all users of the `test_set`
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
             methodology: `Methodology` object which governs the candidate item selection. Default is
                 `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
-
-        Raises:
-            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
+            num_cpus: number of processors that must be reserved for the method
+            save_fit: Boolean value which let you choose if the fit algorithm should be saved and returned by this
+                function. If True, the first value returned by this function is the fit algorithm. Otherwise, the first
+                value will be None. The second value is always the list of predicted uir matrices
 
         Returns:
-            Rank object containing recommendation lists for all users of the test set or for all users in `user_id_list`
+            The first value is the fit algorithm (could be None if `save_fit == False`)
 
+            The second value is a list of predicted uir matrices
         """
-        def compute_single_rank(user_id):
-            user_id = str(user_id)
-            user_train = self.train_set.get_user_interactions(user_id)
+        raise NotImplementedError
 
-            filter_list = None
-            if methodology is not None:
-                filter_list = set(methodology.filter_single(user_id, self.train_set, test_set))
+    def _load_available_contents(self, contents_path: str, items_to_load: set = None):
+        return LoadedContentsDict(contents_path, items_to_load, only_representations=self.item_field)
 
-            user_fitted_alg = self._user_fit_dic.get(user_id)
-            if user_fitted_alg is not None:
-                user_rank = user_fitted_alg.rank(user_train, loaded_items_interface,
-                                                 n_recs, filter_list=filter_list)
-            else:
-                user_rank = []
-                logger.warning(f"No algorithm fitted for user {user_id}! It will be skipped")
+    def __deepcopy__(self, memo):
+        # Create a new instance
+        cls = self.__class__
+        result = cls.__new__(cls)
 
-            return user_id, user_rank
+        # Don't copy self reference
+        memo[id(self)] = result
 
-        if len(self._user_fit_dic) == 0:
-            raise NotFittedAlg("Algorithm not fit! You must call the fit() method first, or fit_rank().")
+        # Don't copy the cache - if it exists
+        if hasattr(self, "_cache"):
+            memo[id(self._cache)] = self._cache.__new__(dict)
 
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
+        # Get all __slots__ of the derived class
+        slots = chain.from_iterable(getattr(s, '__slots__', []) for s in self.__class__.__mro__)
 
-        loaded_items_interface = self.algorithm._load_available_contents(self.items_directory, set())
+        # Deep copy all other attributes
+        for var in slots:
+            setattr(result, var, deepcopy(getattr(self, var), memo))
 
-        rank = []
+        # Return updated instance
+        return result
 
-        logger.info("Don't worry if it looks stuck at first")
-        logger.info("First iterations will stabilize the estimated remaining time")
 
-        with get_iterator_parallel(num_cpus,
-                                   compute_single_rank, all_users,
-                                   progress_bar=True, total=len(all_users)) as pbar:
+class PerUserCBAlgorithm(ContentBasedAlgorithm):
+    """
+    Abstract class for any CB algorithm that is fit for each user, rather than being fit for the whole system once
 
-            pbar.set_description(f"Loading first items from memory...")
-            for user_id, user_rank in pbar:
-                pbar.set_description(f"Computing rank for user {user_id}")
-                rank.append(user_rank)
+    Think of the `CentroidVector` algorithm: it builds a centroid for each user!
 
-        rank = itertools.chain.from_iterable(rank)
-        rank = Rank.from_list(rank)
+    This class has several concrete methods so that you can easily extend and add several per-user cb algorithm without
+    implementing many abstract methods!
+    """
+    __slots__ = ()
 
-        # we force the garbage collector after freeing loaded items
-        del loaded_items_interface
-        gc.collect()
+    @abc.abstractmethod
+    def process_rated(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict):
+        """
+        Abstract method that processes rated items for the single user.
 
-        self._yaml_report = {'mode': 'rank', 'n_recs': repr(n_recs), 'methodology': repr(methodology)}
+        Every content-based algorithm processes rated items differently, it may be needed to extract features
+        from the rated items and label them, extract features only from the positive ones, etc.
 
-        return rank
+        The rated items processed must be stored into a private attribute of the algorithm, later used
+        by the fit() method.
 
-    def predict(self, test_set: Ratings, user_id_list: List = None,
-                methodology: Union[Methodology, None] = TestRatingsMethodology(),
-                num_cpus: int = 1) -> Prediction:
+        Args:
+            user_idx: Mapped integer of the active user (the user for which we must fit the algorithm)
+            train_ratings: `Ratings` object which contains the train set of each user
+            available_loaded_items: The LoadedContents interface which contains loaded contents
         """
-        Method used to calculate score predictions for all users in test set or all users in `user_id_list` parameter.
-        You must first call the `fit()` method before you can compute score predictions.
+        raise NotImplementedError
 
-        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
+    @abc.abstractmethod
+    def fit_single_user(self):
+        """
+        Abstract method that fits the content-based algorithm for a single user.
 
-        Via the `methodology` parameter you can perform different candidate item selection. By default, the
-        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be considered for score
-        prediction
+        Every content based algorithm has a different fit process, it may be needed to fit a classifier,
+        to build the centroid of the positive items of the user, etc.
+
+        It must be called after the process_rated() method since it uses private attributes calculated
+        by said method to fit the algorithm.
+        """
+        raise NotImplementedError
 
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
+    @abc.abstractmethod
+    def predict_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                            filter_list: List[str]) -> np.ndarray:
+        """
+        Predicts how much a user will like unrated items.
 
-        Args:
-            test_set: Ratings object which represents the ground truth of the split considered
-            user_id_list: List of users for which you want to compute score prediction. If None, the ranking
-                will be computed for all users of the `test_set`
-            methodology: `Methodology` object which governs the candidate item selection. Default is
-                `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object, and
+        is a list of items represented with their string ids. Must be necessarily strings and not their mapped integer
+        since items are serialized following their string representation!
 
-        Raises:
-            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
+        Args:
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
+            available_loaded_items: The LoadedContents interface which contains loaded contents
+            filter_list: list of the items to rank. Should contain string item ids
 
         Returns:
-            Prediction object containing score prediction lists for all users of the test set or for all users in
-                `user_id_list`
+            uir matrix for a single user containing user and item idxs (integer representation) with the predicted score
+                as third dimension
+        """
+        raise NotImplementedError
 
+    @abc.abstractmethod
+    def rank_single_user(self, user_idx: int, train_ratings: Ratings, available_loaded_items: LoadedContentsDict,
+                         recs_number: Optional[int], filter_list: List[str]) -> np.ndarray:
         """
-        def compute_single_predict(user_id):
-            user_id = str(user_id)
-            user_train = self.train_set.get_user_interactions(user_id)
+        Rank the top-n recommended items for the active user, where the top-n items to rank are controlled by the
+        `recs_number` and `filter_list` parameter:
 
-            filter_list = None
-            if methodology is not None:
-                filter_list = set(methodology.filter_single(user_id, self.train_set, test_set))
+        * the former one is self-explanatory, the second is a list of items
+        represented with their string ids. Must be necessarily strings and not their mapped integer since items are
+        serialized following their string representation!
 
-            user_fitted_alg = self._user_fit_dic.get(user_id)
-            if user_fitted_alg is not None:
-                user_pred = user_fitted_alg.predict(user_train, loaded_items_interface, filter_list=filter_list)
-            else:
-                user_pred = []
-                logger.warning(f"No algorithm fitted for user {user_id}! It will be skipped")
+        If `recs_number` is `None`, all ranked items will be returned
+
+        The filter list parameter is usually the result of the `filter_single()` method of a `Methodology` object
 
-            return user_id, user_pred
+        Args:
+            user_idx: Mapped integer of the active user
+            train_ratings: `Ratings` object which contains the train set of each user
+            available_loaded_items: The LoadedContents interface which contains loaded contents
+            recs_number: number of the top ranked items to return, if None all ranked items will be returned
+            filter_list: list of the items to rank. Should contain string item ids
+
+        Returns:
+            uir matrix for a single user containing user and item idxs (integer representation) with the ranked score
+                as third dimension sorted in a decreasing order
+        """
+        raise NotImplementedError
+
+    def fit(self, train_set: Ratings, items_directory: str, num_cpus: int = 1) -> Dict[int, Tuple[Callable, Callable]]:
+        """
+        Method which will fit the algorithm chosen for each user in the `train_set` parameter
 
-        if len(self._user_fit_dic) == 0:
-            raise NotFittedAlg("Algorithm not fit! You must call the fit() method first, or fit_rank().")
+        If the algorithm can't be fit for some users, a warning message is printed showing the number of users
+        for which the alg couldn't be fit
 
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
+        Args:
+            train_set: `Ratings` object which contains the train set of each user
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        loaded_items_interface = self.algorithm._load_available_contents(self.items_directory, set())
+        Returns:
+            A dictionary with users idxs (int representation) are keys and tuples containing (`rank_fn`,
+                `predict_fn`) are values. In this dictionary only users for which the *fit* process could be performed
+                appear!
+        """
+        def compute_single_fit(user_idx):
 
-        pred = []
+            nonlocal count_skipped_user
 
-        logger.info("Don't worry if it looks stuck at first")
-        logger.info("First iterations will stabilize the estimated remaining time")
+            try:
+                self.process_rated(user_idx, train_set, loaded_items_interface)
+                self.fit_single_user()
+                user_fit_fns = (self.rank_single_user, self.predict_single_user)
+            except UserSkipAlgFit as e:
+                # warning_message = str(e) + f"\nNo algorithm will be fit for the user {user_id}"
+                # logger.warning(warning_message)
+                user_fit_fns = None
+                count_skipped_user += 1
+
+            return user_idx, user_fit_fns
+
+        count_skipped_user = 0
+        items_to_load = train_set.unique_item_id_column
+        all_users = train_set.unique_user_idx_column
+        loaded_items_interface = self._load_available_contents(items_directory, items_to_load)
 
+        users_fit_dict = {}
         with get_iterator_parallel(num_cpus,
-                                   compute_single_predict, all_users,
+                                   compute_single_fit, all_users,
                                    progress_bar=True, total=len(all_users)) as pbar:
 
-            pbar.set_description(f"Loading first items from memory...")
-            for user_id, user_pred in pbar:
-                pbar.set_description(f"Computing score prediction for user {user_id}")
-                pred.append(user_pred)
+            pbar.set_description("Fitting algorithm")
 
-        pred = itertools.chain.from_iterable(pred)
-        pred = Prediction.from_list(pred)
+            for user_idx, fitted_user_alg in pbar:
+                if fitted_user_alg is not None:
+                    users_fit_dict[user_idx] = fitted_user_alg
+
+        if count_skipped_user > 0:
+            logger.warning(f"{count_skipped_user} users will be skipped because the algorithm chosen "
+                           f"could not be fit for them")
 
         # we force the garbage collector after freeing loaded items
         del loaded_items_interface
         gc.collect()
 
-        self._yaml_report = {'mode': 'score_prediction', 'methodology': repr(methodology)}
+        return users_fit_dict
 
-        return pred
+    def rank(self, users_fit_dict: dict, train_set: Ratings, test_set: Ratings, items_directory: str,
+             user_idx_list: Set[int], n_recs: Optional[int], methodology: Methodology,
+             num_cpus: int) -> List[np.ndarray]:
+        """
+        Method used to calculate ranking for all users in `user_idx_list` parameter.
+        You must first call the `fit()` method ***before*** you can compute the ranking.
+        The `user_idx_list` parameter should contain users with mapped to their integer!
 
-    def fit_predict(self, test_set: Ratings, user_id_list: List = None,
-                    methodology: Union[Methodology, None] = TestRatingsMethodology(),
-                    save_fit: bool = False, num_cpus: int = 1) -> Prediction:
-        """
-        Method used to both fit and calculate score prediction for all users in test set or all users in `user_id_list`
-        parameter.
-        The Recommender System will first be fit for each user in the train set passed in the constructor.
-        If the algorithm can't be fit for some users, a warning message is printed
+        The representation of the fit per-user cb algorithm is a dictionary where users idxs are keys and
+        a tuples containing `rank_fn` and `predict_fn` are values
 
-        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
+        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
+        Otherwise, the rank will contain all unrated items of the particular users.
 
         Via the `methodology` parameter you can perform different candidate item selection. By default, the
-        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be considered for score
-        prediction
-
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
+        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
 
-        With the `save_fit` parameter you can decide if you want that you recommender system remains *fit* even after
-        the complete execution of this method, in case you want to compute ranking/score prediction with other
-        methodologies, or with a different `n_recs` parameter. Be mindful since it can be memory-expensive,
-        thus by default this behaviour is disabled
+        If the algorithm was not fit for some users, they will be skipped and a warning message is printed showing the
+        number of users for which the alg couldn't produce a ranking
 
         Args:
+            users_fit_dict: dictionary with users idxs (int representation) are keys and tuples containing (`rank_fn`,
+                `predict_fn`) are values. In this dictionary only users for which the *fit* process could be performed
+                appear!
+            train_set: `Ratings` object which contains the train set of each user
             test_set: Ratings object which represents the ground truth of the split considered
-            user_id_list: List of users for which you want to compute score prediction. If None, the ranking
-                will be computed for all users of the `test_set`
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user. Default is 10 (top-10 for each user
+                will be computed)
             methodology: `Methodology` object which governs the candidate item selection. Default is
-                `TestRatingsMethodology`
-            save_fit: Boolean value which let you choose if the Recommender System should remain fit even after the
-                complete execution of this method. Default is False
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
         Returns:
-            Rank object containing recommendation lists for all users of the test set or for all users in `user_id_list`
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items sorted in a descending way w.r.t. the third dimension which is the ranked score
         """
-        def compute_single_fit_predict(user_id):
-            user_train = self.train_set.get_user_interactions(user_id)
 
-            alg = self.algorithm
-            if save_fit:
-                alg = deepcopy(alg)
-                self._user_fit_dic[user_id] = alg
+        def compute_single_rank(user_idx: int):
 
-            try:
-                alg.process_rated(user_train, loaded_items_interface)
-                alg.fit()
-
-            except UserSkipAlgFit as e:
-                warning_message = str(e) + f"\nThe algorithm can't be fitted for the user {user_id}"
-                logger.warning(warning_message)
-                if save_fit:
-                    self._user_fit_dic[user_id] = None
-                return user_id, []
+            nonlocal count_skipped_user
 
-            filter_list = None
-            if methodology is not None:
-                filter_list = set(methodology.filter_single(user_id, self.train_set, test_set))
+            filter_list = methodology.filter_single(user_idx, train_set, test_set).astype(int)
+            # need to convert back int to str to load serialized items
+            filter_list = train_set.item_map.convert_seq_int2str(filter_list)
 
-            user_pred = alg.predict(user_train, loaded_items_interface, filter_list=filter_list)
-
-            return user_id, user_pred
+            user_fit_alg = users_fit_dict.get(user_idx)
+            if user_fit_alg is not None:
+                # we access [0] since [0] is rank_fn, [1] is pred_fn
+                user_fit_alg_rank_fn = user_fit_alg[0]
+                user_rank = user_fit_alg_rank_fn(user_idx, test_set, loaded_items_interface,
+                                                 recs_number=n_recs, filter_list=filter_list)
+            else:
+                user_rank = np.array([])
+                count_skipped_user += 1
+                # logger.warning(f"No algorithm fitted for user {user_idx}! It will be skipped")
 
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
+            return user_idx, user_rank
 
-        loaded_items_interface = self.algorithm._load_available_contents(self.items_directory, set())
+        count_skipped_user = 0
 
-        pred = []
+        loaded_items_interface = self._load_available_contents(items_directory, set())
 
-        logger.info("Don't worry if it looks stuck at first")
-        logger.info("First iterations will stabilize the estimated remaining time")
+        uir_rank_list = []
 
         with get_iterator_parallel(num_cpus,
-                                   compute_single_fit_predict, all_users,
-                                   progress_bar=True, total=len(all_users)) as pbar:
+                                   compute_single_rank, user_idx_list,
+                                   progress_bar=True, total=len(user_idx_list)) as pbar:
 
             pbar.set_description(f"Loading first items from memory...")
-            for user_id, user_pred in pbar:
-                pbar.set_description(f"Computing fit_predict for user {user_id}")
-                pred.append(user_pred)
-
-        pred = itertools.chain.from_iterable(pred)
-        pred = Prediction.from_list(pred)
+            for user_idx, user_rank in pbar:
+                pbar.set_description(f"Computing rank for user {user_idx}")
+                uir_rank_list.append(user_rank)
+
+        if count_skipped_user > 0:
+            logger.warning(f"{count_skipped_user} users will be skipped because the algorithm chosen "
+                           f"was not fit for them")
 
         # we force the garbage collector after freeing loaded items
         del loaded_items_interface
         gc.collect()
 
-        self._yaml_report = {'mode': 'score_prediction', 'methodology': repr(methodology)}
-
-        return pred
+        return uir_rank_list
 
-    def fit_rank(self, test_set: Ratings, n_recs: int = 10, user_id_list: List = None,
-                 methodology: Union[Methodology, None] = TestRatingsMethodology(),
-                 save_fit: bool = False, num_cpus: int = 1) -> Rank:
-        """
-        Method used to both fit and calculate ranking for all users in test set or all users in `user_id_list`
-        parameter.
-        The Recommender System will first be fit for each user in the train set passed in the constructor.
-        If the algorithm can't be fit for some users, a warning message is printed
+    def predict(self, users_fit_dict: dict, train_set: Ratings, test_set: Ratings, items_directory: str,
+                user_idx_list: Set[int], methodology: Methodology, num_cpus: int) -> List[np.ndarray]:
+        """
+        Method used to calculate score prediction for all users in `user_idx_list` parameter.
+        You must first call the `fit()` method ***before*** you can compute the ranking.
+        The `user_idx_list` parameter should contain users with mapped to their integer!
 
-        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
-        Otherwise, the rank will contain all unrated items of the particular users
+        The representation of the fit per-user cb algorithm is a dictionary where users idxs are keys and
+        a tuples containing `rank_fn` and `predict_fn` are values
 
         Via the `methodology` parameter you can perform different candidate item selection. By default, the
         `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
 
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
-
-        With the `save_fit` parameter you can decide if you want that you recommender system remains *fit* even after
-        the complete execution of this method, in case you want to compute ranking with other methodologies, or
-        with a different `n_recs` parameter. Be mindful since it can be memory-expensive, thus by default this behaviour
-        is disabled
+        If the algorithm was not fit for some users, they will be skipped and a warning message is printed showing the
+        number of users for which the alg couldn't produce a ranking
 
         Args:
+            users_fit_dict: dictionary with users idxs (int representation) are keys and tuples containing (`rank_fn`,
+                `predict_fn`) are values. In this dictionary only users for which the *fit* process could be performed
+                appear!
+            train_set: `Ratings` object which contains the train set of each user
             test_set: Ratings object which represents the ground truth of the split considered
-            n_recs: Number of the top items that will be present in the ranking of each user.
-                If `None` all candidate items will be returned for the user
-            user_id_list: List of users for which you want to compute the ranking. If None, the ranking will be computed
-                for all users of the `test_set`
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
             methodology: `Methodology` object which governs the candidate item selection. Default is
-                `TestRatingsMethodology`
-            save_fit: Boolean value which let you choose if the Recommender System should remain fit even after the
-                complete execution of this method. Default is False
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
-
-        Raises:
-            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
         Returns:
-            Rank object containing recommendation lists for all users of the test set or for all users in `user_id_list`
+            List of uir matrices for each user, where each uir contains predicted interactions between users and unseen
+                items
         """
-        def compute_single_fit_rank(user_id):
-            user_train = self.train_set.get_user_interactions(user_id)
 
-            alg = self.algorithm
-            if save_fit:
-                alg = deepcopy(alg)
-                self._user_fit_dic[user_id] = alg
+        def compute_single_predict(user_idx: int):
 
-            try:
-                alg.process_rated(user_train, loaded_items_interface)
-                alg.fit()
+            nonlocal count_skipped_user
 
-            except UserSkipAlgFit as e:
-                warning_message = str(e) + f"\nThe algorithm can't be fitted for the user {user_id}"
-                logger.warning(warning_message)
-                if save_fit:
-                    self._user_fit_dic[user_id] = None
-                return user_id, []
+            filter_list = methodology.filter_single(user_idx, train_set, test_set).astype(int)
+            # need to convert back int to str to load serialized items
+            filter_list = train_set.item_map.convert_seq_int2str(filter_list)
 
-            filter_list = None
-            if methodology is not None:
-                filter_list = set(methodology.filter_single(user_id, self.train_set, test_set))
-
-            user_rank = alg.rank(user_train, loaded_items_interface,
-                                 n_recs, filter_list=filter_list)
-
-            return user_id, user_rank
+            user_fitted_alg = users_fit_dict.get(user_idx)
+            if user_fitted_alg is not None:
+                # we access [1] since [1] is pred_fn, [0] is rank_fn
+                user_fitted_alg_pred_fn = user_fitted_alg[1]
+                user_pred = user_fitted_alg_pred_fn(user_idx, train_set, loaded_items_interface, filter_list=filter_list)
+            else:
+                user_pred = np.array([])
+                count_skipped_user += 1
+                # logger.warning(f"No algorithm fitted for user {user_id}! It will be skipped")
 
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
+            return user_idx, user_pred
 
-        loaded_items_interface = self.algorithm._load_available_contents(self.items_directory, set())
+        count_skipped_user = 0
 
-        rank = []
+        loaded_items_interface = self._load_available_contents(items_directory, set())
 
-        logger.info("Don't worry if it looks stuck at first")
-        logger.info("First iterations will stabilize the estimated remaining time")
+        uir_pred_list = []
 
         with get_iterator_parallel(num_cpus,
-                                   compute_single_fit_rank, all_users,
-                                   progress_bar=True, total=len(all_users)) as pbar:
+                                   compute_single_predict, user_idx_list,
+                                   progress_bar=True, total=len(user_idx_list)) as pbar:
 
             pbar.set_description(f"Loading first items from memory...")
-            for user_id, user_rank in pbar:
-                pbar.set_description(f"Computing fit_rank for user {user_id}")
-                rank.append(user_rank)
-
-        rank = itertools.chain.from_iterable(rank)
-        rank = Rank.from_list(rank)
+            for user_idx, user_pred in pbar:
+                pbar.set_description(f"Computing score prediction for user {user_idx}")
+                uir_pred_list.append(user_pred)
+
+        if count_skipped_user > 0:
+            logger.warning(f"{count_skipped_user} users will be skipped because the algorithm chosen "
+                           f"was not fit for them")
 
         # we force the garbage collector after freeing loaded items
         del loaded_items_interface
         gc.collect()
 
-        self._yaml_report = {'mode': 'rank', 'n_recs': repr(n_recs), 'methodology': repr(methodology)}
-
-        return rank
-
-    def __repr__(self):
-        return f"ContentBasedRS(algorithm={self.algorithm}, train_set={self.train_set}, " \
-               f"items_directory={self.items_directory}, users_directory={self.users_directory})"
-
-
-class GraphBasedRS(RecSys):
-    """
-    Class for recommender systems which use a graph in order to make predictions
-
-    Every GBRS differ from each other based the algorithm used.
-
-    Examples:
-
-        In case you perform a splitting of the dataset which returns a single train and test set (e.g. HoldOut
-        technique):
-
-        ```python title="Single split train"
-        from clayrs import recsys as rs
-        from clayrs import content_analyzer as ca
-
-        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
-
-        [train], [test] = rs.HoldOutPartitioning().split_all(original_rat)
+        return uir_pred_list
 
-        alg = rs.NXPageRank()  # any gb algorithm
+    def fit_rank(self, train_set: Ratings, test_set: Ratings, items_directory: str, user_idx_list: Set[int],
+                 n_recs: Optional[int], methodology: Methodology, num_cpus: int,
+                 save_fit: bool) -> Tuple[Optional[dict], List[np.ndarray]]:
+        """
+        Method used to both fit and calculate ranking for all users in `user_idx_list` parameter.
+        The algorithm will first be fit for each user in the `user_idx_list` which should contain user id
+        mapped to their integer!
+
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
+
+        With the `save_fit` parameter you can specify if you need the function to return the algorithm fit (in case
+        you want to perform multiple calls to the `predict()` or `rank()` function). If set to True, the first value
+        returned by this function will be the fit algorithm and the second will be the list of uir matrices with
+        predictions for each user.
+        Otherwise, if `save_fit` is False, the first value returned by this function will be `None`
 
-        graph = rs.NXBipartiteGraph(train)
+        Args:
+            train_set: `Ratings` object which contains the train set of each user
+            test_set: Ratings object which represents the ground truth of the split considered
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
+            n_recs: Number of the top items that will be present in the ranking of each user.
+                If `None` all candidate items will be returned for the user. Default is 10 (top-10 for each user
+                will be computed)
+            methodology: `Methodology` object which governs the candidate item selection. Default is
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            save_fit: Boolean value which let you choose if the fit algorithm should be saved and returned by this
+                function. If True, the first value returned by this function is the fit algorithm. Otherwise, the first
+                value will be None. The second value is always the list of predicted uir matrices
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
-        gbrs = rs.GraphBasedRS(alg, graph)
+        Returns:
+            A tuple where the first value is the fit VBPR algorithm (could be None if `save_fit == False`), the second
+            one is a list of predicted uir matrices all sorted in a decreasing order w.r.t. the ranking scores
+        """
 
-        rank = gbrs.rank(test, n_recs=10)
-        ```
+        def compute_single_fit_rank(user_idx):
 
-        In case you perform a splitting of the dataset which returns a multiple train and test sets (KFold technique):
+            nonlocal count_skipped_user, users_fit_dict
 
-        ```python title="Multiple split train"
-        from clayrs import recsys as rs
-        from clayrs import content_analyzer as ca
+            try:
+                self.process_rated(user_idx, train_set, loaded_items_interface)
+                self.fit_single_user()
 
-        original_rat = ca.Ratings(ca.CSVFile(ratings_path))
+                if save_fit:
+                    users_fit_dict[user_idx] = (self.rank_single_user, self.predict_single_user)
 
-        train_list, test_list = rs.KFoldPartitioning(n_splits=5).split_all(original_rat)
+            except UserSkipAlgFit as e:
+                # warning_message = str(e) + f"\nThe algorithm can't be fitted for the user {user_id}"
+                # logger.warning(warning_message)
+                count_skipped_user += 1
+                return user_idx, np.array([])
 
-        alg = rs.NXPageRank()  # any gb algorithm
+            filter_list = methodology.filter_single(user_idx, train_set, test_set).astype(int)
+            # need to convert back int to str to load serialized items
+            filter_list = train_set.item_map.convert_seq_int2str(filter_list)
 
-        for train_set, test_set in zip(train_list, test_list):
+            user_rank = self.rank_single_user(user_idx, test_set, loaded_items_interface,
+                                              n_recs, filter_list=filter_list)
 
-            graph = rs.NXBipartiteGraph(train_set)
-            gbrs = rs.GraphBasedRS(alg, graph)
-            rank_to_append = gbrs.rank(test_set)
+            return user_idx, user_rank
 
-            result_list.append(rank_to_append)
-        ```
+        count_skipped_user = 0
+        users_fit_dict = {} if save_fit else None
 
-        `result_list` will contain recommendation lists for each split
+        loaded_items_interface = self._load_available_contents(items_directory, set())
 
-    Args:
-        algorithm: the graph based algorithm that will be used in order to
-            rank or make score prediction
-        graph: a Graph object containing interactions
-    """
+        uir_rank_list = []
 
-    def __init__(self,
-                 algorithm: GraphBasedAlgorithm,
-                 graph: FullDiGraph):
+        with get_iterator_parallel(num_cpus,
+                                   compute_single_fit_rank, user_idx_list,
+                                   progress_bar=True, total=len(user_idx_list)) as pbar:
 
-        self.__graph = graph
-        super().__init__(algorithm)
+            pbar.set_description(f"Loading first items from memory...")
+            for user_idx, user_rank in pbar:
+                pbar.set_description(f"Computing fit_rank for user {user_idx}")
+                uir_rank_list.append(user_rank)
+
+        if count_skipped_user > 0:
+            logger.warning(f"{count_skipped_user} users will be skipped because the algorithm chosen "
+                           f"could not be fit for them")
 
-    @property
-    def users(self):
-        return self.__graph.user_nodes
+        # we force the garbage collector after freeing loaded items
+        del loaded_items_interface
+        gc.collect()
 
-    @property
-    def graph(self):
-        """
-        The graph containing interactions
-        """
-        return self.__graph
+        return users_fit_dict, uir_rank_list
 
-    @property
-    def algorithm(self):
-        """
-        The graph based algorithm chosen
+    def fit_predict(self, train_set: Ratings, test_set: Ratings, items_directory: str, user_idx_list: Set[int],
+                    methodology: Methodology, num_cpus: int,
+                    save_fit: bool) -> Tuple[Optional[dict], List[np.ndarray]]:
         """
-        alg: GraphBasedAlgorithm = super().algorithm
-        return alg
+        Method used to both fit and calculate score prediction for all users in `user_idx_list` parameter.
+        The algorithm will first be fit for each user in the `user_idx_list` which should contain user id
+        mapped to their integer!
 
-    def predict(self, test_set: Ratings, user_id_list: List = None,
-                methodology: Union[Methodology, None] = TestRatingsMethodology(),
-                num_cpus: int = 1) -> Prediction:
-        """
-        Method used to calculate score predictions for all users in test set or all users in `user_id_list` parameter.
+        If the algorithm is not a PredictionScore Algorithm, implement this method like this:
 
-        **BE CAREFUL**: not all algorithms are able to perform *score prediction*
+        ```python
+        def fit_predict():
+            raise NotPredictionAlg()
+        ```
 
-        Via the `methodology` parameter you can perform different candidate item selection. By default, the
-        `TestRatingsMethodology()` is used: so for each user items in its test set only will be considered for score
-        prediction
+        Any CB algorithm needs to know where the items are serialized by the content analyzer, hence the
+        `items_directory` parameter
 
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
+        With the `save_fit` parameter you can specify if you need the function to return the algorithm fit (in case
+        you want to perform multiple calls to the `predict()` or `rank()` function). If set to True, the first value
+        returned by this function will be the fit algorithm and the second will be the list of uir matrices with
+        predictions for each user.
+        Otherwise, if `save_fit` is False, the first value returned by this function will be `None`
 
         Args:
+            train_set: `Ratings` object which contains the train set of each user
             test_set: Ratings object which represents the ground truth of the split considered
-            user_id_list: List of users for which you want to compute score prediction. If None, the ranking
-                will be computed for all users of the `test_set`
+            items_directory: Path where complexly represented items are serialized by the Content Analyzer
+            user_idx_list: Set of user idx (int representation) for which a recommendation list must be generated.
+                Users should be represented with their mapped integer!
             methodology: `Methodology` object which governs the candidate item selection. Default is
-                `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+                `TestRatingsMethodology`. If None, AllItemsMethodology() will be used
+            save_fit: Boolean value which let you choose if the fit algorithm should be saved and returned by this
+                function. If True, the first value returned by this function is the fit algorithm. Otherwise, the first
+                value will be None. The second value is always the list of predicted uir matrices
+            num_cpus: number of processors that must be reserved for the method. If set to `0`, all cpus available will
+                be used. Be careful though: multiprocessing in python has a substantial memory overhead!
 
         Returns:
-            Prediction object containing score prediction lists for all users of the test set or for all users in
-                `user_id_list`
-
+            A tuple where the first value is the fit algorithm (could be None if `save_fit == False`), the second
+            one is a list of predicted uir matrices
         """
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
-
-        total_predict_list = self.algorithm.predict(all_users, self.graph, test_set, methodology, num_cpus)
-
-        total_predict = Prediction.from_list(total_predict_list)
 
-        self._yaml_report = {'graph': repr(self.graph), 'mode': 'score_prediction', 'methodology': repr(methodology)}
+        count_skipped_user = 0
+        users_fit_dict = {} if save_fit else None
 
-        return total_predict
+        def compute_single_fit_predict(user_idx):
 
-    def rank(self, test_set: Ratings, n_recs: int = 10, user_id_list: List = None,
-             methodology: Union[Methodology, None] = TestRatingsMethodology(),
-             num_cpus: int = 1) -> Rank:
-        """
-        Method used to calculate ranking for all users in test set or all users in `user_id_list` parameter.
-        You must first call the `fit()` method before you can compute the ranking.
-
-        If the `n_recs` is specified, then the rank will contain the top-n items for the users.
-        Otherwise, the rank will contain all unrated items of the particular users
+            nonlocal count_skipped_user, users_fit_dict
 
-        Via the `methodology` parameter you can perform different candidate item selection. By default, the
-        `TestRatingsMethodology()` is used: so, for each user, items in its test set only will be ranked
-
-        If the algorithm was not fit for some users, they will be skipped and a warning is printed
+            try:
+                self.process_rated(user_idx, train_set, loaded_items_interface)
+                self.fit_single_user()
 
-        Args:
-            test_set: Ratings object which represents the ground truth of the split considered
-            n_recs: Number of the top items that will be present in the ranking of each user.
-                If `None` all candidate items will be returned for the user
-            user_id_list: List of users for which you want to compute the ranking. If None, the ranking will be computed
-                for all users of the `test_set`
-            methodology: `Methodology` object which governs the candidate item selection. Default is
-                `TestRatingsMethodology`
-            num_cpus: number of processors that must be reserved for the method. Default is 0, meaning that
-                the number of cpus will be automatically detected.
+                if save_fit:
+                    users_fit_dict[user_idx] = (self.rank_single_user, self.predict_single_user)
 
-        Raises:
-            NotFittedAlg: Exception raised when this method is called without first calling the `fit` method
+            except UserSkipAlgFit as e:
+                # warning_message = str(e) + f"\nThe algorithm can't be fitted for the user {user_id}"
+                # logger.warning(warning_message)
+                count_skipped_user += 1
+                return user_idx, np.array([])
 
-        Returns:
-            Rank object containing recommendation lists for all users of the test set or for all users in `user_id_list`
+            filter_list = methodology.filter_single(user_idx, train_set, test_set).astype(int)
+            # need to convert back int to str to load serialized items
+            filter_list = train_set.item_map.convert_seq_int2str(filter_list)
 
-        """
-        all_users = set(test_set.user_id_column)
-        if user_id_list is not None:
-            all_users = set(user_id_list)
+            user_pred = self.predict_single_user(user_idx, test_set, loaded_items_interface, filter_list=filter_list)
 
-        total_rank_list = self.algorithm.rank(all_users, self.graph, test_set, n_recs, methodology, num_cpus)
+            return user_idx, user_pred
 
-        total_rank = Rank.from_list(total_rank_list)
+        loaded_items_interface = self._load_available_contents(items_directory, set())
 
-        if len(total_rank) == 0:
-            logger.warning("No items could be ranked for any users! Remember that items to rank must be present "
-                           "in the graph.\n"
-                           "Try changing methodology!")
+        uir_pred_list = []
 
-        elif len(set(total_rank.user_id_column)) != len(all_users):
-            logger.warning(f"No items could be ranked for users {all_users - set(total_rank.user_id_column)}\n"
-                           f"No nodes to rank for them found in the graph. Try changing methodology! ")
+        with get_iterator_parallel(num_cpus,
+                                   compute_single_fit_predict, user_idx_list,
+                                   progress_bar=True, total=len(user_idx_list)) as pbar:
 
-        self._yaml_report = {'graph': repr(self.graph), 'mode': 'rank', 'n_recs': repr(n_recs),
-                             'methodology': repr(methodology)}
+            pbar.set_description(f"Loading first items from memory...")
+            for user_idx, user_rank in pbar:
+                pbar.set_description(f"Computing fit_rank for user {user_idx}")
+                uir_pred_list.append(user_rank)
+
+        if count_skipped_user > 0:
+            logger.warning(f"{count_skipped_user} users will be skipped because the algorithm chosen "
+                           f"could not be fit for them")
 
-        return total_rank
+        # we force the garbage collector after freeing loaded items
+        del loaded_items_interface
+        gc.collect()
 
-    def __repr__(self):
-        return f"GraphBasedRS(algorithm={self.algorithm}, graph={self.graph})"
+        return users_fit_dict, uir_pred_list
```

### Comparing `clayrs-0.4.1/clayrs/utils/automatic_methods.py` & `clayrs-0.5.1/clayrs/utils/automatic_methods.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/utils/class_utils.py` & `clayrs-0.5.1/clayrs/utils/class_utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/utils/context_managers.py` & `clayrs-0.5.1/clayrs/utils/context_managers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import concurrent
+import concurrent.futures
 import os
+from concurrent.futures import as_completed
 from typing import Union, Iterator
 
 import distex
 import contextlib
 
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
@@ -46,7 +49,36 @@
             with get_progbar(iterator_res, total=total) as pbar:
                 yield pbar
         else:
             yield iterator_res
     finally:
         if pool is not None:
             pool.shutdown()
+
+
+@contextlib.contextmanager
+def get_iterator_thread(max_workers, f_to_thread, *args_to_f,
+                        keep_order=False, progress_bar=False, total=None) -> Union[Iterator, tqdm]:
+
+    # min(32, (os.cpu_count() or 1) + 4) taken from ThreadPoolExecutor
+    max_workers = max_workers or min(32, (os.cpu_count() or 1) + 4) or 1
+
+    if max_workers > 1:
+
+        ex = concurrent.futures.ThreadPoolExecutor(max_workers)
+        if keep_order:
+            iterator_res = ex.map(f_to_thread, *args_to_f)
+        else:
+            iterator_res = as_completed([ex.submit(f_to_thread, *args) for args in zip(*args_to_f)])
+    else:
+        ex = None
+        iterator_res = map(f_to_thread, *args_to_f)
+
+    try:
+        if progress_bar:
+            with get_progbar(iterator_res, total=total) as pbar:
+                yield pbar
+        else:
+            yield iterator_res
+    finally:
+        if ex is not None:
+            ex.shutdown()
```

### Comparing `clayrs-0.4.1/clayrs/utils/custom_logger.py` & `clayrs-0.5.1/clayrs/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/utils/load_content.py` & `clayrs-0.5.1/clayrs/utils/load_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs/utils/report.py` & `clayrs-0.5.1/clayrs/utils/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             # NameObject(a1=1.0, a2=2.0) -> [(a1, 1.0), (a2, 2.0)]
             # we are also matching whole nested objects as attributes, with the max recursion discussed above
             # NameObject(a1=1.0, a2=2.0, a3=NestedObject()) -> [(a1, 1.0), (a2, 2.0), (a3, NestedObject())]
             # we are matching any \w preceded by '(' (the beginning) or by a space (it's a follow up parameter)
             # which has as follow-up character the '=' and a nested object after that or anything else.
             # The last part is the bounding, the match ends when ', \w+=' is found (another parameter= or the ')' (the
             # end)
-            tuples_list_args = re.findall(r"(?<=\(|\s)(\w+)=(\w+"+balanced_parenthesis_pattern+r"|.*?)(?=,\s\w+=|\))",
+            tuples_list_args = re.findall(r"(?<=\(|\s)(\w+)=(\w+"+balanced_parenthesis_pattern+r"|.*?)(?=,\s\w+=|\)$)",
                                           repr_string)
 
             dict_args_string = dict(tuples_list_args)
 
             for key, val in dict_args_string.items():
 
                 # Recursive call so that each nested object (if any) will be expanded:
@@ -148,15 +148,15 @@
         field_names = content_analyzer._config.get_field_name_list()
         for field_name in field_names:
 
             field_config_list = content_analyzer._config.get_configs_list(field_name)
 
             for i, field_config in enumerate(field_config_list):
 
-                ca_dict['field_representations']['{}_{}'.format(field_name, str(i))] = dict()
+                ca_dict['field_representations']['{}/{}'.format(field_name, str(i))] = dict()
 
                 single_representation_dict = dict()
 
                 string_technique = repr(field_config.content_technique)
 
                 name_technique, parameter_dict_technique = self._extract_arguments(string_technique)
 
@@ -166,24 +166,24 @@
                 for preprocessing in field_config.preprocessing:
                     string_preprocessing = repr(preprocessing)
 
                     name_preprocessing, parameter_dict_preprocessing = self._extract_arguments(string_preprocessing)
 
                     single_representation_dict['preprocessing'][name_preprocessing] = parameter_dict_preprocessing
 
-                ca_dict['field_representations']['{}_{}'.format(field_name, str(i))] = single_representation_dict
+                ca_dict['field_representations']['{}/{}'.format(field_name, str(i))] = single_representation_dict
 
         return ca_dict
 
     def _report_rs_module(self, original_ratings: Ratings, partitioning_technique: Partitioning, recsys: RecSys):
 
-        # To provide a yaml report for recsys object, a rank or predict method must be called first
-        if recsys is not None and recsys._yaml_report is None:
-            raise ValueError("You must first call with the rank() or predict() method of the recsys object "
-                             "before computing the report!")
+        # # To provide a yaml report for recsys object, a rank or predict method must be called first
+        # if recsys is not None and recsys._yaml_report is None:
+        #     raise ValueError("You must first call with the rank() or predict() method of the recsys object "
+        #                      "before computing the report!")
 
         rs_dict = dict()
 
         if original_ratings is not None:
             rs_dict['interactions'] = dict()
 
             rs_dict['interactions']['n_users'] = len(set(original_ratings.user_id_column))
@@ -216,14 +216,15 @@
 
             parameters_recsys_dict = dict()
 
             name_alg, parameters_alg = self._extract_arguments(repr(recsys.algorithm))
 
             parameters_recsys_dict['algorithm'] = {name_alg: parameters_alg}
 
+            # _yaml_report is empty if no rank or pred method is called first
             for key, val in recsys._yaml_report.items():
 
                 val = val if isinstance(val, str) else repr(val)
 
                 # each item of the dict of the recsys may be an object with nested objects as attributes,
                 # we check this
                 name, parameters_dict = self._extract_arguments(val)
@@ -330,15 +331,15 @@
         """
 
         def represent_none(self, _):
             return self.represent_scalar('tag:yaml.org,2002:null', 'null')
 
         def dump_yaml(output_dir, data):
             with open(output_dir, 'w') as yaml_file:
-                pyaml.dump(data, yaml_file, sort_dicts=False, safe=True)
+                pyaml.dump(data, yaml_file, sort_dicts=False, safe=True,)
 
         # None values will be represented as 'null' in yaml file.
         # without this, they will simply be represented as an empty string
         pyaml.add_representer(type(None), represent_none)
 
         if content_analyzer is not None:
             ca_dict = self._report_ca_module(content_analyzer)
```

### Comparing `clayrs-0.4.1/clayrs/utils/save_content.py` & `clayrs-0.5.1/clayrs/utils/save_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/clayrs.egg-info/PKG-INFO` & `clayrs-0.5.1/clayrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: clayrs
-Version: 0.4.1
+Version: 0.5.1
 Summary: Complexly represent contents, build recommender systems, evaluate them. All in one place!
 Home-page: https://github.com/swapUniba/ClayRS
 Author: Antonio Silletti, Elio Musacchio, Roberta Sallustio
 License: GPL-3.0
 Keywords: recommender system,cbrs,evaluation,recsys
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Unit
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img src="https://user-images.githubusercontent.com/26851363/172485577-be6993ef-47c3-4b3c-9187-4988f6c44d94.svg" alt="ClayRS logo" style="width:75%;"/>
 </p>
 
 
 # ClayRS
 
 [![Build Status](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml/badge.svg)](https://github.com/swapUniba/ClayRS/actions/workflows/testing_pipeline.yml)&nbsp;&nbsp;
 [![Docs](https://github.com/swapUniba/ClayRS/actions/workflows/docs_building.yml/badge.svg)](https://swapuniba.github.io/ClayRS/)&nbsp;&nbsp;
 [![codecov](https://codecov.io/gh/swapUniba/ClayRS/branch/master/graph/badge.svg?token=dftmT3QD8D)](https://codecov.io/gh/swapUniba/ClayRS)&nbsp;&nbsp;
-[![Python versions](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/)
 
 
 ***ClayRS*** is a python framework for (mainly) content-based recommender systems which allows you to perform several operations, starting from a raw representation of users and items to building and evaluating a recommender system. It also supports graph-based recommendation with feature selection algorithms and graph manipulation methods.
 
 The framework has three main modules, which you can also use individually:
 
 <p align="center">
```

### Comparing `clayrs-0.4.1/clayrs.egg-info/SOURCES.txt` & `clayrs-0.5.1/clayrs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -39,19 +39,28 @@
 clayrs/content_analyzer/field_content_production_techniques/__init__.py
 clayrs/content_analyzer/field_content_production_techniques/field_content_production_technique.py
 clayrs/content_analyzer/field_content_production_techniques/synset_document_frequency.py
 clayrs/content_analyzer/field_content_production_techniques/tf_idf.py
 clayrs/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
 clayrs/content_analyzer/field_content_production_techniques/embedding_technique/combining_technique.py
 clayrs/content_analyzer/field_content_production_techniques/embedding_technique/embedding_technique.py
+clayrs/content_analyzer/field_content_production_techniques/visual_techniques/__init__.py
+clayrs/content_analyzer/field_content_production_techniques/visual_techniques/high_level_techniques.py
+clayrs/content_analyzer/field_content_production_techniques/visual_techniques/low_level_techniques.py
+clayrs/content_analyzer/field_content_production_techniques/visual_techniques/visual_content_techniques.py
 clayrs/content_analyzer/information_processor/__init__.py
-clayrs/content_analyzer/information_processor/ekphrasis.py
-clayrs/content_analyzer/information_processor/information_processor.py
-clayrs/content_analyzer/information_processor/nltk.py
-clayrs/content_analyzer/information_processor/spacy.py
+clayrs/content_analyzer/information_processor/ekphrasis_processor.py
+clayrs/content_analyzer/information_processor/information_processor_abstract.py
+clayrs/content_analyzer/information_processor/nltk_processor.py
+clayrs/content_analyzer/information_processor/spacy_processor.py
+clayrs/content_analyzer/information_processor/postprocessors/__init__.py
+clayrs/content_analyzer/information_processor/postprocessors/postprocessor.py
+clayrs/content_analyzer/information_processor/visual_preprocessors/__init__.py
+clayrs/content_analyzer/information_processor/visual_preprocessors/torch_builtin_augmenter.py
+clayrs/content_analyzer/information_processor/visual_preprocessors/torch_builtin_transformer.py
 clayrs/content_analyzer/memory_interfaces/__init__.py
 clayrs/content_analyzer/memory_interfaces/memory_interfaces.py
 clayrs/content_analyzer/memory_interfaces/text_interface.py
 clayrs/content_analyzer/ratings_manager/__init__.py
 clayrs/content_analyzer/ratings_manager/ratings.py
 clayrs/content_analyzer/ratings_manager/score_processor.py
 clayrs/content_analyzer/ratings_manager/sentiment_analysis.py
@@ -105,14 +114,18 @@
 clayrs/recsys/graphs/feature_selection/exceptions.py
 clayrs/recsys/graphs/feature_selection/feature_selection_alg.py
 clayrs/recsys/graphs/feature_selection/feature_selection_fn.py
 clayrs/recsys/graphs/nx_implementation/__init__.py
 clayrs/recsys/graphs/nx_implementation/nx_bipartite_graphs.py
 clayrs/recsys/graphs/nx_implementation/nx_full_graphs.py
 clayrs/recsys/graphs/nx_implementation/nx_tripartite_graphs.py
+clayrs/recsys/visual_based_algorithm/__init__.py
+clayrs/recsys/visual_based_algorithm/vbpr/__init__.py
+clayrs/recsys/visual_based_algorithm/vbpr/vbpr_algorithm.py
+clayrs/recsys/visual_based_algorithm/vbpr/vbpr_network.py
 clayrs/utils/__init__.py
 clayrs/utils/automatic_methods.py
 clayrs/utils/class_utils.py
 clayrs/utils/const.py
 clayrs/utils/context_managers.py
 clayrs/utils/custom_logger.py
 clayrs/utils/load_content.py
@@ -144,18 +157,27 @@
 test/content_analyzer/field_content_production_techniques/__init__.py
 test/content_analyzer/field_content_production_techniques/test_field_content_production_technique.py
 test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py
 test/content_analyzer/field_content_production_techniques/test_tf_idf.py
 test/content_analyzer/field_content_production_techniques/embedding_technique/__init__.py
 test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py
 test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py
+test/content_analyzer/field_content_production_techniques/visual_technique/__init__.py
+test/content_analyzer/field_content_production_techniques/visual_technique/test_high_level_techniques.py
+test/content_analyzer/field_content_production_techniques/visual_technique/test_low_level_techniques.py
+test/content_analyzer/field_content_production_techniques/visual_technique/test_visual_content_technique.py
 test/content_analyzer/information_processor/__init__.py
 test/content_analyzer/information_processor/test_ekphrasis.py
 test/content_analyzer/information_processor/test_nlp.py
 test/content_analyzer/information_processor/test_spacy.py
+test/content_analyzer/information_processor/test_visualpostprocessors/__init__.py
+test/content_analyzer/information_processor/test_visualpostprocessors/test_visualpostprocessor.py
+test/content_analyzer/information_processor/test_visualpreprocessors/__init__.py
+test/content_analyzer/information_processor/test_visualpreprocessors/test_torch_builtin_augmenter.py
+test/content_analyzer/information_processor/test_visualpreprocessors/test_torch_builtin_transformer.py
 test/content_analyzer/memory_interfaces/__init__.py
 test/content_analyzer/memory_interfaces/test_text_interface.py
 test/content_analyzer/ratings_manager/__init__.py
 test/content_analyzer/ratings_manager/test_rating_processor.py
 test/content_analyzer/ratings_manager/test_ratings.py
 test/content_analyzer/ratings_manager/test_sentiment_analysis.py
 test/content_analyzer/utils/__init__.py
@@ -200,13 +222,16 @@
 test/recsys/graphs/feature_selection/__init__.py
 test/recsys/graphs/feature_selection/test_feature_selection.py
 test/recsys/graphs/feature_selection/test_feature_selection_alg.py
 test/recsys/graphs/test_networkx_implementation/__init__.py
 test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py
 test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py
 test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py
+test/recsys/visual_based_algorithm/__init__.py
+test/recsys/visual_based_algorithm/vbpr/__init__.py
+test/recsys/visual_based_algorithm/vbpr/test_vbpr.py
 test/utils/__init__.py
 test/utils/test_automatic_methods.py
 test/utils/test_class_utils.py
 test/utils/test_context_managers.py
 test/utils/test_load_content.py
 test/utils/test_report.py
```

### Comparing `clayrs-0.4.1/setup.py` & `clayrs-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VERSION = "0.4.1"
+VERSION = "0.5.1"
 
 setup(name='clayrs',
       version=VERSION,
       license='GPL-3.0',
       author='Antonio Silletti, Elio Musacchio, Roberta Sallustio',
       install_requires=requirements,
       description='Complexly represent contents, build recommender systems, evaluate them. All in one place!',
       long_description=long_description,
       long_description_content_type="text/markdown",
       keywords=['recommender system', 'cbrs', 'evaluation', 'recsys'],
       url='https://github.com/swapUniba/ClayRS',
       include_package_data=True,
       packages=setuptools.find_packages(),
-      python_requires='>=3.7',
+      python_requires='>=3.8',
 
       classifiers=[
             'Development Status :: 3 - Alpha',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3 :: Only',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Topic :: Software Development :: Libraries',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Testing :: Unit'
       ]
```

### Comparing `clayrs-0.4.1/test/content_analyzer/content_representation/test_content.py` & `clayrs-0.5.1/test/content_analyzer/content_representation/test_content.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/content_representation/test_representation_container.py` & `clayrs-0.5.1/test/content_analyzer/content_representation/test_representation_container.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_doc2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 import os
 import pathlib as pl
 
 from clayrs.content_analyzer.embeddings.embedding_learner.doc2vec import GensimDoc2Vec
-from clayrs.content_analyzer.information_processor.nltk import NLTK
+from clayrs.content_analyzer.information_processor.nltk_processor import NLTK
 from clayrs.content_analyzer.raw_information_source import JSONFile
 from test import dir_test_files
 
 file_path = os.path.join(dir_test_files, 'movies_info_reduced.json')
 
 
 class TestGensimDoc2Vec(TestCase):
```

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_embedding_learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 
 import os
 
-from clayrs.content_analyzer.information_processor.nltk import NLTK
+from clayrs.content_analyzer.information_processor.nltk_processor import NLTK
 from clayrs.content_analyzer.raw_information_source import JSONFile
 from test.content_analyzer.embeddings.test_embedding_source import TestEmbeddingSource
 from clayrs.content_analyzer.embeddings.embedding_learner.doc2vec import GensimDoc2Vec
 from clayrs.content_analyzer.embeddings.embedding_learner.fasttext import GensimFastText
 from clayrs.content_analyzer.embeddings.embedding_learner.latent_semantic_analysis import GensimLatentSemanticAnalysis
 from clayrs.content_analyzer.embeddings.embedding_learner.random_indexing import GensimRandomIndexing
 from clayrs.content_analyzer.embeddings.embedding_learner.word2vec import GensimWord2Vec
```

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_fasttext.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 import os
 import pathlib as pl
 
 from clayrs.content_analyzer.embeddings.embedding_learner import GensimFastText
-from clayrs.content_analyzer.information_processor.nltk import NLTK
+from clayrs.content_analyzer.information_processor.nltk_processor import NLTK
 from clayrs.content_analyzer.raw_information_source import JSONFile
 from test import dir_test_files
 
 file_path = os.path.join(dir_test_files, 'movies_info_reduced.json')
 
 
 class TestGensimFastText(TestCase):
```

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_latent_semantic_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_lda.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_random_indexing.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_learner/test_word2vec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 import os
 import pathlib as pl
 
 from clayrs.content_analyzer.embeddings.embedding_learner import GensimWord2Vec
-from clayrs.content_analyzer.information_processor.nltk import NLTK
+from clayrs.content_analyzer.information_processor.nltk_processor import NLTK
 from clayrs.content_analyzer.raw_information_source import JSONFile
 from test import dir_test_files
 
 file_path = os.path.join(dir_test_files, 'movies_info_reduced.json')
 
 
 class TestGensimWord2Vec(TestCase):
```

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_gensim_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_sbert.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/embedding_loader/test_transformer.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/embeddings/test_embedding_source.py` & `clayrs-0.5.1/test/content_analyzer/embeddings/test_embedding_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py` & `clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_combining_technique.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py` & `clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/embedding_technique/test_embedding_technique.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,47 +19,47 @@
 
 file_path = os.path.join(dir_test_files, "movies_info_reduced.json")
 
 
 class TestEmbeddingTechnique(TestCase):
     def test_produce_content(self):
         technique = WordEmbeddingTechnique(GensimFastText())
-        embedding_list = technique.produce_content("Plot", [NLTK()], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [NLTK()], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
     def test_produce_content_str(self):
         self.skipTest("Test requires internet but is too complex to be mocked")
         technique = WordEmbeddingTechnique('glove-twitter-25')
         self.assertIsInstance(technique.embedding_source, Gensim)
-        embedding_list = technique.produce_content("Plot", [NLTK()], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [NLTK()], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
         technique = SentenceEmbeddingTechnique('paraphrase-distilroberta-base-v1')
         self.assertIsInstance(technique.embedding_source, Sbert)
-        embedding_list = technique.produce_content("Plot", [NLTK()], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [NLTK()], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
         technique = Word2DocEmbedding('glove-twitter-25', Centroid())
         self.assertIsInstance(technique.embedding_source, Gensim)
-        embedding_list = technique.produce_content("Plot", [], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
         technique = Sentence2DocEmbedding('paraphrase-distilroberta-base-v1', Centroid())
         self.assertIsInstance(technique.embedding_source, Sbert)
-        embedding_list = technique.produce_content("Plot", [NLTK()], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [NLTK()], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
         technique = Word2SentenceEmbedding('glove-twitter-25', Centroid())
         self.assertIsInstance(technique.embedding_source, Gensim)
-        embedding_list = technique.produce_content("Plot", [], JSONFile(file_path))
+        embedding_list = technique.produce_content("Plot", [], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
     def test_load_not_existing_source(self):
         self.skipTest("Test requires internet but is too complex to be mocked")
         with self.assertRaises(FileNotFoundError):
             WordEmbeddingTechnique('not_existing_model')
@@ -85,21 +85,21 @@
 
 class TestSentenceEmbeddingTechnique(TestCase):
 
     def test_produce_single_repr(self):
         file_path = os.path.join(dir_test_files, "movies_info_reduced.json")
         fromsentencetowords = SentenceEmbeddingTechnique(BertTransformers("prajjwal1/bert-tiny"))
 
-        embedding_list = fromsentencetowords.produce_content("Plot", [], JSONFile(file_path))
+        embedding_list = fromsentencetowords.produce_content("Plot", [], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
 
 
 class TestFromSentenceWordsEmbeddingTechnique(TestCase):
 
     def test_produce_single_repr(self):
         file_path = os.path.join(dir_test_files, "movies_info_reduced.json")
         fromsentencetowords = Sentence2WordEmbedding(BertTransformers("prajjwal1/bert-tiny"))
 
-        embedding_list = fromsentencetowords.produce_content("Plot", [], JSONFile(file_path))
+        embedding_list = fromsentencetowords.produce_content("Plot", [], [], JSONFile(file_path))
         self.assertEqual(len(embedding_list), 20)
         self.assertIsInstance(embedding_list[0], EmbeddingField)
```

### Comparing `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py` & `clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/test_synset_document_frequency.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 file_path = os.path.join(dir_test_files, "movies_info_reduced.json")
 
 
 class TestSynsetDocumentFrequency(TestCase):
     def test_produce_content(self):
         technique = PyWSDSynsetDocumentFrequency()
 
-        features_bag_list = technique.produce_content("Plot", [], JSONFile(file_path))
+        features_bag_list = technique.produce_content("Plot", [], [], JSONFile(file_path))
 
         self.assertEqual(len(features_bag_list), 20)
         self.assertIsInstance(features_bag_list[0], FeaturesBagField)
```

### Comparing `clayrs-0.4.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py` & `clayrs-0.5.1/test/content_analyzer/field_content_production_techniques/test_tf_idf.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 file_path = os.path.join(dir_test_files, "movies_info_reduced.json")
 
 
 class TestWhooshTfIdf(TestCase):
     def test_produce_content(self):
         technique = WhooshTfIdf()
 
-        features_bag_list = technique.produce_content("Plot", [], JSONFile(file_path))
+        features_bag_list = technique.produce_content("Plot", [], [], JSONFile(file_path))
 
         self.assertEqual(len(features_bag_list), 20)
         self.assertIsInstance(features_bag_list[0], FeaturesBagField)
 
 
 class TestSkLearnTfIdf(TestCase):
 
     def test_produce_content(self):
         technique = SkLearnTfIdf()
 
-        features_bag_list = technique.produce_content("Title", [], JSONFile(file_path))
+        features_bag_list = technique.produce_content("Title", [], [], JSONFile(file_path))
 
         self.assertEqual(len(features_bag_list), 20)
         self.assertIsInstance(features_bag_list[0], FeaturesBagField)
```

### Comparing `clayrs-0.4.1/test/content_analyzer/information_processor/test_ekphrasis.py` & `clayrs-0.5.1/test/content_analyzer/information_processor/test_ekphrasis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import ekphrasis.dicts.emoticons
 
-from clayrs.content_analyzer.information_processor.ekphrasis import Ekphrasis
+from clayrs.content_analyzer.information_processor.ekphrasis_processor import Ekphrasis
 
 
 class TestEkphrasis(unittest.TestCase):
     def test_omit_normalize(self):
         # we normalize email and percentages but we omit only emails
         ek = Ekphrasis(omit=['email'], normalize=['email', 'percent'])
```

### Comparing `clayrs-0.4.1/test/content_analyzer/information_processor/test_nlp.py` & `clayrs-0.5.1/test/content_analyzer/information_processor/test_nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 
 from nltk import Tree
 
-from clayrs.content_analyzer.information_processor.nltk import NLTK
+from clayrs.content_analyzer.information_processor.nltk_processor import NLTK
 
 
 class TestNLTK(TestCase):
 
     def test_process_stopwords(self):
         nltka = NLTK(stopwords_removal=True)
         expected = ["striped", "bats", "hanging", "feet", "best"]
```

### Comparing `clayrs-0.4.1/test/content_analyzer/information_processor/test_spacy.py` & `clayrs-0.5.1/test/content_analyzer/information_processor/test_spacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from clayrs.content_analyzer.information_processor.spacy import Spacy
+from clayrs.content_analyzer.information_processor.spacy_processor import Spacy
 
 
 class TestSpacy(TestCase):
 
     def test_process_stopwords(self):
         spa = Spacy(stopwords_removal=True)
         expected = ["striped", "bats", "hanging", "feet", "best"]
```

### Comparing `clayrs-0.4.1/test/content_analyzer/memory_interfaces/test_text_interface.py` & `clayrs-0.5.1/test/content_analyzer/memory_interfaces/test_text_interface.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/ratings_manager/test_rating_processor.py` & `clayrs-0.5.1/test/content_analyzer/ratings_manager/test_rating_processor.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py` & `clayrs-0.5.1/test/content_analyzer/ratings_manager/test_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/test_config.py` & `clayrs-0.5.1/test/content_analyzer/test_config.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/test_content_analyzer_main.py` & `clayrs-0.5.1/test/content_analyzer/test_content_analyzer_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
+import shutil
 import unittest
 from unittest import TestCase
 import lzma
 import pickle
 import numpy as np
 import scipy.sparse
 
 from clayrs.content_analyzer.exogenous_properties_retrieval import PropertiesFromDataset
 from clayrs.content_analyzer import ContentAnalyzer, FieldConfig, ExogenousConfig, ItemAnalyzerConfig
-from clayrs.content_analyzer.content_representation.content import SimpleField, FeaturesBagField, \
+from clayrs.content_analyzer.content_representation.content import FeaturesBagField, \
     EmbeddingField, IndexField, PropertiesDict
 from clayrs.content_analyzer.field_content_production_techniques import OriginalData
 from clayrs.content_analyzer.embeddings.embedding_loader.gensim import Gensim
 from clayrs.content_analyzer.field_content_production_techniques.embedding_technique.embedding_technique \
     import WordEmbeddingTechnique
 from clayrs.content_analyzer.field_content_production_techniques.tf_idf import SkLearnTfIdf
 from clayrs.content_analyzer.information_processor import NLTK
@@ -157,22 +158,22 @@
             id=['imdbID'],
             output_directory=output_dir,
         )
 
         movies_ca_config.add_multiple_config(
             field_name='Title',
             config_list=[FieldConfig(OriginalData(), NLTK(lemmatization=True, stopwords_removal=True),
-                         SearchIndex(os.path.join(output_dir, "index")), "test_search"),
+                         memory_interface=SearchIndex(os.path.join(output_dir, "index")), id="test_search"),
 
                          FieldConfig(SkLearnTfIdf(), NLTK(),
-                                     KeywordIndex(os.path.join(output_dir, "index1")),
-                                     "test_keyword"),
+                                     memory_interface=KeywordIndex(os.path.join(output_dir, "index1")),
+                                     id="test_keyword"),
 
                          FieldConfig(OriginalData(), NLTK(),
-                                     SearchIndex(os.path.join(output_dir, "index")))
+                                     memory_interface=SearchIndex(os.path.join(output_dir, "index")))
                          ])
 
         content_analyzer = ContentAnalyzer(movies_ca_config)
         content_analyzer.fit()
 
         for name in os.listdir(THIS_DIR):
             if os.path.isdir(os.path.join(THIS_DIR, name)) \
@@ -183,86 +184,14 @@
 
                     self.assertIsInstance(content.get_field("Title")[0], IndexField)
                     self.assertIsInstance(content.get_field("Title")[0].value, str)
                     self.assertIsInstance(content.get_field("Title")[1], IndexField)
                     self.assertIsInstance(content.get_field("Title")[1].value, str)
                     break
 
-    # Functionality to decode NOT IMPLEMENTED
-    #
-    # def test_decode_field_data_string(self):
-    #     movies_ca_config = ItemAnalyzerConfig(
-    #         source=JSONFile(decode_string),
-    #         id=['imdbID'],
-    #         output_directory=decode_path + 'movies_string_'
-    #     )
-    #
-    #     movies_ca_config.add_multiple_config(
-    #         field_name='Title',
-    #         config_list=[FieldConfig()]
-    #     )
-    #     ContentAnalyzer(config=movies_ca_config).fit()
-    #
-    #     for name in os.listdir(decode_path):
-    #         if os.path.isdir(os.path.join(decode_path, name)) \
-    #                 and 'movies_string_' in str(name):
-    #
-    #             with lzma.open(os.path.join(decode_path, name, 'tt0113497.xz'), 'r') as file:
-    #                 content = pickle.load(file)
-    #
-    #                 self.assertIsInstance(content.get_field("Title")[0], SimpleField)
-    #                 self.assertIsInstance(content.get_field("Title")[0].value, str)
-    #                 break
-    #
-    # def test_decode_field_data_tfidf(self):
-    #     movies_ca_config = ItemAnalyzerConfig(
-    #         source=JSONFile(decode_tfidf),
-    #         id=['imdbID'],
-    #         output_directory=decode_path + 'movies_tfidf_'
-    #     )
-    #
-    #     movies_ca_config.add_multiple_config(
-    #         field_name='Title',
-    #         config_list=[FieldConfig()]
-    #     )
-    #     ContentAnalyzer(config=movies_ca_config).fit()
-    #
-    #     for name in os.listdir(decode_path):
-    #         if os.path.isdir(os.path.join(decode_path, name)) \
-    #                 and 'movies_tfidf_' in str(name):
-    #             with lzma.open(os.path.join(decode_path, name, 'tt0113497.xz'), 'r') as file:
-    #                 content = pickle.load(file)
-    #
-    #                 self.assertIsInstance(content.get_field("Title")[0], FeaturesBagField)
-    #                 self.assertIsInstance(content.get_field("Title")[0].value, dict)
-    #                 break
-    #
-    # def test_decode_field_data_embedding(self):
-    #     movies_ca_config = ItemAnalyzerConfig(
-    #         source=JSONFile(decode_embedding),
-    #         id=['imdbID'],
-    #         output_directory=decode_path + 'movies_embedding_'
-    #     )
-    #
-    #     movies_ca_config.add_multiple_config(
-    #         field_name='Title',
-    #         config_list=[FieldConfig()]
-    #     )
-    #     ContentAnalyzer(config=movies_ca_config).fit()
-    #
-    #     for name in os.listdir(decode_path):
-    #         if os.path.isdir(os.path.join(decode_path, name)) \
-    #                 and 'movies_embedding_' in str(name):
-    #             with lzma.open(os.path.join(decode_path, name, 'tt0113497.xz'), 'r') as file:
-    #                 content = pickle.load(file)
-    #
-    #                 self.assertIsInstance(content.get_field("Title")[0], EmbeddingField)
-    #                 self.assertIsInstance(content.get_field("Title")[0].value, np.ndarray)
-    #                 break
-
 
 class TestContentAnalyzer(TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         cls.out_dir = 'test_export_json/'
 
     def test_fit_export_json(self):
@@ -284,14 +213,14 @@
 
         self.assertEqual(len(processed_source), 20)
         for processed_content in processed_source:
             self.assertIn('Plot#0', processed_content)
             self.assertIn('Plot#1', processed_content)
             self.assertIn('imdbRating#0', processed_content)
 
-    # def doCleanups(self) -> None:
-    #     if os.path.isdir(self.out_dir):
-    #         shutil.rmtree(self.out_dir)
+    def doCleanups(self) -> None:
+        if os.path.isdir(self.out_dir):
+            shutil.rmtree(self.out_dir)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `clayrs-0.4.1/test/content_analyzer/test_exogenous_properties_retrieval.py` & `clayrs-0.5.1/test/content_analyzer/test_exogenous_properties_retrieval.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/test_raw_information_source.py` & `clayrs-0.5.1/test/content_analyzer/test_raw_information_source.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/utils/test_check_tokenization.py` & `clayrs-0.5.1/test/content_analyzer/utils/test_check_tokenization.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/content_analyzer/utils/test_id_merger.py` & `clayrs-0.5.1/test/content_analyzer/utils/test_id_merger.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/evaluation/metrics/test_classification_metrics.py` & `clayrs-0.5.1/test/evaluation/metrics/test_classification_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,39 @@
 
         # any ClassificationMetric will work
         metric = Precision(relevant_threshold=4)
 
         with self.assertRaises(ValueError):
             metric.perform(split_no_rel)
 
+    def test_exception_different_users(self):
+
+        # test case in which user appears in prediction set but not in truth
+        pred_all_users = pred_w_new_items
+
+        truth_missing_u2 = pd.DataFrame(
+            {'user_id': ['u1', 'u1', 'u1', 'u1', 'u1'],
+             'item_id': ['i1', 'i2', 'i3', 'i4', 'i6'],
+             'score': [3, 2, 3, 1, 2]})
+        truth_missing_u2 = Ratings.from_dataframe(truth_missing_u2)
+
+        with self.assertRaises(ValueError):
+            Precision(relevant_threshold=2).perform(Split(pred_all_users, truth_missing_u2))
+
+        # test case in which user appears in truth but not in prediction set
+        pred_missing_u1 = pd.DataFrame(
+            {'user_id': ['u2', 'u2', 'u2', 'u2'],
+             'item_id': ['i4', 'i6', 'i1', 'i8'],
+             'score': [350, 200, 100, 50]})
+        pred_missing_u1 = Ratings.from_dataframe(pred_missing_u1)
+
+        truth_all_users = truth
+
+        with self.assertRaises(ValueError):
+            Precision(relevant_threshold=2).perform(Split(pred_missing_u1, truth_all_users))
 
 class TestPrecision(TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.metric_macro = Precision(relevant_threshold=3, sys_average='macro')
         cls.metric_micro = Precision(relevant_threshold=3, sys_average='micro')
```

### Comparing `clayrs-0.4.1/test/evaluation/metrics/test_error_metrics.py` & `clayrs-0.5.1/test/evaluation/metrics/test_error_metrics.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -249,8 +249,8 @@
         sys_expected = (u1_expected + u2_expected) / 2
         sys_result = float(result.query('user_id == "sys"')[str(metric)])
 
         self.assertAlmostEqual(sys_expected, sys_result)
 
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `clayrs-0.4.1/test/evaluation/metrics/test_fairness_metrics.py` & `clayrs-0.5.1/test/evaluation/metrics/test_fairness_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,49 +482,52 @@
         n_users = len(set(self.original_ratings.user_id_column))  # { u1, u2, u3, u4, u5, u6 } so 6 users
         pop_by_item = {item_id: count / n_users
                        for item_id, count in Counter(self.original_ratings.item_id_column).items()}
 
         expected_result_list = []
 
         for group_name, valid_group in valid_groups_splitted.items():
+            valid_group_idx = self.original_ratings.user_map.convert_seq_str2int(list(valid_group))
+
             # *******************************************************************************************
             # *** For every user in the group calculate the average popularity of the recommendations ***
             # *******************************************************************************************
 
             # compute for each user of the group the popularity sum in the recommendations
             # (cut the ranking list if top_n != None)
             RECS_sum_pop_group = {
-                user: sum([pop_by_item.get(interaction.item_id)
-                           for interaction in self.split.pred.get_user_interactions(user)][:top_n])
+                user_idx: sum([pop_by_item.get(self.split.pred.item_id_column[interaction_idx])
+                               for interaction_idx in self.split.pred.get_user_interactions(user_idx,
+                                                                                            as_indices=True)][:top_n])
 
-                for user in valid_group
+                for user_idx in valid_group_idx
             }
 
             # compute for each user of the group the average popularity in the recommendations
             # (sum_pop_item_recommended / n_item_recommended)
             # (cut the ranking list if top_n != None)
-            RECS_avg_pop_group = {user: sum_pop / len(self.split.pred.get_user_interactions(user)[:top_n])
-                                  for user, sum_pop in RECS_sum_pop_group.items()}
+            RECS_avg_pop_group = {user_idx: sum_pop / len(self.split.pred.get_user_interactions(user_idx)[:top_n])
+                                  for user_idx, sum_pop in RECS_sum_pop_group.items()}
 
             # ************************************************************************************
             # *** For every user in the group calculate the average popularity of the profiles ***
             # ************************************************************************************
 
             # compute for each user of the group the popularity sum in the recommendations
             PROFILE_sum_pop_group = {
-                user: sum([pop_by_item.get(interaction.item_id)
-                           for interaction in self.train.get_user_interactions(user)])
+                user_idx: sum([pop_by_item.get(self.train.item_id_column[interaction_idx])
+                               for interaction_idx in self.train.get_user_interactions(user_idx, as_indices=True)])
 
-                for user in valid_group
+                for user_idx in valid_group_idx
             }
 
             # compute for each user of the group the average popularity in the recommendations
             # (sum_pop_item_recommended / n_item_recommended)
-            PROFILE_avg_pop_group = {user: sum_pop / len(self.train.get_user_interactions(user))
-                                     for user, sum_pop in PROFILE_sum_pop_group.items()}
+            PROFILE_avg_pop_group = {user_idx: sum_pop / len(self.train.get_user_interactions(user_idx))
+                                     for user_idx, sum_pop in PROFILE_sum_pop_group.items()}
 
             # ************************
             # *** Compute DeltaGAP ***
             # ************************
 
             # sum the RECS_avg_pop of every user of the group / n_users in group
             RECS_gap_group = sum(RECS_avg_pop_group.values()) / len(valid_group)
```

### Comparing `clayrs-0.4.1/test/evaluation/metrics/test_plot_metrics.py` & `clayrs-0.5.1/test/evaluation/metrics/test_plot_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,20 +288,20 @@
         metric.perform(split)
         self.assertTrue(os.path.isfile(os.path.join('test_prof_recs/overwrite', 'prof_vs_recs.png')))
         self.assertTrue(os.path.isfile(os.path.join('test_prof_recs/overwrite', 'prof_vs_recs.csv')))
 
         self.assertFalse(os.path.isfile(os.path.join('test_prof_recs/overwrite', 'prof_vs_recs (3).png')))
         self.assertFalse(os.path.isfile(os.path.join('test_prof_recs/overwrite', 'prof_vs_recs (3).csv')))
 
-    # @classmethod
-    # def tearDownClass(cls) -> None:
-    #     os.remove('pop_ratio_profile_vs_recs.png')
-    #     os.remove('pop_ratio_profile_vs_recs.svg')
-    #     shutil.rmtree('test_prof_recs')
-    #     shutil.rmtree('test_more_splits')
+    @classmethod
+    def tearDownClass(cls) -> None:
+        os.remove('pop_ratio_profile_vs_recs.png')
+        os.remove('pop_ratio_profile_vs_recs.svg')
+        shutil.rmtree('test_prof_recs')
+        shutil.rmtree('test_more_splits')
 
 
 class TestPopRecsCorrelation(TestCase):
     def test_perform(self):
         # Save on same folder
         metric = PopRecsCorrelation(original_ratings=original_ratings)
         metric.perform(split)
```

### Comparing `clayrs-0.4.1/test/evaluation/metrics/test_ranking_metrics.py` & `clayrs-0.5.1/test/evaluation/metrics/test_ranking_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 pred_only_one_item = Ratings.from_dataframe(pred_only_one_item)
 
 truth = pd.DataFrame({'user_id': ['u1', 'u1', 'u1', 'u1', 'u1', 'u2', 'u2', 'u2'],
                       'item_id': ['i1', 'i2', 'i3', 'i4', 'i6', 'i1', 'i8', 'i4'],
                       'score': [3, 2, 3, 1, 2, 4, 3, 3]})
 truth = Ratings.from_dataframe(truth)
 
+
 split_only_new = Split(pred_only_new_items, truth)
 split_w_new_items = Split(pred_w_new_items, truth)
 split_only_one = Split(pred_only_one_item, truth)
 
 
 def for_each_method(test_func):
     def wrapper(self, *args, **kwargs):
@@ -51,33 +52,33 @@
         cls.metric = NDCG()
 
     def test_perform_only_new(self):
         metric = self.metric
 
         result_only_new = metric.perform(split_only_new)
 
-        ndcgs_predicted = set(result_only_new[str(metric)])
-        ndcgs_expected = {0}
-        self.assertEqual(ndcgs_expected, ndcgs_predicted)
+        # no items predicted is in truth, so ndcg can't be computed
+        for result in result_only_new[str(metric)]:
+            self.assertTrue(np.isnan(result))
 
     def test_perform_w_new_items(self):
         metric = self.metric
 
         result_w_new_items = metric.perform(split_w_new_items)
 
-        u1_actual = [[2, 3, 1, 0, 2, 3, 0, 0]]
-        u1_ideal = [[3, 3, 2, 2, 1, 0, 0, 0]]
+        u1_actual = [[600, 650, 220, 500, 300]]
+        u1_truth = [[3, 2, 3, 1, 2]]
 
-        u1_expected_ndcg = ndcg_score(u1_ideal, u1_actual)
+        u1_expected_ndcg = ndcg_score(u1_truth, u1_actual)
         u1_result_ndcg = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
 
         self.assertAlmostEqual(u1_expected_ndcg, u1_result_ndcg)
 
-        u2_actual = [[3, 0, 4, 3]]
-        u2_ideal = [[4, 3, 3, 0]]
+        u2_actual = [[100, 50, 350]]
+        u2_ideal = [[4, 3, 3]]
 
         u2_expected_ndcg = ndcg_score(u2_ideal, u2_actual)
         u2_result_ndcg = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
 
         self.assertAlmostEqual(u2_expected_ndcg, u2_result_ndcg)
 
         sys_expected_ndcg = (u1_expected_ndcg + u2_expected_ndcg) / 2
@@ -100,26 +101,26 @@
 
     def test_perform(self):
         k = 2
         metric = NDCGAtK(k=k)
 
         result_w_new_items = metric.perform(split_w_new_items)
 
-        u1_actual = [[2, 3, 1, 0, 2, 3, 0, 0]]
-        u1_ideal = [[3, 3, 2, 2, 1, 0, 0, 0]]
+        u1_actual_all = [[600, 650, 220, 500, 300]]
+        u1_truth_all = [[3, 2, 3, 1, 2]]
 
-        u1_expected_ndcg = ndcg_score(u1_ideal, u1_actual, k=k)
+        u1_expected_ndcg = ndcg_score(u1_truth_all, u1_actual_all, k=k)
         u1_result_ndcg = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
 
         self.assertAlmostEqual(u1_expected_ndcg, u1_result_ndcg)
 
-        u2_actual = [[3, 0, 4, 3]]
-        u2_ideal = [[4, 3, 3, 0]]
+        u2_actual_all = [[100, 50, 350]]
+        u2_truth_all = [[4, 3, 3]]
 
-        u2_expected_ndcg = ndcg_score(u2_ideal, u2_actual, k=k)
+        u2_expected_ndcg = ndcg_score(u2_truth_all, u2_actual_all, k=k)
         u2_result_ndcg = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
 
         self.assertAlmostEqual(u2_expected_ndcg, u2_result_ndcg)
 
         sys_expected_ndcg = (u1_expected_ndcg + u2_expected_ndcg) / 2
         sys_result_ndcg = float(result_w_new_items.query('user_id == "sys"')[str(metric)])
 
@@ -411,22 +412,26 @@
 
 
 class TestMAPAtK(unittest.TestCase):
 
     def test__compute_ap(self):
         relevant_threshold = 3
 
-        user_predictions = pred_w_new_items.get_user_interactions('u1')
-        user_truth = truth.get_user_interactions('u1')
-        user_truth_relevant_items = set(interaction.item_id for interaction in user_truth
-                                        if interaction.score >= relevant_threshold)
+        u1_uidx_pred = pred_w_new_items.user_map["u1"]
+        user_predictions_items_uidx = pred_w_new_items.get_user_interactions(u1_uidx_pred)[:, 1].astype(int)
+        user_predictions_items_str = pred_w_new_items.item_map[user_predictions_items_uidx]
+
+        u1_uidx_truth = truth.user_map["u1"]
+        user_truth = truth.get_user_interactions(u1_uidx_truth)
+        user_truth_relevant_items_uidx = user_truth[np.where(user_truth[:, 2] >= relevant_threshold)][:, 1].astype(int)
+        user_truth_relevant_items_str = truth.item_map[user_truth_relevant_items_uidx]
 
         metric = MAPAtK(k=2)
 
-        result_u1_ap = metric._compute_ap(user_predictions, user_truth_relevant_items)
+        result_u1_ap = metric._compute_ap(user_predictions_items_str, user_truth_relevant_items_str)
         expected_u1_ap = 1/2 * 1/2
         self.assertAlmostEqual(expected_u1_ap, result_u1_ap)
 
 
 class TestCorrelation(unittest.TestCase):
     @classmethod
     def setUpClass(cls) -> None:
@@ -455,62 +460,64 @@
 
     @for_each_method
     def test_perform_w_new_items(self, method):
         metric = Correlation(method)
 
         result_w_new_items = metric.perform(split_w_new_items)
 
-        u1_actual = pd.Series([1, 5, 0, 4, 2])
-        u1_ideal = pd.Series([0, 1, 2, 3, 4])
+        u1_truth = pd.Series([3, 2, 3, 1, 2])
+        u1_pred = pd.Series([600, 650, 220, 500, 300])
 
-        u1_expected_pearson = u1_actual.corr(u1_ideal, method)
-        u1_result_pearson = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
+        u1_expected_corr = u1_truth.corr(u1_pred, method)
+        u1_result_corr = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
 
-        self.assertAlmostEqual(u1_expected_pearson, u1_result_pearson)
+        self.assertAlmostEqual(u1_expected_corr, u1_result_corr)
 
-        u2_actual = pd.Series([2, 3, 0])
-        u2_ideal = pd.Series([0, 1, 2])
+        u2_truth = pd.Series([4, 3, 3])
+        u2_pred = pd.Series([100, 50, 350])
 
-        u2_expected_pearson = u2_actual.corr(u2_ideal, method)
-        u2_result_pearson = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
+        u2_expected_corr = u2_truth.corr(u2_pred, method)
+        u2_result_corr = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
 
-        self.assertAlmostEqual(u2_expected_pearson, u2_result_pearson)
+        self.assertAlmostEqual(u2_expected_corr, u2_result_corr)
 
-        sys_expected_pearson = (u1_expected_pearson + u2_expected_pearson) / 2
+        sys_expected_pearson = (u1_expected_corr + u2_expected_corr) / 2
         sys_result_pearson = float(result_w_new_items.query('user_id == "sys"')[str(metric)])
 
         self.assertAlmostEqual(sys_expected_pearson, sys_result_pearson)
 
     @for_each_method
     def test_perform_w_new_items_top_n(self, method: str):
         metric = Correlation(method, top_n=self.top_n)
 
         result_w_new_items = metric.perform(split_w_new_items)
 
-        u1_actual = pd.Series([1, 0])
-        u1_ideal = pd.Series([0, 1, 2, 3, 4])
+        # top_2 items i2==650, i1==600
+        u1_truth = pd.Series([3, 2])
+        u1_pred = pd.Series([600, 650])
 
-        u1_expected_pearson = u1_actual.corr(u1_ideal, method)
-        u1_result_pearson = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
+        u1_expected_corr = u1_truth.corr(u1_pred, method)
+        u1_result_corr = float(result_w_new_items.query('user_id == "u1"')[str(metric)])
 
-        self.assertAlmostEqual(u1_expected_pearson, u1_result_pearson)
+        self.assertAlmostEqual(u1_expected_corr, u1_result_corr)
 
-        u2_actual = pd.Series([0])
-        u2_ideal = pd.Series([0, 1, 2])
+        # top_2 items i4=350, i6==200 which does not appear in truth
+        u2_truth = pd.Series([3])
+        u2_pred = pd.Series([350])
 
-        u2_expected_pearson = u2_actual.corr(u2_ideal, method)
-        u2_result_pearson = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
+        u2_expected_corr = u2_truth.corr(u2_pred, method)
+        u2_result_corr = float(result_w_new_items.query('user_id == "u2"')[str(metric)])
 
-        self.assertTrue(np.isnan(u2_expected_pearson))
-        self.assertTrue(np.isnan(u2_result_pearson))
+        self.assertTrue(np.isnan(u2_expected_corr))
+        self.assertTrue(np.isnan(u2_result_corr))
 
-        sys_expected_pearson = u1_expected_pearson  # the mean doesn't consider nan values
-        sys_result_pearson = float(result_w_new_items.query('user_id == "sys"')[str(metric)])
+        sys_expected_corr = u1_expected_corr  # the mean doesn't consider nan values
+        sys_result_corr = float(result_w_new_items.query('user_id == "sys"')[str(metric)])
 
-        self.assertAlmostEqual(sys_expected_pearson, sys_result_pearson)
+        self.assertAlmostEqual(sys_expected_corr, sys_result_corr)
 
     @for_each_method
     def test_perform_only_one(self, method: str):
         metric = Correlation(method)
 
         result_only_one = metric.perform(split_only_one)
```

### Comparing `clayrs-0.4.1/test/evaluation/test_eval_model.py` & `clayrs-0.5.1/test/evaluation/test_eval_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from clayrs.evaluation.metrics.ranking_metrics import NDCG
 
 from clayrs.evaluation.metrics.classification_metrics import Precision
 from clayrs.evaluation.eval_model import EvalModel
 
 import pandas as pd
 
-from test import dir_test_files
-
 original_ratings = pd.DataFrame(
     {'user_id': ['u1', 'u1', 'u1', 'u1', 'u1', 'u1', 'u1', 'u1',
                  'u2', 'u2', 'u2', 'u2',
                  'u3', 'u3', 'u3', 'u3', 'u3', 'u3',
                  'u4', 'u4', 'u4', 'u4', 'u4', 'u4', 'u4',
                  'u5', 'u5', 'u5', 'u5', 'u5',
                  'u6', 'u6'],
@@ -226,18 +224,24 @@
         os.remove('long_tail_distr_truth (1).png')
 
     def test_fit_user_list(self):
         # we compute evaluation only for a certain users
 
         # we must also cut user profiles of DeltaGAP by only considering u1, u2, u3
         self.metric_list.pop(4)
+
+        filter_list = ['u1', 'u2', 'u3']
+        filter_1 = train_1.user_map.convert_seq_str2int(filter_list)
+        filter_2 = train_2.user_map.convert_seq_str2int(filter_list)
+        original_filter = original_ratings.user_map.convert_seq_str2int(filter_list)
+
         self.metric_list.append(DeltaGap({'a': 0.2, 'b': 0.5, 'c': 0.3},
-                                         user_profiles=[train_1.filter_ratings(['u1', 'u2', 'u3']),
-                                                        train_2.filter_ratings(['u1', 'u2', 'u3'])],
-                                         original_ratings=original_ratings.filter_ratings(['u1', 'u2', 'u3']))
+                                         user_profiles=[train_1.filter_ratings(filter_1),
+                                                        train_2.filter_ratings(filter_2)],
+                                         original_ratings=original_ratings.filter_ratings(original_filter))
                                 )
 
         em = EvalModel(pred_list, truth_list, self.metric_list)
         sys_result, user_results = em.fit(['u1', 'u2', 'u3'])
 
         self.assertIsInstance(sys_result, pd.DataFrame)
         self.assertIsInstance(user_results, pd.DataFrame)
```

### Comparing `clayrs-0.4.1/test/evaluation/test_statistical_tests.py` & `clayrs-0.5.1/test/evaluation/test_statistical_tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,16 @@
                                          'NDCG': [0.5, 0.7, 0.8, 0.2],
                                          'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
 
         equal_users_sys2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                          'NDCG': [0.8, 0.2, 0.2, 0.4],
                                          'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
-        result = StatisticalTest._common_users(equal_users_sys1, equal_users_sys2, column_list=['NDCG'])
+        result = StatisticalTest._common_users(equal_users_sys1, "user_id", equal_users_sys2, "user_id",
+                                               column_list=['NDCG'])
 
         expected_dict = {'NDCG_x': [0.5, 0.7, 0.8, 0.2],
                          'user_id': ['u1', 'u2', 'u3', 'u4'],
                          'NDCG_y': [0.8, 0.2, 0.2, 0.4]}
         result_dict = result.to_dict(orient='list')
 
         self.assertDictEqual(expected_dict, result_dict)
@@ -31,15 +32,16 @@
                                          'NDCG': [0.5, 0.7, 0.8, 0.2],
                                          'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
 
         equal_users_sys2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                          'NDCG': [0.8, 0.2, 0.2, 0.4],
                                          'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
-        result = StatisticalTest._common_users(equal_users_sys1, equal_users_sys2, column_list=['NDCG'])
+        result = StatisticalTest._common_users(equal_users_sys1, "user_id", equal_users_sys2,
+                                               "user_id", column_list=['NDCG'])
 
         expected_dict = {'NDCG_x': [0.8, 0.2],
                          'user_id': ['u3', 'u4'],
                          'NDCG_y': [0.2, 0.4]}
         result_dict = result.to_dict(orient='list')
 
         self.assertDictEqual(expected_dict, result_dict)
@@ -49,15 +51,16 @@
                                          'MRR': [0.5, 0.7, 0.8, 0.2],
                                          'Precision - macro': [0.998, 0.123, 0.556, 0.887]})
 
         equal_users_sys2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                          'NDCG': [0.8, 0.2, 0.2, 0.4],
                                          'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
-        result = StatisticalTest._common_users(equal_users_sys1, equal_users_sys2, column_list=[])
+        result = StatisticalTest._common_users(equal_users_sys1, "user_id", equal_users_sys2, "user_id",
+                                               column_list=[])
 
         expected_dict = {'user_id': ['u1', 'u2', 'u3', 'u4']}
         result_dict = result.to_dict(orient='list')
 
         self.assertDictEqual(expected_dict, result_dict)
 
         # no metric in common and no user in common
@@ -65,15 +68,16 @@
                                          'MRR': [0.5, 0.7, 0.8, 0.2],
                                          'Precision - macro': [0.998, 0.123, 0.556, 0.887]})
 
         equal_users_sys2 = pd.DataFrame({'user_id': ['u5', 'u6', 'u7', 'u8'],
                                          'NDCG': [0.8, 0.2, 0.2, 0.4],
                                          'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
-        result = StatisticalTest._common_users(equal_users_sys1, equal_users_sys2, column_list=[])
+        result = StatisticalTest._common_users(equal_users_sys1, "user_id", equal_users_sys2, "user_id",
+                                               column_list=[])
 
         expected_dict = {'user_id': []}
         result_dict = result.to_dict(orient='list')
 
         self.assertDictEqual(expected_dict, result_dict)
 
 
@@ -97,18 +101,22 @@
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                               'NDCG': [0.8, 0.2, 0.2, 0.4],
                                               'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
 
-        result_ndcg = result_df['NDCG'].values[0]
-        result_precision = result_df['Precision - micro'].values[0]
+                         list(result_df.columns))
+
+        result_ndcg = tuple(result_df['NDCG'].values[0])
+
+        result_precision = tuple(result_df['Precision - micro'].values[0])
 
         expected_ndcg = external_function([0.5, 0.7, 0.8, 0.2], [0.8, 0.2, 0.2, 0.4])
         expected_precision = external_function([0.998, 0.123, 0.556, 0.887], [0.45, 0.23, 0.112, 0.776])
 
         self.assertEqual(expected_ndcg, result_ndcg)
         self.assertEqual(expected_precision, result_precision)
 
@@ -124,25 +132,29 @@
 
         users_metrics_result3 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                               'NDCG': [0.9, 0.3, 0.2, 0.5],
                                               'Precision - micro': [0.44, 0.88, 0.21, 0.56]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2, users_metrics_result3])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
+
+                              list(result_df.columns))
 
         # we expect sys1/sys2, sys1/sys3, sys2/sys3
         self.assertTrue(len(result_df) == 3)
 
-        result_ndcg_12 = result_df['NDCG'].values[0]
-        result_ndcg_13 = result_df['NDCG'].values[1]
-        result_ndcg_23 = result_df['NDCG'].values[2]
-        result_precision_12 = result_df['Precision - micro'].values[0]
-        result_precision_13 = result_df['Precision - micro'].values[1]
-        result_precision_23 = result_df['Precision - micro'].values[2]
+        result_ndcg_12 = tuple(result_df['NDCG'].values[0])
+        result_ndcg_13 = tuple(result_df['NDCG'].values[1])
+        result_ndcg_23 = tuple(result_df['NDCG'].values[2])
+
+        result_precision_12 = tuple(result_df['Precision - micro'].values[0])
+        result_precision_13 = tuple(result_df['Precision - micro'].values[1])
+        result_precision_23 = tuple(result_df['Precision - micro'].values[2])
 
         expected_ndcg_12 = external_function([0.5, 0.7, 0.8, 0.2], [0.8, 0.2, 0.2, 0.4])
         expected_ndcg_13 = external_function([0.5, 0.7, 0.8, 0.2], [0.9, 0.3, 0.2, 0.5])
         expected_ndcg_23 = external_function([0.8, 0.2, 0.2, 0.4], [0.9, 0.3, 0.2, 0.5])
         expected_precision_12 = external_function([0.998, 0.123, 0.556, 0.887], [0.45, 0.23, 0.112, 0.776])
         expected_precision_13 = external_function([0.998, 0.123, 0.556, 0.887], [0.44, 0.88, 0.21, 0.56])
         expected_precision_23 = external_function([0.45, 0.23, 0.112, 0.776], [0.44, 0.88, 0.21, 0.56])
@@ -150,31 +162,66 @@
         self.assertEqual(expected_ndcg_12, result_ndcg_12)
         self.assertEqual(expected_ndcg_13, result_ndcg_13)
         self.assertEqual(expected_ndcg_23, result_ndcg_23)
         self.assertEqual(expected_precision_12, result_precision_12)
         self.assertEqual(expected_precision_13, result_precision_13)
         self.assertEqual(expected_precision_23, result_precision_23)
 
+        # perform all users in common but not all metrics
+        users_metrics_result1 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
+                                              'NDCG': [0.5, 0.7, 0.8, 0.2],
+                                              'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
+
+        users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
+                                              'NDCG': [0.8, 0.2, 0.2, 0.4],
+                                              'Recall - micro': [0.45, 0.23, 0.112, 0.776]})
+
+        users_metrics_result3 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
+                                              'MRR': [0.9, 0.3, 0.2, 0.5],
+                                              'Recall - micro': [0.44, 0.88, 0.21, 0.56]})
+
+        result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2, users_metrics_result3])
+
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Recall - micro', 'statistic'), ('Recall - micro', 'pvalue')],
+
+                              list(result_df.columns))
+
+        # we expect sys1/sys2, sys2/sys3 (sys1/sys3 missing since no metric is in common)
+        self.assertTrue(len(result_df) == 2)
+
+        # sys1/sys2 do not have in common recall (so nan value is expected)
+        self.assertTrue(np.isnan(result_df['Recall - micro']["statistic"].values[0]))
+        self.assertTrue(np.isnan(result_df['Recall - micro']["pvalue"].values[0]))
+
+        # sys2/sys3 do not have in common ndcg (so nan value is expected)
+        self.assertTrue(np.isnan(result_df["NDCG"]["statistic"].values[1]))
+        self.assertTrue(np.isnan(result_df["NDCG"]["pvalue"].values[1]))
+
     def perform_only_some_in_common(self, class_to_test, external_function):
         # perform only some users in common
         users_metrics_result1 = pd.DataFrame({'user_id': ['u5', 'u6', 'u3', 'u4'],
                                               'NDCG': [0.5, 0.7, 0.8, 0.2],
                                               'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'NDCG': [0.8, 0.2, 0.2, 0.4],
                                               'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
+
+                         list(result_df.columns))
 
-        result_ndcg = result_df['NDCG'].values[0]
-        result_precision = result_df['Precision - micro'].values[0]
+        result_ndcg = tuple(result_df['NDCG'].values[0])
+        result_precision = tuple(result_df['Precision - micro'].values[0])
 
+        # we consider values only from user in common
         expected_ndcg = external_function([0.8, 0.2], [0.2, 0.4])
         expected_precision = external_function([0.556, 0.887], [0.23, 0.776])
 
         self.assertEqual(expected_ndcg, result_ndcg)
         self.assertEqual(expected_precision, result_precision)
 
         # perform only some users and only some columns in common
@@ -184,17 +231,19 @@
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'MRR': [0.8, 0.2, 0.2, 0.4],
                                               'NDCG': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue')],
+
+                         list(result_df.columns))
 
-        result_ndcg = result_df['NDCG'].values[0]
+        result_ndcg = tuple(result_df['NDCG'].values[0])
 
         expected_ndcg = external_function([0.8, 0.2], [0.23, 0.776])
 
         self.assertEqual(expected_ndcg, result_ndcg)
         self.assertEqual(expected_precision, result_precision)
 
     def perform_nothing_in_common(self, class_to_test, external_function):
@@ -205,23 +254,26 @@
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'NDCG': [0.8, 0.2, 0.2, 0.4],
                                               'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
 
-        result_ndcg = result_df['NDCG'].values[0]
-        result_precision = result_df['Precision - micro'].values[0]
+                         list(result_df.columns))
 
-        self.assertTrue(np.isnan(result_ndcg.statistic))
-        self.assertTrue(np.isnan(result_ndcg.pvalue))
-        self.assertTrue(np.isnan(result_precision.statistic))
-        self.assertTrue(np.isnan(result_precision.pvalue))
+        result_ndcg = tuple(result_df['NDCG'].values[0])
+        result_precision = tuple(result_df['Precision - micro'].values[0])
+
+        self.assertTrue(np.isnan(result_ndcg[0]))
+        self.assertTrue(np.isnan(result_ndcg[1]))
+        self.assertTrue(np.isnan(result_precision[0]))
+        self.assertTrue(np.isnan(result_precision[1]))
 
         # perform users in common but not columns in common
         users_metrics_result1 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
                                               'NDCG': [0.5, 0.7, 0.8, 0.2],
                                               'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
@@ -240,23 +292,26 @@
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'NDCG': [np.nan, 0.2, 0.2, 0.4],
                                               'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
+
+                         list(result_df.columns))
 
         # ndcg column has one nan values, we don't use it
         expected_ndcg = external_function([0.7, 0.8, 0.2], [0.2, 0.2, 0.4])
         # other metric columns are unaffected
         expected_precision = external_function([0.998, 0.123, 0.556, 0.887], [0.45, 0.23, 0.112, 0.776])
 
-        result_ndcg = result_df['NDCG'].values[0]
-        result_precision = result_df['Precision - micro'].values[0]
+        result_ndcg = tuple(result_df['NDCG'].values[0])
+        result_precision = tuple(result_df['Precision - micro'].values[0])
 
         self.assertEqual(expected_ndcg, result_ndcg)
         self.assertEqual(expected_precision, result_precision)
 
         # all users have nan values in NDCG column
         users_metrics_result1 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'NDCG': [np.nan, np.nan, np.nan, np.nan],
@@ -264,28 +319,75 @@
 
         users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u3', 'u2', 'u4'],
                                               'NDCG': [np.nan, np.nan, np.nan, np.nan],
                                               'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
 
         result_df = class_to_test.perform([users_metrics_result1, users_metrics_result2])
 
-        self.assertTrue(['NDCG', 'Precision - micro'] == list(result_df.columns))
+        self.assertCountEqual([('NDCG', 'statistic'), ('NDCG', 'pvalue'),
+                               ('Precision - micro', 'statistic'), ('Precision - micro', 'pvalue')],
+
+                         list(result_df.columns))
 
         # NDCG columns has all nan values, so we can't compute the statistic
-        result_ndcg = result_df['NDCG'].values[0]
+        result_ndcg = tuple(result_df['NDCG'].values[0])
 
-        self.assertTrue(np.isnan(result_ndcg.statistic))
-        self.assertTrue(np.isnan(result_ndcg.pvalue))
+        self.assertTrue(np.isnan(result_ndcg[0]))
+        self.assertTrue(np.isnan(result_ndcg[1]))
 
         # other metric columns are unaffected
         expected_precision = external_function([0.998, 0.123, 0.556, 0.887], [0.45, 0.23, 0.112, 0.776])
-        result_precision = result_df['Precision - micro'].values[0]
+        result_precision = tuple(result_df['Precision - micro'].values[0])
 
         self.assertEqual(expected_precision, result_precision)
 
+    def test_check_col_specified(self):
+
+        # perform by default column name is "user_id", so no necessary to specify it
+        stat_test = Ttest()
+        stat_test_col_specified = Ttest("user_id")
+
+        users_metrics_result1 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
+                                              'NDCG': [0.5, 0.7, 0.8, 0.2],
+                                              'Precision - micro': [0.998, 0.123, 0.556, 0.887]})
+
+        users_metrics_result2 = pd.DataFrame({'user_id': ['u1', 'u2', 'u3', 'u4'],
+                                              'NDCG': [0.8, 0.2, 0.2, 0.4],
+                                              'Precision - micro': [0.45, 0.23, 0.112, 0.776]})
+
+        expected = stat_test.perform([users_metrics_result1, users_metrics_result2])
+        result = stat_test_col_specified.perform([users_metrics_result1, users_metrics_result2])
+
+        self.assertEqual(tuple(expected["NDCG"].values[0]), tuple(result["NDCG"].values[0]))
+        self.assertEqual(tuple(expected["Precision - micro"].values[0]),
+                         tuple(result["Precision - micro"].values[0]))
+
+        # the two dataframes have different column name for "user_id"
+
+        users_metrics_result2.columns = ["user_idx", "NDCG", "Precision - micro"]
+
+        with self.assertRaises(KeyError):
+            stat_test.perform([users_metrics_result1, users_metrics_result2])
+
+        # but if we specify it we are safe
+        stat_test_col_specified = Ttest("user_id", "user_idx")
+
+        result = stat_test_col_specified.perform([users_metrics_result1, users_metrics_result2])
+
+        self.assertEqual(tuple(expected["NDCG"].values[0]), tuple(result["NDCG"].values[0]))
+        self.assertEqual(tuple(expected["Precision - micro"].values[0]),
+                         tuple(result["Precision - micro"].values[0]))
+
+        # case in which the user columns specified do not match len of df_list
+        stat_test_col_specified = Ttest("user_id", "user_idx", "user_idxx")
+
+        with self.assertRaises(ValueError):
+            stat_test_col_specified.perform([users_metrics_result1, users_metrics_result2])
+
+
 
 class TestTtest(TestPairedTest):
 
     def test_perform_all_in_common(self):
         self.perform_all_in_common(Ttest(), ttest_ind)
 
     def test_perform_only_some_in_common(self):
```

### Comparing `clayrs-0.4.1/test/evaluation/test_utils.py` & `clayrs-0.5.1/test/evaluation/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,35 +54,45 @@
     def test_get_avg_pop(self):
 
         counter_popularity = Counter(self.custom_rat.item_id_column)
 
         # Expected result are item_popularity rated by user / n_item rated by user
         # item_popularity is the number of occurrences of the item in the 'to_id' column
 
-        u1_items = [interaction.item_id for interaction in self.custom_rat.get_user_interactions('u1')]
-        result_u1 = get_avg_pop(u1_items, counter_popularity)
+        u1_idx = self.custom_rat.user_map["u1"]
+        u1_items_idx = self.custom_rat.get_user_interactions(u1_idx)[:, 1].astype(int)
+        u1_items_str = self.custom_rat.item_map[u1_items_idx]
+        result_u1 = get_avg_pop(u1_items_str, counter_popularity)
         expected_u1 = (counter_popularity['i1'] + counter_popularity['i2']) / 2
         self.assertAlmostEqual(expected_u1, result_u1)
 
-        u2_items = [interaction.item_id for interaction in self.custom_rat.get_user_interactions('u2')]
-        result_u2 = get_avg_pop(u2_items, counter_popularity)
+        u2_idx = self.custom_rat.user_map["u2"]
+        u2_items_idx = self.custom_rat.get_user_interactions(u2_idx)[:, 1].astype(int)
+        u2_items_str = self.custom_rat.item_map[u2_items_idx]
+        result_u2 = get_avg_pop(u2_items_str, counter_popularity)
         expected_u2 = (counter_popularity['i1'] + counter_popularity['i50']) / 2
         self.assertAlmostEqual(expected_u2, result_u2)
 
-        u3_items = [interaction.item_id for interaction in self.custom_rat.get_user_interactions('u3')]
-        result_u3 = get_avg_pop(u3_items, counter_popularity)
+        u3_idx = self.custom_rat.user_map["u3"]
+        u3_items_idx = self.custom_rat.get_user_interactions(u3_idx)[:, 1].astype(int)
+        u3_items_str = self.custom_rat.item_map[u3_items_idx]
+        result_u3 = get_avg_pop(u3_items_str, counter_popularity)
         expected_u3 = (counter_popularity['i1'] + counter_popularity['i2']) / 2
         self.assertAlmostEqual(expected_u3, result_u3)
 
-        u4_items = [interaction.item_id for interaction in self.custom_rat.get_user_interactions('u4')]
-        result_u4 = get_avg_pop(u4_items, counter_popularity)
+        u4_idx = self.custom_rat.user_map["u4"]
+        u4_items_idx = self.custom_rat.get_user_interactions(u4_idx)[:, 1].astype(int)
+        u4_items_str = self.custom_rat.item_map[u4_items_idx]
+        result_u4 = get_avg_pop(u4_items_str, counter_popularity)
         expected_u4 = (counter_popularity['i1'] + counter_popularity['i50']) / 2
         self.assertAlmostEqual(expected_u4, result_u4)
 
-        u5_items = [interaction.item_id for interaction in self.custom_rat.get_user_interactions('u5')]
-        result_u5 = get_avg_pop(u5_items, counter_popularity)
+        u5_idx = self.custom_rat.user_map["u5"]
+        u5_items_idx = self.custom_rat.get_user_interactions(u5_idx)[:, 1].astype(int)
+        u5_items_str = self.custom_rat.item_map[u5_items_idx]
+        result_u5 = get_avg_pop(u5_items_str, counter_popularity)
         expected_u5 = (counter_popularity['i2'] + counter_popularity['i70']) / 2
         self.assertAlmostEqual(expected_u5, result_u5)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `clayrs-0.4.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py` & `clayrs-0.5.1/test/recsys/content_based_algorithm/centroid_vector/test_centroid_vector.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,146 +11,127 @@
     NotPredictionAlg, EmptyUserRatings
 from clayrs.recsys.content_based_algorithm.centroid_vector.similarities import CosineSimilarity
 from test import dir_test_files
 
 
 class TestCentroidVector(TestCase):
 
-    def setUp(self) -> None:
+    @classmethod
+    def setUpClass(cls) -> None:
         ratings = pd.DataFrame.from_records([
             ("A000", "tt0114576", 1, "54654675"),
             ("A000", "tt0112453", -0.2, "54654675"),
             ("A001", "tt0114576", 0.8, "54654675"),
             ("A001", "tt0112896", -0.4, "54654675"),
             ("A000", "tt0113041", 0.6, "54654675"),
             ("A002", "tt0112453", -0.2, "54654675"),
             ("A002", "tt0113497", 0.5, "54654675"),
             ("A003", "tt0112453", -0.8, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
-        self.ratings = Ratings.from_dataframe(ratings)
-
-        self.filter_list = ['tt0112641', 'tt0112760', 'tt0112896']
+        ratings = Ratings.from_dataframe(ratings)
+        ratings.item_map.append(['tt0112641', 'tt0112760'])
+        cls.ratings = ratings
 
         movies_dir = os.path.join(dir_test_files, 'complex_contents', 'movies_codified/')
 
-        self.available_loaded_items = LoadedContentsDict(movies_dir)
+        cls.filter_list = ['tt0112641', 'tt0112760', 'tt0112896']
+
+        cls.available_loaded_items = LoadedContentsDict(movies_dir)
 
     def test_predict(self):
         alg = CentroidVector({'Genre': ['embedding']}, CosineSimilarity(), threshold=0)
 
-        user_id = 'A000'
-        user_ratings = self.ratings.get_user_interactions(user_id)
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        user_idx = self.ratings.user_map['A000']
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
         # Will raise Exception since it's not a Score Prediction Algorithm
         with self.assertRaises(NotPredictionAlg):
-            alg.predict(user_ratings, self.available_loaded_items)
+            alg.predict_single_user(user_idx, self.ratings, self.available_loaded_items, self.filter_list)
 
     def test_rank_single_representation(self):
         # Single representation
         alg = CentroidVector({'Genre': ['embedding']}, CosineSimilarity(), threshold=0)
 
-        user_id = 'A000'
-        user_ratings = self.ratings.get_user_interactions(user_id)
+        user_idx = self.ratings.user_map.convert_str2int('A000')
 
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
-        # rank with filter_list
-        res_filtered = alg.rank(user_ratings, self.available_loaded_items, filter_list=self.filter_list)
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_filtered])
+        # unbounded rank
+        res_filtered = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items,
+                                            recs_number=None, filter_list=self.filter_list)
+        # convert int to string for comparison with filter list
+        item_ranked_set = set(self.ratings.item_map.convert_seq_int2str(res_filtered[:, 1].astype(int)))
         self.assertEqual(len(item_ranked_set), len(self.filter_list))
         self.assertCountEqual(item_ranked_set, self.filter_list)
 
-        res_all_unrated = alg.rank(user_ratings, self.available_loaded_items)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_all_unrated])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
-
-        # rank with n_recs specified
-        n_recs = 5
-        res_n_recs = alg.rank(user_ratings, self.available_loaded_items, n_recs)
+        # rank with recs_number specified
+        n_recs = 2
+        res_n_recs = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items, n_recs, self.filter_list)
         self.assertEqual(len(res_n_recs), n_recs)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_n_recs])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
 
     def test_rank_multiple_representations(self):
         # Multiple representations with auto threshold based on the mean ratings of the user
         alg = CentroidVector({'Plot': ['tfidf', 'embedding'],
                               "Genre": ['tfidf', 'embedding'],
                               'imdbRating': [0]}, CosineSimilarity())
 
-        user_id = 'A000'
-        user_ratings = self.ratings.get_user_interactions(user_id)
+        user_idx = self.ratings.user_map.convert_str2int('A000')
 
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
         # rank with filter_list
-        res_filtered = alg.rank(user_ratings, self.available_loaded_items, filter_list=self.filter_list)
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_filtered])
+        res_filtered = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items, recs_number=None,
+                                            filter_list=self.filter_list)
+        # convert int to string for comparison with filter list
+        item_ranked_set = set(self.ratings.item_map.convert_seq_int2str(res_filtered[:, 1].astype(int)))
         self.assertEqual(len(item_ranked_set), len(self.filter_list))
         self.assertCountEqual(item_ranked_set, self.filter_list)
 
-        # rank without filter_list
-        res_all_unrated = alg.rank(user_ratings, self.available_loaded_items)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_all_unrated])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
-
         # rank with n_recs specified
-        n_recs = 5
-        res_n_recs = alg.rank(user_ratings, self.available_loaded_items, n_recs)
+        n_recs = 2
+        res_n_recs = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items, n_recs,
+                                          filter_list=self.filter_list)
         self.assertEqual(len(res_n_recs), n_recs)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_predicted.item_id for interaction_predicted in res_n_recs])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
 
     def test_raise_errors(self):
         # Only negative available
         ratings = pd.DataFrame.from_records([
             ("A000", "tt0112281", -1, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
         ratings = Ratings.from_dataframe(ratings)
 
         alg = CentroidVector({'Plot': 'embedding'}, CosineSimilarity(), 0)
-        user_ratings = ratings.get_user_interactions('A000')
+        user_idx = ratings.user_map.convert_str2int('A000')
 
         with self.assertRaises(OnlyNegativeItems):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         # No Item available locally
         ratings = pd.DataFrame.from_records([
             ("A000", "non existent", 1, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
         ratings = Ratings.from_dataframe(ratings)
 
         alg = CentroidVector({'Plot': 'embedding'}, CosineSimilarity(), 0)
-        user_ratings = ratings.get_user_interactions('A000')
+        user_idx = ratings.user_map.convert_str2int('A000')
 
         with self.assertRaises(NoRatedItems):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         # User has no ratings
-        user_ratings = []
+        ratings = Ratings.from_list([('u1', 'i1', 2)], {'u1': 0}, {'i1': 0})
+        user_idx = 1
 
         alg = CentroidVector({'Plot': 'embedding'}, CosineSimilarity(), 0)
 
         with self.assertRaises(EmptyUserRatings):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         with self.assertRaises(EmptyUserRatings):
-            alg.rank(user_ratings, self.available_loaded_items)
+            alg.rank_single_user(user_idx, ratings, self.available_loaded_items, 2, self.filter_list)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `clayrs-0.4.1/test/recsys/content_based_algorithm/classifier/test_classifier.py` & `clayrs-0.5.1/test/recsys/content_based_algorithm/classifier/test_classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,170 +21,149 @@
                 test_func(*((self, classifier) + args), **kwargs)
 
     return wrapper
 
 
 class TestClassifierRecommender(TestCase):
 
-    def setUp(self) -> None:
+    @classmethod
+    def setUpClass(cls) -> None:
         ratings = pd.DataFrame.from_records([
             ("A000", "tt0112281", 0.5, "54654675"),
             ("A000", "tt0112302", 0.5, "54654675"),
             ("A001", "tt0114576", 0.8, "54654675"),
             ("A001", "tt0112896", -0.4, "54654675"),
             ("A000", "tt0112346", -0.5, "54654675"),
             ("A000", "tt0112453", -0.5, "54654675"),
             ("A002", "tt0112453", -0.2, "54654675"),
             ("A002", "tt0113497", 0.5, "54654675"),
             ("A003", "tt0112453", -0.8, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
-        self.ratings = Ratings.from_dataframe(ratings)
-
-        # tt0112281 is rated for A000 but let's suppose we want to know its rank
-        self.filter_list = ['tt0112281', 'tt0112760', 'tt0112896']
+        ratings = Ratings.from_dataframe(ratings)
+        ratings.item_map.append(['tt0112760'])
+        cls.ratings = ratings
 
         movies_dir = os.path.join(dir_test_files, 'complex_contents', 'movies_codified/')
+        # tt0112281 is rated for A000 but let's suppose we want to know its rank
+        cls.filter_list = ['tt0112281', 'tt0112760', 'tt0112896']
 
-        self.available_loaded_items = LoadedContentsDict(movies_dir)
+        cls.available_loaded_items = LoadedContentsDict(movies_dir)
 
         # IMPORTANT! If a new classifier is added, just add it to this list to test it
-        self.classifiers_list = [
+        cls.classifiers_list = [
             SkSVC(), SkKNN(), SkRandomForest(), SkLogisticRegression(),
             SkDecisionTree(), SkGaussianProcess()
         ]
 
     def test_predict(self):
         # Doesn't matter which classifier we chose
         alg = ClassifierRecommender({'Plot': ['tfidf']}, SkSVC(), threshold=0)
-        user_ratings = self.ratings.get_user_interactions("A000")
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        user_idx = self.ratings.user_map['A000']
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
         # Will raise Exception since it's not a Score Prediction Algorithm
         with self.assertRaises(NotPredictionAlg):
-            alg.predict(user_ratings, self.available_loaded_items)
+            alg.predict_single_user(user_idx, self.ratings, self.available_loaded_items, self.filter_list)
 
     @for_each_classifier
     def test_rank_single_representation(self, classifier: Classifier):
         clf = classifier
 
         # Single representation
         alg = ClassifierRecommender({'Plot': ['tfidf']}, clf, threshold=0)
 
-        user_ratings = self.ratings.get_user_interactions("A000")
-
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        user_idx = self.ratings.user_map['A000']
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
         # rank with filter_list
-        res_filtered = alg.rank(user_ratings, self.available_loaded_items, filter_list=self.filter_list)
-        item_ranked_set = set([interaction_filtered.item_id for interaction_filtered in res_filtered])
+        res_filtered = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items,
+                                            recs_number=None, filter_list=self.filter_list)
+        # convert int to string for comparison with filter list
+        item_ranked_set = set(self.ratings.item_map.convert_seq_int2str(res_filtered[:, 1].astype(int)))
         self.assertEqual(len(item_ranked_set), len(self.filter_list))
         self.assertCountEqual(item_ranked_set, self.filter_list)
 
-        # rank without filter_list
-        res_all_unrated = alg.rank(user_ratings, self.available_loaded_items)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_filtered.item_id for interaction_filtered in res_all_unrated])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
-
         # rank with n_recs specified
-        n_recs = 5
-        res_n_recs = alg.rank(user_ratings, self.available_loaded_items, n_recs)
+        n_recs = 2
+        res_n_recs = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items, n_recs, self.filter_list)
         self.assertEqual(len(res_n_recs), n_recs)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_nrecs.item_id for interaction_nrecs in res_n_recs])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
 
     @for_each_classifier
     def test_rank_multiple_representations(self, classifier: Classifier):
         clf = classifier
 
         # Multiple representations with auto threshold based on the mean ratings of the user
         alg = ClassifierRecommender({'Plot': ['tfidf', 'embedding'],
                                      'Genre': ['tfidf', 'embedding'],
                                      'imdbRating': [0]}, clf)
 
-        user_ratings = self.ratings.get_user_interactions("A000")
-
-        alg.process_rated(user_ratings, self.available_loaded_items)
-        alg.fit()
+        user_idx = self.ratings.user_map['A000']
+        alg.process_rated(user_idx, self.ratings, self.available_loaded_items)
+        alg.fit_single_user()
 
         # rank with filter_list
-        res_filtered = alg.rank(user_ratings, self.available_loaded_items, filter_list=self.filter_list)
-        item_ranked_set = set([interaction_filtered.item_id for interaction_filtered in res_filtered])
+        res_filtered = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items,
+                                            recs_number=None, filter_list=self.filter_list)
+        # convert int to string for comparison with filter list
+        item_ranked_set = set(self.ratings.item_map.convert_seq_int2str(res_filtered[:, 1].astype(int)))
         self.assertEqual(len(item_ranked_set), len(self.filter_list))
         self.assertCountEqual(item_ranked_set, self.filter_list)
 
-        # rank without filter_list
-        res_all_unrated = alg.rank(user_ratings, self.available_loaded_items)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_filtered.item_id for interaction_filtered in res_all_unrated])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
-
         # rank with n_recs specified
-        n_recs = 5
-        res_n_recs = alg.rank(user_ratings, self.available_loaded_items, n_recs)
+        n_recs = 2
+        res_n_recs = alg.rank_single_user(user_idx, self.ratings, self.available_loaded_items, n_recs, self.filter_list)
         self.assertEqual(len(res_n_recs), n_recs)
-        item_rated_set = set([interaction.item_id for interaction in user_ratings])
-        item_ranked_set = set([interaction_nrecs.item_id for interaction_nrecs in res_n_recs])
-        # We expect this to be empty, since the alg should rank only unrated items (unless in filter list)
-        rated_in_ranked = item_ranked_set.intersection(item_rated_set)
-        self.assertEqual(len(rated_in_ranked), 0)
 
     def test_raise_errors(self):
         # Only positive available
         ratings = pd.DataFrame.from_records([
             ("A000", "tt0112281", 1, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
         ratings = Ratings.from_dataframe(ratings)
 
         alg = ClassifierRecommender({'Plot': 'tfidf'}, SkKNN(), 0)
-        user_ratings = ratings.get_user_interactions("A000")
+        user_idx = self.ratings.user_map['A000']
 
         with self.assertRaises(OnlyPositiveItems):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         # Only negative available
         ratings = pd.DataFrame.from_records([
             ("A000", "tt0112281", -1, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
         ratings = Ratings.from_dataframe(ratings)
 
         alg = ClassifierRecommender({'Plot': 'tfidf'}, SkKNN(), 0)
-        user_ratings = ratings.get_user_interactions("A000")
+        user_idx = self.ratings.user_map['A000']
 
         with self.assertRaises(OnlyNegativeItems):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         # No Item avilable locally
         ratings = pd.DataFrame.from_records([
             ("A000", "non existent", 0.5, "54654675")],
             columns=["user_id", "item_id", "score", "timestamp"])
         ratings = Ratings.from_dataframe(ratings)
 
         alg = ClassifierRecommender({'Plot': 'tfidf'}, SkKNN(), 0)
-        user_ratings = ratings.get_user_interactions("A000")
+        user_idx = self.ratings.user_map['A000']
 
         with self.assertRaises(NoRatedItems):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         # User has no ratings
-        user_ratings = []
+        ratings = Ratings.from_list([('u1', 'i1', 2)], {'u1': 0}, {'i1': 0})
+        user_idx = 1
 
         alg = ClassifierRecommender({'Plot': 'tfidf'}, SkKNN(), 0)
 
         with self.assertRaises(EmptyUserRatings):
-            alg.process_rated(user_ratings, self.available_loaded_items)
+            alg.process_rated(user_idx, ratings, self.available_loaded_items)
 
         with self.assertRaises(EmptyUserRatings):
-            alg.rank(user_ratings, self.available_loaded_items)
+            alg.rank_single_user(user_idx, ratings, self.available_loaded_items, 2, self.filter_list)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `clayrs-0.4.1/test/recsys/content_based_algorithm/test_contents_loader.py` & `clayrs-0.5.1/test/recsys/content_based_algorithm/test_contents_loader.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py` & `clayrs-0.5.1/test/recsys/graph_based_algorithm/page_rank/test_page_rank.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py` & `clayrs-0.5.1/test/recsys/graph_based_algorithm/test_graph_based_algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from unittest import TestCase
 import pandas as pd
 
 from clayrs.content_analyzer import Ratings
-from clayrs.recsys.graph_based_algorithm.graph_based_algorithm import GraphBasedAlgorithm
 from clayrs.recsys.graphs.graph import ItemNode, UserNode, PropertyNode
 from clayrs.recsys.graphs.nx_implementation.nx_full_graphs import NXFullGraph
 
 from clayrs.recsys.graph_based_algorithm.page_rank.nx_page_rank import NXPageRank
 
 
 class TestGraphBasedAlgorithm(TestCase):
```

### Comparing `clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection.py` & `clayrs-0.5.1/test/recsys/graphs/feature_selection/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py` & `clayrs-0.5.1/test/recsys/graphs/feature_selection/test_feature_selection_alg.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py` & `clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_bipartite_graphs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 from unittest import TestCase
 
 import pandas as pd
 import os
 import lzma
 import pickle
 
@@ -17,16 +18,16 @@
                               'score': [0.8, 0.7, -0.4, 1.0, 0.4, 0.1, -0.3, 0.7]})
 rat = Ratings.from_dataframe(rat)
 
 rat_timestamp = pd.DataFrame.from_dict({'from_id': ["1", "1", "2", "2", "2", "3", "4", "4"],
                                         'to_id': ["tt0112281", "tt0112302", "tt0112281", "tt0112346",
                                                   "tt0112453", "tt0112453", "tt0112346", "tt0112453"],
                                         'score': [0.8, 0.7, -0.4, 1.0, 0.4, 0.1, -0.3, 0.7],
-                                        'timestamp': ['11111', '22222', '33333', '44444',
-                                                      '55555', '66666', '777777', '88888']
+                                        'timestamp': [11111, 22222, 33333, 44444,
+                                                      55555, 66666, 777777, 88888]
                                         })
 rat_timestamp = Ratings.from_dataframe(rat_timestamp, timestamp_column='timestamp')
 
 
 class TestNXBipartiteGraph(TestCase):
 
     def setUp(self) -> None:
@@ -37,46 +38,68 @@
 
         self.graph_timestamp: NXBipartiteGraph = NXBipartiteGraph(rat_timestamp)
 
         self.empty_graph: NXBipartiteGraph = NXBipartiteGraph()
 
     def test_graph_creation(self):
         # test that all nodes are added to the graph
-        for interaction in rat:
-            self.assertTrue(UserNode(interaction.user_id) in self.g.user_nodes)
-            self.assertTrue(ItemNode(interaction.item_id) in self.g.item_nodes)
 
-            link_data = self.g.get_link_data(UserNode(interaction.user_id), ItemNode(interaction.item_id))
+        user_column = rat.user_id_column
+        item_column = rat.item_id_column
+        score_column = rat.score_column
+
+        ratings_iterator = zip(user_column, item_column, score_column)
+
+        for interaction in ratings_iterator:
+            self.assertTrue(UserNode(interaction[0]) in self.g.user_nodes)
+            self.assertTrue(ItemNode(interaction[1]) in self.g.item_nodes)
+
+            link_data = self.g.get_link_data(UserNode(interaction[0]), ItemNode(interaction[1]))
             self.assertIsNotNone(link_data)
 
-            expected_data_link = {'weight': interaction.score}
-            result = self.g.get_link_data(UserNode(interaction.user_id), ItemNode(interaction.item_id))
+            expected_data_link = {'weight': interaction[2]}
+            result = self.g.get_link_data(UserNode(interaction[0]), ItemNode(interaction[1]))
 
             self.assertEqual(expected_data_link, result)
 
     def test_graph_creation_custom_label(self):
         # test that all nodes are added to the graph and the link between them has
         # a changed label
-        for interaction in rat:
-            self.assertTrue(UserNode(interaction.user_id) in self.graph_custom_label.user_nodes)
-            self.assertTrue(ItemNode(interaction.item_id) in self.graph_custom_label.item_nodes)
 
-            link_data = self.graph_custom_label.get_link_data(UserNode(interaction.user_id),
-                                                              ItemNode(interaction.item_id))
+        user_column = rat.user_id_column
+        item_column = rat.item_id_column
+        score_column = rat.score_column
+
+        ratings_iterator = zip(user_column, item_column, score_column)
+
+        for interaction in ratings_iterator:
+            self.assertTrue(UserNode(interaction[0]) in self.graph_custom_label.user_nodes)
+            self.assertTrue(ItemNode(interaction[1]) in self.graph_custom_label.item_nodes)
+
+            link_data = self.graph_custom_label.get_link_data(UserNode(interaction[0]),
+                                                              ItemNode(interaction[1]))
             self.assertIsNotNone(link_data)
 
-            expected_data_link = {'label': 'my_label', 'weight': interaction.score}
-            result = self.graph_custom_label.get_link_data(UserNode(interaction.user_id), ItemNode(interaction.item_id))
+            expected_data_link = {'label': 'my_label', 'weight': interaction[2]}
+            result = self.graph_custom_label.get_link_data(UserNode(interaction[0]), ItemNode(interaction[1]))
 
             self.assertEqual(expected_data_link, result)
 
     def test_graph_creation_w_timestamp(self):
-        for interaction in rat_timestamp:
-            expected_data_link = {'weight': interaction.score, 'timestamp': interaction.timestamp}
-            result = self.graph_timestamp.get_link_data(UserNode(interaction.user_id), ItemNode(interaction.item_id))
+
+        user_column = rat.user_id_column
+        item_column = rat.item_id_column
+        score_column = rat.score_column
+        timestamp_column = rat.timestamp_column
+
+        ratings_iterator = zip(user_column, item_column, score_column, timestamp_column)
+
+        for interaction in ratings_iterator:
+            expected_data_link = {'weight': interaction[2], 'timestamp': interaction[3]}
+            result = self.graph_timestamp.get_link_data(UserNode(interaction[0]), ItemNode(interaction[1]))
 
             self.assertEqual(expected_data_link, result)
 
     def test_graph_creation_empty(self):
         self.assertTrue(len(self.empty_graph.user_nodes) == 0)
         self.assertTrue(len(self.empty_graph.item_nodes) == 0)
 
@@ -324,37 +347,14 @@
 
         # remove not existent node
         user_nodes_before_removal = self.g.user_nodes
         self.g.remove_node(UserNode("not existent"))
         user_nodes_after_removal = self.g.user_nodes
         self.assertEqual(user_nodes_before_removal, user_nodes_after_removal)
 
-    #
-    # def test_convert_to_dataframe(self):
-    #     converted_df = self.g.convert_to_dataframe()
-    #     self.assertNotIn('label', converted_df.columns)
-    #     for user, item in zip(converted_df['from_id'], converted_df['to_id']):
-    #         self.assertIsInstance(user, Node)
-    #         self.assertIsInstance(item, Node)
-    #
-    #     result = np.sort(converted_df, axis=0)
-    #     expected = np.sort(self.df, axis=0)
-    #     self.assertTrue(np.array_equal(expected, result))
-    #
-    #     converted_df = self.g.convert_to_dataframe(only_values=True, with_label=True)
-    #     self.assertIn('label', converted_df.columns)
-    #     for user, item in zip(converted_df['from_id'], converted_df['to_id']):
-    #         self.assertNotIsInstance(user, Node)
-    #         self.assertNotIsInstance(item, Node)
-    #
-    #     converted_df = converted_df[['from_id', 'to_id', 'score']]
-    #     result = np.sort(converted_df, axis=0)
-    #     expected = np.sort(self.df, axis=0)
-    #     self.assertTrue(np.array_equal(expected, result))
-    #
     def test_copy(self):
         copy = self.g.copy()
         self.assertTrue(copy == self.g)
 
         copy.add_node(UserNode('prova'))
 
         self.assertFalse(copy == self.g)
@@ -363,7 +363,9 @@
 
         self.g.serialize('./test_serialize', 'test_graph')
 
         with lzma.open(os.path.join('./test_serialize/test_graph.xz'), 'rb') as graph_file:
             graph = pickle.load(graph_file)
 
         self.assertEqual(self.g, graph)
+
+        shutil.rmtree("test_serialize")
```

### Comparing `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py` & `clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_full_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py` & `clayrs-0.5.1/test/recsys/graphs/test_networkx_implementation/test_nx_tripartite_graphs.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/recsys/test_experiment.py` & `clayrs-0.5.1/test/recsys/test_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,18 @@
         # check dirs have been created
         self.assertTrue(os.path.isdir("my_experiment"))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "CentroidVector_1")))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "ClassifierRecommender_1")))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "ClassifierRecommender_2")))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "LinearPredictor_1")))
 
+        # check user_map and item_map have been created
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "user_map.yml")))
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "item_map.yml")))
+
         # check train test splits have been created
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split1.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split1.csv")))
 
         # check rank created for centroid vector 1
@@ -203,14 +207,18 @@
         # check dirs have been created
         self.assertTrue(os.path.isdir("my_experiment"))
         self.assertFalse(os.path.isdir(os.path.join("my_experiment", "CentroidVector_1")))
         self.assertFalse(os.path.isdir(os.path.join("my_experiment", "ClassifierRecommender_1")))
         self.assertFalse(os.path.isdir(os.path.join("my_experiment", "ClassifierRecommender_2")))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "LinearPredictor_1")))
 
+        # check user_map and item_map have been created
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "user_map.yml")))
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "item_map.yml")))
+
         # check train test splits have been created
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split1.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split1.csv")))
 
         # check predict created for linear predictor
@@ -242,20 +250,22 @@
                                      items_directory=items_dir,
                                      output_folder="my_experiment")
 
         cbe.predict(num_cpus=num_cpus)
 
         self.assertTrue(os.path.isdir("my_experiment"))
 
-        # since no algorithm is a score prediction one, only train and test split will be present
+        # since no algorithm is a score prediction one, only train, test split and item and user map will be present
         # and no other thing
         contents_directory = os.listdir("my_experiment")
 
         contents_directory.remove("HoldOutPartitioning_train_split0.csv")
         contents_directory.remove("HoldOutPartitioning_test_split0.csv")
+        contents_directory.remove("user_map.yml")
+        contents_directory.remove("item_map.yml")
 
         self.assertTrue(len(contents_directory) == 0)
 
     def test_predict_raise_error(self):
         cbe = ContentBasedExperiment(self.rat,
                                      partitioning_technique=HoldOutPartitioning(random_state=42),
                                      algorithm_list=[CentroidVector({'Plot': 0}, similarity=CosineSimilarity()),
@@ -292,14 +302,18 @@
         self.gbe.rank(num_cpus=num_cpus)
 
         # check dirs have been created
         self.assertTrue(os.path.isdir("my_experiment"))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "NXPageRank_1")))
         self.assertTrue(os.path.isdir(os.path.join("my_experiment", "NXPageRank_2")))
 
+        # check user_map and item_map have been created
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "user_map.yml")))
+        self.assertTrue(os.path.isfile(os.path.join("my_experiment", "item_map.yml")))
+
         # check train test splits have been created
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split0.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_test_split1.csv")))
         self.assertTrue(os.path.isfile(os.path.join("my_experiment", "KFoldPartitioning_train_split1.csv")))
 
         # check rank created for nx page rank 1
@@ -331,22 +345,24 @@
 
     def test_no_one_predictor(self):
 
         self.gbe.predict(num_cpus=num_cpus)
 
         self.assertTrue(os.path.isdir("my_experiment"))
 
-        # since no algorithm is a score prediction one, only train and test split will be present
+        # since no algorithm is a score prediction one, only train, test split and item and user map will be present
         # and no other thing
         contents_directory = os.listdir("my_experiment")
 
         contents_directory.remove("KFoldPartitioning_train_split0.csv")
         contents_directory.remove("KFoldPartitioning_test_split0.csv")
         contents_directory.remove("KFoldPartitioning_train_split1.csv")
         contents_directory.remove("KFoldPartitioning_test_split1.csv")
+        contents_directory.remove("user_map.yml")
+        contents_directory.remove("item_map.yml")
 
         self.assertTrue(len(contents_directory) == 0)
 
     def test_predict_raise_error(self):
         with self.assertRaises(NotPredictionAlg):
             self.gbe.predict(num_cpus=num_cpus, skip_alg_error=False)
```

### Comparing `clayrs-0.4.1/test/recsys/test_methodology.py` & `clayrs-0.5.1/test/recsys/test_methodology.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,38 +35,55 @@
 test2 = pd.DataFrame.from_records([
     ("001", "tt0112281", 3.5, "54654675"),
     ("001", "tt0112302", 4.5, "54654675"),
     ("002", "tt0112346", 4, "54654675"),
     ("003", "tt0112453", 2, "54654675")],
     columns=["from_id", "to_id", "score", "timestamp"])
 
-train1_rat = Ratings.from_dataframe(train1)
-test1_rat = Ratings.from_dataframe(test1)
-train2_rat = Ratings.from_dataframe(train2)
-test2_rat = Ratings.from_dataframe(test2)
+# we create manually the mapping since we want a global mapping containing train and test items
+item1_map = {}
+for item_id in train1[["to_id"]].append(test1[["to_id"]])["to_id"]:
+    if item_id not in item1_map:
+        item1_map[item_id] = len(item1_map)
 
+item2_map = {}
+for item_id in train2[["to_id"]].append(test2[["to_id"]])["to_id"]:
+    if item_id not in item2_map:
+        item2_map[item_id] = len(item2_map)
 
-def _unpack_result_w_iter(result_list_w_iter):
-    result_list = []
-    for result_w_iter in result_list_w_iter:
-        result_unpacked = {}
-        for user, items_iterator in result_w_iter.items():
-            result_unpacked[user] = set(items_iterator)
+train1_rat = Ratings.from_dataframe(train1, item_map=item1_map)
+test1_rat = Ratings.from_dataframe(test1, item_map=item1_map)
+train2_rat = Ratings.from_dataframe(train2, item_map=item2_map)
+test2_rat = Ratings.from_dataframe(test2, item_map=item2_map)
 
-        result_list.append(result_unpacked)
 
-    return result_list
+class TestMethodology(TestCase):
 
+    def assertDictListCountEqual(self, dict1, dict2):
 
-class TestTestRatingsMethodology(TestCase):
+        user_list_dict1 = list(dict1.keys())
+        user_list_dict2 = list(dict2.keys())
+        self.assertCountEqual(user_list_dict1, user_list_dict2)
+
+        for user in user_list_dict1:
+            self.assertCountEqual(dict1[user], dict2[user])
+
+
+class TestTestRatingsMethodology(TestMethodology):
 
     def test_filter_all(self):
 
-        result_list = [TestRatingsMethodology().filter_all(train1_rat, test1_rat),
-                       TestRatingsMethodology().filter_all(train2_rat, test2_rat)]
+        ratings_1 = TestRatingsMethodology()
+        ratings_2 = TestRatingsMethodology()
+
+        ratings_1.setup(train1_rat, test1_rat)
+        ratings_2.setup(train2_rat, test2_rat)
+
+        result_list = [ratings_1.filter_all(train1_rat, test1_rat, ids_as_str=True),
+                       ratings_2.filter_all(train2_rat, test2_rat, ids_as_str=True)]
 
         # for every user get the items in its test_set1
         expected_list = [test1[['from_id', 'to_id']], test2[['from_id', 'to_id']]]
 
         self.assertTrue(len(expected_list), len(result_list))
 
         for expected, result in zip(expected_list, result_list):
@@ -76,16 +93,22 @@
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_filter_all_only_greater_eq(self):
 
-        result_list = [TestRatingsMethodology(only_greater_eq=3).filter_all(train1_rat, test1_rat),
-                       TestRatingsMethodology(only_greater_eq=3).filter_all(train2_rat, test2_rat)]
+        ratings_1 = TestRatingsMethodology(only_greater_eq=3)
+        ratings_2 = TestRatingsMethodology(only_greater_eq=3)
+
+        ratings_1.setup(train1_rat, test1_rat)
+        ratings_2.setup(train2_rat, test2_rat)
+
+        result_list = [ratings_1.filter_all(train1_rat, test1_rat, ids_as_str=True),
+                       ratings_2.filter_all(train2_rat, test2_rat, ids_as_str=True)]
 
         # for every user get the items in its test_set1 with score >= 3
         expected_split_1 = pd.DataFrame({
             'from_id': ['002',
                         '003', '003'],
             'to_id': ["tt0112641",
                       "tt0113041", "tt0112281"]
@@ -109,40 +132,57 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_result_as_dict_iter(self):
-        result_list_iter = [TestRatingsMethodology().filter_all(train1_rat, test1_rat, result_as_iter_dict=True),
-                            TestRatingsMethodology().filter_all(train2_rat, test2_rat, result_as_iter_dict=True)]
+
+        ratings_1 = TestRatingsMethodology()
+        ratings_2 = TestRatingsMethodology()
+
+        ratings_1.setup(train1_rat, test1_rat)
+        ratings_2.setup(train2_rat, test2_rat)
+
+        result_list = [ratings_1.filter_all(train1_rat, test1_rat, result_as_dict=True, ids_as_str=True),
+                       ratings_2.filter_all(train2_rat, test2_rat, result_as_dict=True, ids_as_str=True)]
+
+        # convert numpy to list for dict equal assertion
+        result_list[0] = dict((user, list(filter_list)) for user, filter_list in result_list[0].items())
+        result_list[1] = dict((user, list(filter_list)) for user, filter_list in result_list[1].items())
 
         # for every user get the items in its test_set1
-        expected_list = [{'001': {"tt0112641", "tt0112760"},
-                          '002': {"tt0112641", "tt0112896"},
-                          '003': {"tt0113041", "tt0112281"}},
-                         {'001': {"tt0112281", "tt0112302"},
-                          '002': {"tt0112346"},
-                          '003': {"tt0112453"}}
+        expected_list = [{'001': ["tt0112641", "tt0112760"],
+                          '002': ["tt0112641", "tt0112896"],
+                          '003': ["tt0113041", "tt0112281"]},
+
+                         {'001': ["tt0112281", "tt0112302"],
+                          '002': ["tt0112346"],
+                          '003': ["tt0112453"]}
                          ]
 
-        result_list = _unpack_result_w_iter(result_list_iter)
-
         self.assertTrue(len(expected_list), len(result_list))
 
-        self.assertCountEqual(result_list, expected_list)
+        self.assertDictListCountEqual(expected_list[0], result_list[0])
+        self.assertDictListCountEqual(expected_list[1], result_list[1])
 
 
 # poor choice of words sadly
-class TestTestItemsMethodology(TestCase):
+class TestTestItemsMethodology(TestMethodology):
 
     def test_filter_all(self):
 
-        result_list = [TestItemsMethodology().filter_all(train1_rat, test1_rat),
-                       TestItemsMethodology().filter_all(train2_rat, test2_rat)]
+        test_1 = TestItemsMethodology()
+        test_2 = TestItemsMethodology()
+
+        test_1.setup(train1_rat, test1_rat)
+        test_2.setup(train2_rat, test2_rat)
+
+        result_list = [test_1.filter_all(train1_rat, test1_rat, ids_as_str=True),
+                       test_2.filter_all(train2_rat, test2_rat, ids_as_str=True)]
 
         # for every user get the all items present in test_set1 except the items
         # present in the training_set1 of the user
         expected_split_1 = pd.DataFrame({
             'from_id': ['001', '001', '001', '001',
                         '002', '002', '002', '002', '002',
                         '003', '003', '003', '003', '003'],
@@ -172,16 +212,23 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_filter_all_only_greater_eq(self):
-        result_list = [TestItemsMethodology(only_greater_eq=3).filter_all(train1_rat, test1_rat),
-                       TestItemsMethodology(only_greater_eq=3).filter_all(train2_rat, test2_rat)]
+
+        test_1 = TestItemsMethodology(only_greater_eq=3)
+        test_2 = TestItemsMethodology(only_greater_eq=3)
+
+        test_1.setup(train1_rat, test1_rat)
+        test_2.setup(train2_rat, test2_rat)
+
+        result_list = [test_1.filter_all(train1_rat, test1_rat, ids_as_str=True),
+                       test_2.filter_all(train2_rat, test2_rat, ids_as_str=True)]
 
         # for every user get the all items present in test_set1 with score >= 3 except the items
         # present in the training_set1 of the user
         expected_split_1 = pd.DataFrame({
             'from_id': ['001', '001',
                         '002', '002', '002',
                         '003', '003', '003'],
@@ -211,44 +258,60 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_result_as_dict(self):
-        result_list_iter = [TestItemsMethodology().filter_all(train1_rat, test1_rat, result_as_iter_dict=True),
-                            TestItemsMethodology().filter_all(train2_rat, test2_rat, result_as_iter_dict=True)]
+
+        test_1 = TestItemsMethodology()
+        test_2 = TestItemsMethodology()
+
+        test_1.setup(train1_rat, test1_rat)
+        test_2.setup(train2_rat, test2_rat)
+
+        result_list = [test_1.filter_all(train1_rat, test1_rat, result_as_dict=True),
+                       test_2.filter_all(train2_rat, test2_rat, result_as_dict=True)]
+
+        # convert numpy to list for dict equal assertion
+        result_list[0] = dict((user, list(filter_list)) for user, filter_list in result_list[0].items())
+        result_list[1] = dict((user, list(filter_list)) for user, filter_list in result_list[1].items())
 
         expected_split_1 = {
             '001': ["tt0112641", "tt0112760", "tt0112896", "tt0113041"],
             '002': ["tt0112641", "tt0112760", "tt0112896", "tt0113041", "tt0112281"],
             '003': ["tt0112641", "tt0112760", "tt0112896", "tt0113041", "tt0112281"]
         }
 
         expected_split_2 = {
             '001': ["tt0112281", "tt0112302", "tt0112346", "tt0112453"],
             '002': ["tt0112281", "tt0112302", "tt0112346", "tt0112453"],
             '003': ["tt0112302", "tt0112346", "tt0112453"]
         }
 
         expected_list = [expected_split_1, expected_split_2]
-        result_list = _unpack_result_w_iter(result_list_iter)
 
         self.assertTrue(len(expected_list), len(result_list))
 
-        self.assertCountEqual(expected_list[0], result_list[0])
-        self.assertCountEqual(expected_list[1], result_list[1])
+        self.assertDictListCountEqual(expected_list[0], result_list[0])
+        self.assertDictListCountEqual(expected_list[1], result_list[1])
 
 
-class TestTrainingItemsMethodology(TestCase):
+class TestTrainingItemsMethodology(TestMethodology):
 
     def test_filter_all(self):
 
-        result_list = [TrainingItemsMethodology().filter_all(train1_rat, test1_rat),
-                       TrainingItemsMethodology().filter_all(train2_rat, test2_rat)]
+        train_1 = TrainingItemsMethodology()
+        train_2 = TrainingItemsMethodology()
+
+        train_1.setup(train1_rat, test1_rat)
+        train_2.setup(train2_rat, test2_rat)
+
+        result_list = [train_1.filter_all(train1_rat, test1_rat, ids_as_str=True),
+                       train_2.filter_all(train2_rat, test2_rat, ids_as_str=True)]
 
         # for every user get the all items present in training_set1 except the items
         # present in the training_set1 of the user
         expected_split_1 = pd.DataFrame({
             'from_id': ['001', '001',
                         '002', '002', '002',
                         '003', '003', '003'],
@@ -278,16 +341,23 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_filter_all_only_greater_eq(self):
-        result_list = [TrainingItemsMethodology(only_greater_eq=3).filter_all(train1_rat, test1_rat),
-                       TrainingItemsMethodology(only_greater_eq=3).filter_all(train2_rat, test2_rat)]
+
+        train_1 = TrainingItemsMethodology(only_greater_eq=3)
+        train_2 = TrainingItemsMethodology(only_greater_eq=3)
+
+        train_1.setup(train1_rat, test1_rat)
+        train_2.setup(train2_rat, test2_rat)
+
+        result_list = [train_1.filter_all(train1_rat, test1_rat),
+                       train_2.filter_all(train2_rat, test2_rat)]
 
         # for every user get the all items present in training_set1 with score >= 3 except the items
         # present in the training_set1 of the user
         expected_split_1 = pd.DataFrame({
             'from_id': ['001',
                         '002', '002',
                         '003', '003', '003'],
@@ -317,71 +387,87 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_result_as_dict(self):
-        result_list_iter = [TrainingItemsMethodology().filter_all(train1_rat, test1_rat, result_as_iter_dict=True),
-                            TrainingItemsMethodology().filter_all(train2_rat, test2_rat, result_as_iter_dict=True)]
+
+        train_1 = TrainingItemsMethodology()
+        train_2 = TrainingItemsMethodology()
+
+        train_1.setup(train1_rat, test1_rat)
+        train_2.setup(train2_rat, test2_rat)
+
+        result_list = [train_1.filter_all(train1_rat, test1_rat, result_as_dict=True),
+                       train_2.filter_all(train2_rat, test2_rat, result_as_dict=True)]
+
+        # convert numpy to list for dict equal assertion
+        result_list[0] = dict((user, list(filter_list)) for user, filter_list in result_list[0].items())
+        result_list[1] = dict((user, list(filter_list)) for user, filter_list in result_list[1].items())
 
         expected_split_1 = {
             '001': ["tt0112346", "tt0112453"],
             '002': ["tt0112281", "tt0112302", "tt0112453"],
             '003': ["tt0112281", "tt0112302", "tt0112346"]
         }
 
         expected_split_2 = {
             '001': ["tt0112896", "tt0113041", "tt0112281"],
             '002': ["tt0112760", "tt0113041", "tt0112281"],
             '003': ["tt0112641", "tt0112760", "tt0112896"]
         }
 
         expected_list = [expected_split_1, expected_split_2]
-        result_list = _unpack_result_w_iter(result_list_iter)
 
         self.assertTrue(len(expected_list), len(result_list))
 
-        self.assertCountEqual(expected_list[0], result_list[0])
-        self.assertCountEqual(expected_list[1], result_list[1])
+        self.assertDictListCountEqual(expected_list[0], result_list[0])
+        self.assertDictListCountEqual(expected_list[1], result_list[1])
 
 
-class TestAllItemsMethodology(TestCase):
+class TestAllItemsMethodology(TestMethodology):
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.all_items = ["tt0112281",
                          "tt0112302",
                          "tt0112346",
                          "tt0112453",
-                         "iall1",
-                         "iall2",
-                         "iall3",
-                         "iall4"]
+                         "inew1",
+                         "inew2",
+                         "inew3",
+                         "inew4"]
 
     def test_filter_all(self):
-        result_list = [AllItemsMethodology(set(self.all_items)).filter_all(train1_rat, test1_rat),
-                       AllItemsMethodology(set(self.all_items)).filter_all(train2_rat, test2_rat)]
+        all_1 = AllItemsMethodology()
+        all_2 = AllItemsMethodology()
+
+        all_1.setup(train1_rat, test1_rat)
+        all_2.setup(train2_rat, test2_rat)
+
+        result_list = [all_1.filter_all(train1_rat, test1_rat),
+                       all_2.filter_all(train2_rat, test2_rat)]
 
         expected_split_1 = pd.DataFrame({
             'from_id': ["001", "001", "001", "001", "001", "001",
                         "002", "002", "002", "002", "002", "002", "002",
                         "003", "003", "003", "003", "003", "003", "003"],
-            'to_id': ["tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4",
-                      "tt0112281", "tt0112302", "tt0112453", "iall1", "iall2", "iall3", "iall4",
-                      "tt0112281", "tt0112302", "tt0112346", "iall1", "iall2", "iall3", "iall4", ]
+            'to_id': ["tt0112346", "tt0112453", "tt0112641", "tt0112760", "tt0112896", "tt0113041",
+                      "tt0112281", "tt0112302", "tt0112453", "tt0112641", "tt0112760", "tt0112896", "tt0113041",
+                      "tt0112281", "tt0112302", "tt0112346", "tt0112641", "tt0112760", "tt0112896", "tt0113041"]
         })
 
         expected_split_2 = pd.DataFrame({
-            'from_id': ["001", "001", "001", "001", "001", "001", "001", "001",
-                        "002", "002", "002", "002", "002", "002", "002", "002",
-                        "003", "003", "003", "003", "003", "003", "003"],
-            'to_id': ["tt0112281", "tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4",
-                      "tt0112281", "tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4",
-                      "tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4"]
+            'from_id': ["001", "001", "001", "001", "001", "001",
+                        "002", "002", "002", "002", "002", "002",
+                        "003", "003", "003", "003", "003", "003"],
+            'to_id': ["tt0112896", "tt0113041", "tt0112281", "tt0112302", "tt0112346", "tt0112453",
+                      "tt0112760", "tt0113041", "tt0112281", "tt0112302", "tt0112346", "tt0112453",
+                      "tt0112641", "tt0112760", "tt0112896", "tt0112302", "tt0112346", "tt0112453"]
         })
 
         expected_list = [expected_split_1, expected_split_2]
 
         self.assertTrue(len(expected_list), len(result_list))
 
         for expected, result in zip(expected_list, result_list):
@@ -390,35 +476,75 @@
 
             result = np.array(result)
             result.sort(axis=0)
 
             self.assertTrue(np.array_equal(expected, result))
 
     def test_result_as_dict(self):
-        result_list_iter = [AllItemsMethodology(set(self.all_items)).filter_all(train1_rat, test1_rat,
-                                                                                result_as_iter_dict=True),
-                            AllItemsMethodology(set(self.all_items)).filter_all(train2_rat, test2_rat,
-                                                                                result_as_iter_dict=True)]
+        all_1 = AllItemsMethodology()
+        all_2 = AllItemsMethodology()
+
+        all_1.setup(train1_rat, test1_rat)
+        all_2.setup(train2_rat, test2_rat)
+
+        result_list = [all_1.filter_all(train1_rat, test1_rat, result_as_dict=True),
+                       all_2.filter_all(train2_rat, test2_rat, result_as_dict=True)]
+
+        # convert numpy to list for dict equal assertion
+        result_list[0] = dict((user, list(filter_list)) for user, filter_list in result_list[0].items())
+        result_list[1] = dict((user, list(filter_list)) for user, filter_list in result_list[1].items())
+
+        expected_split_1 = {
+            "001": ["tt0112346", "tt0112453", "tt0112641", "tt0112760", "tt0112896", "tt0113041"],
+            "002": ["tt0112281", "tt0112302", "tt0112453", "tt0112641", "tt0112760", "tt0112896", "tt0113041"],
+            "003": ["tt0112281", "tt0112302", "tt0112346", "tt0112641", "tt0112760", "tt0112896", "tt0113041"]
+        }
+
+        expected_split_2 = {
+            "001": ["tt0112896", "tt0113041", "tt0112281", "tt0112302", "tt0112346", "tt0112453"],
+            "002": ["tt0112760", "tt0113041", "tt0112281", "tt0112302", "tt0112346", "tt0112453"],
+            "003": ["tt0112641", "tt0112760", "tt0112896", "tt0112302", "tt0112346", "tt0112453"]
+        }
+
+        expected_list = [expected_split_1, expected_split_2]
+
+        self.assertTrue(len(expected_list), len(result_list))
+
+        self.assertDictListCountEqual(expected_list[0], result_list[0])
+        self.assertDictListCountEqual(expected_list[1], result_list[1])
+
+    def test_items_new(self):
+        all_1 = AllItemsMethodology(items_list=self.all_items)
+        all_2 = AllItemsMethodology(items_list=self.all_items)
+
+        all_1.setup(train1_rat, test1_rat)
+        all_2.setup(train2_rat, test2_rat)
+
+        result_list = [all_1.filter_all(train1_rat, test1_rat, result_as_dict=True),
+                       all_2.filter_all(train2_rat, test2_rat, result_as_dict=True)]
+
+        # convert numpy to list for dict equal assertion
+        result_list[0] = dict((user, list(filter_list)) for user, filter_list in result_list[0].items())
+        result_list[1] = dict((user, list(filter_list)) for user, filter_list in result_list[1].items())
 
         expected_split_1 = {
-            '001': ["tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4"],
-            '002': ["tt0112281", "tt0112302", "tt0112453", "iall1", "iall2", "iall3", "iall4"],
-            '003': ["tt0112281", "tt0112302", "tt0112346", "iall1", "iall2", "iall3", "iall4"]
+            '001': ["tt0112346", "tt0112453", "inew1", "inew2", "inew3", "inew4"],
+            '002': ["tt0112281", "tt0112302", "tt0112453", "inew1", "inew2", "inew3", "inew4"],
+            '003': ["tt0112281", "tt0112302", "tt0112346", "inew1", "inew2", "inew3", "inew4"]
         }
 
         expected_split_2 = {
-            '001': ["tt0112281", "tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4", ],
-            '002': ["tt0112281", "tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4", ],
-            '003': ["tt0112302", "tt0112346", "tt0112453", "iall1", "iall2", "iall3", "iall4"]
+            '001': ["tt0112281", "tt0112302", "tt0112346", "tt0112453", "inew1", "inew2", "inew3", "inew4"],
+            '002': ["tt0112281", "tt0112302", "tt0112346", "tt0112453", "inew1", "inew2", "inew3", "inew4"],
+            '003': ["tt0112302", "tt0112346", "tt0112453", "inew1", "inew2", "inew3", "inew4"]
         }
 
         expected_list = [expected_split_1, expected_split_2]
-        result_list = _unpack_result_w_iter(result_list_iter)
 
         self.assertTrue(len(expected_list), len(result_list))
 
-        self.assertCountEqual(expected_list[0], result_list[0])
-        self.assertCountEqual(expected_list[1], result_list[1])
+        self.assertDictListCountEqual(expected_list[0], result_list[0])
+        self.assertDictListCountEqual(expected_list[1], result_list[1])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `clayrs-0.4.1/test/recsys/test_recsys.py` & `clayrs-0.5.1/test/recsys/visual_based_algorithm/vbpr/test_vbpr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,325 +1,307 @@
 import os
+import unittest
 from unittest import TestCase
+
+import numpy as np
 import pandas as pd
+import torch
 
 from clayrs.content_analyzer import Ratings
-from clayrs.recsys import LinearPredictor, SkLinearRegression, TrainingItemsMethodology
-from clayrs.recsys.content_based_algorithm.classifier.classifiers import SkSVC
-from clayrs.recsys.recsys import GraphBasedRS, ContentBasedRS
-from clayrs.recsys.content_based_algorithm.classifier.classifier_recommender import ClassifierRecommender
-from clayrs.recsys.content_based_algorithm.exceptions import NotPredictionAlg, NotFittedAlg
-from clayrs.recsys.graph_based_algorithm.page_rank.nx_page_rank import NXPageRank
-from clayrs.recsys.graphs import NXFullGraph
-
+from clayrs.recsys import TestRatingsMethodology
+from clayrs.recsys.content_based_algorithm.exceptions import NotPredictionAlg
+from clayrs.recsys.visual_based_algorithm.vbpr.vbpr_algorithm import VBPR
 from test import dir_test_files
 
 train_ratings = pd.DataFrame.from_records([
     ("A000", "tt0114576", 5, "54654675"),
     ("A001", "tt0114576", 3, "54654675"),
     ("A001", "tt0112896", 1, "54654675"),
     ("A000", "tt0113041", 1, "54654675"),
     ("A002", "tt0112453", 2, "54654675"),
+    ("A000", "non_existent", 2, "54654675"),
     ("A002", "tt0113497", 4, "54654675"),
     ("A003", "tt0112453", 1, "54654675"),
     ("A003", "tt0113497", 4, "54654675")],
     columns=["from_id", "to_id", "score", "timestamp"])
-train_ratings = Ratings.from_dataframe(train_ratings)
-
-# No locally available items for A000
-train_ratings_some_missing = pd.DataFrame.from_records([
-    ("A000", "not_existent1", 5, "54654675"),
-    ("A001", "tt0114576", 3, "54654675"),
-    ("A001", "tt0112896", 1, "54654675"),
-    ("A000", "not_existent2", 5, "54654675")],
-    columns=["from_id", "to_id", "score", "timestamp"])
-train_ratings_some_missing = Ratings.from_dataframe(train_ratings_some_missing)
 
 test_ratings = pd.DataFrame.from_records([
     ("A000", "tt0114388", None),
     ("A000", "tt0112302", None),
     ("A001", "tt0113189", None),
     ("A001", "tt0113228", None),
     ("A002", "tt0114319", None),
     ("A002", "tt0114709", None),
     ("A003", "tt0114885", None)],
     columns=["from_id", "to_id", "score"])
-test_ratings = Ratings.from_dataframe(test_ratings)
 
+# we create manually the mapping since we want a global mapping containing train and test items
+user_map = {}
+users_train = train_ratings["from_id"]
+users_test = test_ratings["from_id"]
+
+all_users = users_train.append(users_test)
+for user_id in all_users:
+    if user_id not in user_map:
+        user_map[user_id] = len(user_map)
+
+item_map = {}
 
-# Each of the cbrs algorithm has its own class tests, so we just take
-# one cbrs alg as example. The behaviour is the same for all cbrs alg
-class TestContentBasedRS(TestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        cls.movies_multiple = os.path.join(dir_test_files, 'complex_contents', 'movies_codified/')
-
-    def test_fit(self):
-        # Test fit with cbrs algorithm
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
-
-        cbrs.fit(num_cpus=1)
-
-        # For the following user the algorithm could be fit
-        self.assertIsNotNone(cbrs._user_fit_dic.get("A000"))
-        self.assertIsNotNone(cbrs._user_fit_dic.get("A001"))
-        self.assertIsNotNone(cbrs._user_fit_dic.get("A002"))
-        self.assertIsNotNone(cbrs._user_fit_dic.get("A003"))
-
-        # Test fit with the cbrs algorithm
-        # For user A000 no items available locally, so the alg will not be fit for it
-        cbrs_missing = ContentBasedRS(alg, train_ratings_some_missing, self.movies_multiple)
-
-        cbrs_missing.fit(num_cpus=1)
-
-        # For user A000 the alg could not be fit, but it could for A001
-        self.assertIsNone(cbrs_missing._user_fit_dic.get("A000"))
-        self.assertIsNotNone(cbrs_missing._user_fit_dic.get("A001"))
-
-    def test_raise_error_without_fit(self):
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
-
-        with self.assertRaises(NotFittedAlg):
-            cbrs.rank(train_ratings, num_cpus=1)
-
-        with self.assertRaises(NotFittedAlg):
-            cbrs.predict(train_ratings, num_cpus=1)
-
-    def test_rank(self):
-        # Test fit with the cbrs algorithm
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
-
-        # we must fit the algorithm in order to rank
-        cbrs.fit(num_cpus=1)
-
-        # Test ranking with the cbrs algorithm on specified items
-        result_rank_filtered = cbrs.rank(test_ratings, num_cpus=1)
-        self.assertEqual(len(result_rank_filtered), len(test_ratings))
-
-        # Test ranking with the cbrs algorithm on all available unseen items
-        result_rank_all = cbrs.rank(test_ratings, methodology=None, num_cpus=1)
-        self.assertTrue(len(result_rank_all) != 0)
-
-        # Test top-n ranking with the cbrs algorithm for only some users
-        result_rank_numbered = cbrs.rank(test_ratings, n_recs=2, methodology=None, user_id_list=["A000", "A003"],
-                                         num_cpus=1)
-        self.assertEqual(set(result_rank_numbered.user_id_column), {"A000", "A003"})
-        for user in {"A000", "A003"}:
-            result_single = result_rank_numbered.get_user_interactions(user)
-            self.assertTrue(len(result_single) == 2)
-
-        # Test ranking with alternative methodology
-        result_different_meth = cbrs.rank(test_ratings, methodology=TrainingItemsMethodology(), num_cpus=1)
-        for user in set(test_ratings.user_id_column):
-            result_single = result_different_meth.get_user_interactions(user)
-            result_single_items = set([result_interaction.item_id for result_interaction in result_single])
-            items_already_seen_user = set([train_interaction.item_id
-                                           for train_interaction in train_ratings.get_user_interactions(user)])
-            items_expected_rank = set([train_interaction.item_id
-                                       for train_interaction in train_ratings
-                                       if train_interaction.item_id not in items_already_seen_user])
-
-            self.assertEqual(items_expected_rank, result_single_items)
-
-        # Test algorithm not fitted
-        cbrs = ContentBasedRS(alg, train_ratings_some_missing, self.movies_multiple)
-
-        cbrs.fit(num_cpus=1)
-        result_empty = cbrs.rank(test_ratings, user_id_list=['A000'], num_cpus=1)
-        self.assertTrue(len(result_empty) == 0)
+items_train = train_ratings["to_id"]
+items_test = test_ratings["to_id"]
+
+all_items = items_train.append(items_test)
+for item_id in all_items:
+    if item_id not in item_map:
+        item_map[item_id] = len(item_map)
+
+
+class TestVBPR(TestCase):
+    train_ratings = Ratings.from_dataframe(train_ratings, user_map=user_map, item_map=item_map)
+    test_ratings = Ratings.from_dataframe(test_ratings, user_map=user_map, item_map=item_map)
+
+    user_map = train_ratings.user_map
+    item_map = train_ratings.item_map
+
+    movies_dir = os.path.join(dir_test_files, 'complex_contents', 'movies_codified/')
 
     def test_predict(self):
-        # Test fit with the cbrs algorithm
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
-
-        # we must fit the algorithm in order to predict
-        cbrs.fit(num_cpus=1)
-
-        # Test predict with the cbrs algorithm on specified items
-        result_predict_filtered = cbrs.predict(test_ratings, num_cpus=1)
-        self.assertEqual(len(result_predict_filtered), len(test_ratings))
-
-        # Test predict with the cbrs algorithm on all available unseen items
-        result_predict_all = cbrs.predict(test_ratings, methodology=None, num_cpus=1)
-        self.assertTrue(len(result_predict_all) != 0)
-
-        # Test predict with the cbrs algorithm for only some users
-        result_predict_subset = cbrs.predict(test_ratings, methodology=None, user_id_list=["A000", "A003"], num_cpus=1)
-        self.assertEqual(set(result_predict_subset.user_id_column), {"A000", "A003"})
-        for user in {"A000", "A003"}:
-            result_single = result_predict_subset.get_user_interactions(user)
-            self.assertTrue(len(result_single) != 0)
-
-        # Test predict with alternative methodology
-        result_different_meth = cbrs.predict(test_ratings, methodology=TrainingItemsMethodology(), num_cpus=1)
-        for user in set(test_ratings.user_id_column):
-            result_single = result_different_meth.get_user_interactions(user)
-            result_single_items = set([result_interaction.item_id for result_interaction in result_single])
-            items_already_seen_user = set([train_interaction.item_id
-                                           for train_interaction in train_ratings.get_user_interactions(user)])
-            items_expected_rank = set([train_interaction.item_id
-                                       for train_interaction in train_ratings
-                                       if train_interaction.item_id not in items_already_seen_user])
-
-            self.assertEqual(items_expected_rank, result_single_items)
-
-        # Test algorithm not fitted
-        cbrs = ContentBasedRS(alg, train_ratings_some_missing, self.movies_multiple)
-
-        cbrs.fit(num_cpus=1)
-        result_empty = cbrs.predict(test_ratings, user_id_list=['A000'], num_cpus=1)
-        self.assertTrue(len(result_empty) == 0)
-
-    def test_predict_raise_error(self):
-        alg = ClassifierRecommender({'Plot': ['tfidf', 'embedding']}, SkSVC())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu", seed=42)
+        alg_network = alg.fit(self.train_ratings, items_directory=self.movies_dir, num_cpus=1)
 
-        # You must fit first in order to predict
-        cbrs.fit(num_cpus=1)
+        # Will raise Exception since it's not a Score Prediction Algorithm
+        with self.assertRaises(NotPredictionAlg):
+            alg.predict(alg_network, train_set=self.train_ratings, test_set=self.train_ratings,
+                        items_directory=self.movies_dir, user_idx_list=self.test_ratings.unique_user_idx_column,
+                        methodology=TestRatingsMethodology(), num_cpus=1)
 
-        # This will raise error since page rank is not a prediction algorithm
+        # Will raise Exception since it's not a Score Prediction Algorithm
         with self.assertRaises(NotPredictionAlg):
-            cbrs.predict(test_ratings)
+            alg.fit_predict(train_set=self.train_ratings, test_set=self.test_ratings, items_directory=self.movies_dir,
+                            user_idx_list=self.test_ratings.unique_user_idx_column,
+                            methodology=TestRatingsMethodology(), num_cpus=1, save_fit=True)
 
-    def test_fit_rank(self):
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
+    def test_build_only_positive_ratings(self):
 
-        result = cbrs.fit_rank(test_ratings, save_fit=True, num_cpus=1)
+        # ------ FIXED THRESHOLD (but still all ratings are returned) ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=0, seed=42)
 
-        self.assertTrue(len(result) != 0)
+        only_pos_ratings = alg._build_only_positive_ratings(self.train_ratings)
 
-        # with self.assertRaises(NotFittedAlg):
-        #     cbrs.rank(test_ratings)
+        self.assertEqual(self.train_ratings, only_pos_ratings)
 
+        # ------ FIXED THRESHOLD (for each user, a subset of its ratings is returned) ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=3, seed=42)
 
-    def test_fit_predict(self):
-        alg = LinearPredictor({'Plot': ['tfidf', 'embedding']}, SkLinearRegression())
-        cbrs = ContentBasedRS(alg, train_ratings, self.movies_multiple)
+        expected_pos_ratings = pd.DataFrame.from_records([
+            ("A000", "tt0114576", 5, "54654675"),
+            ("A001", "tt0114576", 3, "54654675"),
+            ("A002", "tt0113497", 4, "54654675"),
+            ("A003", "tt0113497", 4, "54654675")],
+            columns=["user_id", "item_id", "score", "timestamp"])
+        expected_pos_ratings = Ratings.from_dataframe(expected_pos_ratings,
+                                                      user_map=self.train_ratings.user_map,
+                                                      item_map=self.train_ratings.item_map)
 
-        result = cbrs.fit_predict(test_ratings, num_cpus=1)
+        only_pos_ratings = alg._build_only_positive_ratings(self.train_ratings)
 
-        self.assertTrue(len(result) != 0)
+        self.assertEqual(expected_pos_ratings, only_pos_ratings)
 
+        # ------ FIXED THRESHOLD (for some users, no ratings are returned) ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=4, seed=42)
+
+        # user 1 doesn't have any rating anymore
+        expected_pos_ratings = pd.DataFrame.from_records([
+            ("A000", "tt0114576", 5, "54654675"),
+            ("A002", "tt0113497", 4, "54654675"),
+            ("A003", "tt0113497", 4, "54654675")],
+            columns=["user_id", "item_id", "score", "timestamp"])
+        expected_pos_ratings = Ratings.from_dataframe(expected_pos_ratings,
+                                                      user_map=self.train_ratings.user_map,
+                                                      item_map=self.train_ratings.item_map)
 
-class TestGraphBasedRS(TestCase):
+        only_pos_ratings = alg._build_only_positive_ratings(self.train_ratings)
 
-    @classmethod
-    def setUpClass(cls) -> None:
-        # different test ratings from the cbrs since a graph based algorithm
-        # can give predictions only to items that are in the graph
-        test_ratings = pd.DataFrame.from_records([
-            ("A000", "tt0112896", None),
-            ("A000", "tt0112453", None),
-            ("A001", "tt0114576", None),
-            ("A001", "tt0113497", None),
-            ("A002", "tt0114576", None),
-            ("A002", "tt0113041", None),
-            ("A003", "tt0114576", None)],
-            columns=["from_id", "to_id", "score"])
-        cls.test_ratings = Ratings.from_dataframe(test_ratings)
+        self.assertEqual(expected_pos_ratings, only_pos_ratings)
 
-        train_ratings = pd.DataFrame.from_records([
+        # --- FIXED THRESHOLD (empty ratings are returned, meaning that the threshold was too high for all users) ---
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=6, seed=42)
+
+        with self.assertRaises(ValueError):
+            alg._build_only_positive_ratings(self.train_ratings)
+
+        # ------ THRESHOLD SET TO NONE (for each user, a subset of its ratings is returned) ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=None, seed=42)
+
+        expected_pos_ratings = pd.DataFrame.from_records([
             ("A000", "tt0114576", 5, "54654675"),
             ("A001", "tt0114576", 3, "54654675"),
-            ("A001", "tt0112896", 1, "54654675"),
-            ("A000", "tt0113041", 1, "54654675"),
-            ("A002", "tt0112453", 2, "54654675"),
             ("A002", "tt0113497", 4, "54654675"),
-            ("A003", "tt0112453", 1, "54654675"),
             ("A003", "tt0113497", 4, "54654675")],
-            columns=["from_id", "to_id", "score", "timestamp"])
-        train_ratings = Ratings.from_dataframe(train_ratings)
+            columns=["user_id", "item_id", "score", "timestamp"])
+        expected_pos_ratings = Ratings.from_dataframe(expected_pos_ratings,
+                                                      user_map=self.train_ratings.user_map,
+                                                      item_map=self.train_ratings.item_map)
 
-        cls.graph = NXFullGraph(train_ratings)
+        only_pos_ratings = alg._build_only_positive_ratings(self.train_ratings)
 
-    def test_rank(self):
-        # Test rank with the graph based algorithm
-        alg = NXPageRank()
-        gbrs = GraphBasedRS(alg, self.graph)
-
-        # Test ranking with the graph based algorithm on specified items
-        result_rank_filtered = gbrs.rank(self.test_ratings, num_cpus=1)
-        self.assertEqual(len(result_rank_filtered), len(self.test_ratings))
-
-        # Test ranking with the gbrs algorithm on all unseen items that are in the graph
-        result_rank_all = gbrs.rank(self.test_ratings, methodology=None, num_cpus=1)
-        self.assertTrue(len(result_rank_all) != 0)
-
-        # Test top-n ranking with the gbrs algorithm only for some users
-        result_rank_numbered = gbrs.rank(self.test_ratings, n_recs=2, methodology=None, user_id_list=["A000", "A003"],
-                                         num_cpus=1)
-        self.assertEqual(set(result_rank_numbered.user_id_column), {"A000", "A003"})
-        for user in {"A000", "A003"}:
-            result_single = result_rank_numbered.get_user_interactions(user)
-            self.assertTrue(len(result_single) == 2)
-
-        # Test ranking with alternative methodology
-        result_different_meth = gbrs.rank(self.test_ratings, methodology=TrainingItemsMethodology(), num_cpus=1)
-        for user in set(self.test_ratings.user_id_column):
-            result_single = set([pred_rank.item_id for pred_rank in result_different_meth if pred_rank.user_id == user])
-            items_already_seen_user = set([original_interaction.item_id
-                                           for original_interaction in train_ratings.get_user_interactions(user)])
-            items_expected_rank = set([train_interaction.item_id
-                                       for train_interaction in train_ratings
-                                       if train_interaction.item_id not in items_already_seen_user])
-
-            self.assertEqual(items_expected_rank, result_single)
-
-    def test_predict_raise_error(self):
-        alg = NXPageRank()
-        gbrs = GraphBasedRS(alg, self.graph)
+        self.assertEqual(expected_pos_ratings, only_pos_ratings)
+
+    def test_load_items_features(self):
+
+        # ------ Generic case, items features (for items in ratings) are loaded from the source ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=None, normalize=False, seed=42)
+
+        features = alg._load_items_features(self.train_ratings, self.movies_dir)
+
+        items_id_locally_available = set(filename.split(".")[0] for filename in os.listdir(self.movies_dir))
+        items_id_to_extract_features = list(self.train_ratings.item_map.map)
+
+        first_not_none_element = next(item for item in features if item is not None)
+        for i, item_id_to_extract in enumerate(items_id_to_extract_features):
+
+            # if is not present then array of zeros is used
+            if item_id_to_extract not in items_id_locally_available:
+                expected = torch.zeros(size=first_not_none_element.shape)
+                result = features[i]
+
+                np.testing.assert_array_equal(expected.numpy(), result)
+            # otherwise if it is present obviously we expect that features are different from array of zeros
+            else:
+                not_expected = torch.zeros(size=first_not_none_element.shape)
+                result = features[i]
+
+                self.assertFalse(np.array_equal(not_expected.numpy(), result))
+
+        # ------ Normalization set to True, features are expected to be in the [0, 1] range ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=None, normalize=True, seed=42)
+
+        features = alg._load_items_features(self.train_ratings, self.movies_dir)
+
+        self.assertTrue(all(min(feature) >= 0 and max(feature) <= 1 for feature in features))
+
+        # ------ Limit case, all items in the ratings do not have a matching serialized feature ------
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=0, device="cpu",
+                   threshold=None, seed=42)
+
+        ratings_non_existent_features_items = pd.DataFrame.from_records([
+            ("A000", "featureless_1", 4, "54654675"),
+            ("A001", "featureless_2", 3, "54654675"),
+            ("A002", "featureless_3", 5, "54654675"),
+            ("A002", "featureless_4", 4, "54654675"),
+            ("A003", "featureless_5", 4, "54654675")],
+            columns=["user_id", "item_id", "score", "timestamp"])
+        ratings_non_existent_features_items = Ratings.from_dataframe(ratings_non_existent_features_items)
+
+        with self.assertRaises(FileNotFoundError):
+            alg._load_items_features(ratings_non_existent_features_items, self.movies_dir)
+
+    def test_rank_single_representation(self):
+        # Single representation
+        alg = VBPR({'Genre': ['embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=1, device="cpu", seed=42)
+        alg_network = alg.fit(self.train_ratings, items_directory=self.movies_dir, num_cpus=1)
+
+        # unbounded rank
+        result_rank_filtered = alg.rank(alg_network, train_set=self.train_ratings, test_set=self.test_ratings,
+                                        items_directory=self.movies_dir,
+                                        user_idx_list=self.train_ratings.unique_user_idx_column,
+                                        methodology=TestRatingsMethodology(), num_cpus=1, n_recs=None)
+
+        # result_rank_filtered contains one ranked uir per user
+        self.assertEqual(len(self.test_ratings.unique_user_idx_column), len(result_rank_filtered))
+
+        for rank_user_uir in result_rank_filtered:
+            user_idx = rank_user_uir[0][0]  # the idx for the uir rank is in the first column first cell ([0][0])
+            self.assertEqual(len(self.test_ratings.get_user_interactions(user_idx)), len(rank_user_uir))
+
+        # rank with recs_number specified
+        n_recs = 2
+        res_n_recs = alg.rank(alg_network, train_set=self.train_ratings, test_set=self.test_ratings,
+                              items_directory=self.movies_dir, user_idx_list=self.test_ratings.unique_user_idx_column,
+                              methodology=TestRatingsMethodology(), num_cpus=1, n_recs=n_recs)
+
+        # result_rank_filtered contains one ranked uir per user
+        self.assertEqual(len(self.test_ratings.unique_user_idx_column), len(result_rank_filtered))
+
+        for rank_user_uir in res_n_recs[:-1]:
+            self.assertEqual(n_recs, len(rank_user_uir))
+
+        # user A003 has only 1 item in the test set to recommend (test ratings methodology)
+        self.assertEqual(1, len(res_n_recs[-1]))
+
+    def test_rank_multiple_representations(self):
+        # Multiple representations
+        alg = VBPR({'Plot': ['tfidf', 'embedding'], 'Genre': ['tfidf', 'embedding']}, gamma_dim=10, theta_dim=10,
+                   batch_size=64, epochs=1, device="cpu", seed=42)
+        alg_network = alg.fit(self.train_ratings, items_directory=self.movies_dir, num_cpus=1)
+
+        # unbounded rank
+        result_rank_filtered = alg.rank(alg_network, train_set=self.train_ratings, test_set=self.test_ratings,
+                                        items_directory=self.movies_dir,
+                                        user_idx_list=self.test_ratings.unique_user_idx_column,
+                                        methodology=TestRatingsMethodology(), num_cpus=1, n_recs=None)
+
+        # result_rank_filtered contains one ranked uir per user
+        self.assertEqual(len(self.test_ratings.unique_user_idx_column), len(result_rank_filtered))
+
+        for rank_user_uir in result_rank_filtered:
+            user_idx = rank_user_uir[0][0]  # the idx for the uir rank is in the first column first cell ([0][0])
+            self.assertEqual(len(self.test_ratings.get_user_interactions(user_idx)), len(rank_user_uir))
+
+        # rank with recs_number specified
+        n_recs = 2
+        res_n_recs = alg.rank(alg_network, train_set=self.train_ratings, test_set=self.test_ratings,
+                              items_directory=self.movies_dir, user_idx_list=self.test_ratings.unique_user_idx_column,
+                              methodology=TestRatingsMethodology(), num_cpus=1, n_recs=n_recs)
+
+        # result_rank_filtered contains one ranked uir per user
+        self.assertEqual(len(self.test_ratings.unique_user_idx_column), len(result_rank_filtered))
+
+        for rank_user_uir in res_n_recs[:-1]:
+            self.assertEqual(n_recs, len(rank_user_uir))
+
+        # user A003 has only 1 item in the test set to recommend (test ratings methodology)
+        self.assertEqual(1, len(res_n_recs[-1]))
+
+    def test_fit_rank(self):
+        # Compare results when using fit and rank with results obtained from calling fit_rank directly
+        alg = VBPR({'Genre': ['tfidf', 'embedding']}, gamma_dim=10, theta_dim=10, batch_size=64, epochs=1,
+                   device="cpu", seed=42)
+
+        alg_network = alg.fit(self.train_ratings, items_directory=self.movies_dir, num_cpus=1)
+        result_rank_fit = alg.rank(alg_network, train_set=self.train_ratings, test_set=self.test_ratings,
+                                   items_directory=self.movies_dir,
+                                   user_idx_list=self.test_ratings.unique_user_idx_column,
+                                   methodology=TestRatingsMethodology(), num_cpus=1, n_recs=None)
+
+        alg_network_fit, result_rank_fit_rank = alg.fit_rank(train_set=self.train_ratings, test_set=self.test_ratings,
+                                                             items_directory=self.movies_dir,
+                                                             user_idx_list=self.test_ratings.unique_user_idx_column,
+                                                             methodology=TestRatingsMethodology(), num_cpus=1,
+                                                             n_recs=None,
+                                                             save_fit=True)
+
+        for single_result_rank_fit, single_result_rank_fit_rank in zip(result_rank_fit, result_rank_fit_rank):
+            np.testing.assert_array_equal(single_result_rank_fit, single_result_rank_fit_rank)
+
+        self.assertIsNotNone(alg_network_fit)  # save_fit == True so the fit alg is returned
+
+        # test save_fit == False
+        alg_network_fit, _ = alg.fit_rank(train_set=self.train_ratings, test_set=self.test_ratings,
+                                          items_directory=self.movies_dir,
+                                          user_idx_list=self.test_ratings.unique_user_idx_column,
+                                          methodology=TestRatingsMethodology(), num_cpus=1,
+                                          n_recs=None,
+                                          save_fit=False)
+
+        self.assertIsNone(alg_network_fit)  # save_fit == False is we don't save the fit alg
 
-        # This will raise error since page rank is not a prediction algorithm
-        with self.assertRaises(NotPredictionAlg):
-            gbrs.predict(self.test_ratings, num_cpus=1)
 
-    def test_rank_filterlist_empty_A000(self):
-        # no items to recommend is in the graph for user A000
-        test_ratings = pd.DataFrame.from_records([
-            ("A000", "not_in_graph", None),
-            ("A000", "not_in_graph1", None),
-            ("A001", "tt0114576", None),
-            ("A001", "tt0113497", None),
-            ("A002", "tt0114576", None),
-            ("A002", "tt0113041", None),
-            ("A003", "tt0114576", None)],
-            columns=["from_id", "to_id", "score"])
-        test_ratings = Ratings.from_dataframe(test_ratings)
-
-        # Test rank with the graph based algorithm
-        alg = NXPageRank()
-        gbrs = GraphBasedRS(alg, self.graph)
-
-        # Test ranking with the graph based algorithm with items not present in the graph for A000
-        result_rank = gbrs.rank(test_ratings, num_cpus=1)
-        self.assertTrue(len(result_rank) != 0)
-
-        # no rank is present for A000
-        with self.assertRaises(KeyError):
-            result_rank.get_user_interactions('A000')
-
-    def test_rank_filterlist_empty_all(self):
-        # different test ratings from the cbrs since a graph based algorithm
-        # can give predictions only to items that are in the graph
-        test_ratings = pd.DataFrame.from_records([
-            ("A000", "not_in_graph", None),
-            ("A000", "not_in_graph1", None),
-            ("A001", "not_in_graph2", None),
-            ("A001", "not_in_graph3", None),
-            ("A002", "not_in_graph4", None),
-            ("A002", "not_in_graph5", None),
-            ("A003", "not_in_graph6", None)],
-            columns=["from_id", "to_id", "score"])
-        test_ratings = Ratings.from_dataframe(test_ratings)
-
-        # Test rank with the graph based algorithm
-        alg = NXPageRank()
-        gbrs = GraphBasedRS(alg, self.graph)
-
-        # Test ranking with the graph based algorithm on items not in the graph, we expect it to be empty
-        result_rank_empty = gbrs.rank(test_ratings, num_cpus=1)
-        self.assertTrue(len(result_rank_empty) == 0)
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `clayrs-0.4.1/test/utils/test_automatic_methods.py` & `clayrs-0.5.1/test/utils/test_automatic_methods.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/utils/test_class_utils.py` & `clayrs-0.5.1/test/utils/test_class_utils.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/utils/test_context_managers.py` & `clayrs-0.5.1/test/utils/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `clayrs-0.4.1/test/utils/test_report.py` & `clayrs-0.5.1/test/utils/test_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,36 +66,36 @@
         self.assertIsNotNone(exogenous_representations_dict.get('PropertiesFromDataset'))
 
         # Check that field representations codified are present
         field_dict = result.get("field_representations")
         self.assertIsNotNone(field_dict)
 
         # Representations for plot field
-        plot_dict = field_dict.get('plot_0')
+        plot_dict = field_dict.get('plot/0')
         self.assertIsNotNone(plot_dict)
 
         self.assertIsNotNone(plot_dict.get('SkLearnTfIdf'))
 
         plot_preprocessing_dict = plot_dict.get('preprocessing')
         self.assertIsNotNone(plot_preprocessing_dict)
         self.assertIsNotNone(plot_preprocessing_dict.get('NLTK'))
         self.assertIsNotNone(plot_preprocessing_dict.get('Ekphrasis'))
 
         # Representation 0 for genres field
-        genres_0_dict = field_dict.get('genres_0')
+        genres_0_dict = field_dict.get('genres/0')
         self.assertIsNotNone(genres_0_dict)
 
         self.assertIsNotNone(genres_0_dict.get('WordEmbeddingTechnique'))
 
         genres_0_preprocessing_dict = genres_0_dict.get('preprocessing')
         self.assertIsNotNone(genres_0_preprocessing_dict)
         self.assertIsNotNone(genres_0_preprocessing_dict.get('Spacy'))
 
         # Representation 1 for genres field
-        genres_1_dict = field_dict.get('genres_1')
+        genres_1_dict = field_dict.get('genres/1')
         self.assertIsNotNone(genres_1_dict)
 
         self.assertIsNotNone(genres_1_dict.get('SentenceEmbeddingTechnique'))
 
         genres_1_preprocessing_dict = genres_1_dict.get('preprocessing')
         self.assertIsNotNone(genres_1_preprocessing_dict)
         self.assertIsNotNone(genres_1_preprocessing_dict.get('Spacy'))
@@ -167,31 +167,14 @@
         self.assertIsNotNone(partitioning_dict)
         self.assertIsNotNone(partitioning_dict.get('HoldOutPartitioning'))
 
         recsys_dict = result.get('recsys')
         self.assertIsNotNone(recsys_dict)
         self.assertIsNotNone(recsys_dict.get('GraphBasedRS'))
 
-    def test_rs_yaml_error(self):
-        original_rat = Ratings(CSVFile(rat_path))
-
-        pt = HoldOutPartitioning()
-
-        train_list, test_list = pt.split_all(original_rat)
-
-        alg = NXPageRank()
-
-        graph = NXFullGraph(train_list[0])
-
-        gbrs = GraphBasedRS(alg, graph=graph)
-
-        # try to build report without calling the rank method first
-        with self.assertRaises(ValueError):
-            Report(output_dir="this doesn't work").yaml(recsys=gbrs)
-
     @staticmethod
     def _build_eva_report():
 
         # rank same as truth since we don't care about results
         rank = Rank(CSVFile(rat_path))
         truth = Ratings(CSVFile(rat_path))
```

