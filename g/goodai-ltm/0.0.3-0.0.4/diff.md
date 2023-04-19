# Comparing `tmp/goodai-ltm-0.0.3.tar.gz` & `tmp/goodai-ltm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.0.3.tar", last modified: Wed Apr 19 18:24:52 2023, max compression
+gzip compressed data, was "goodai-ltm-0.0.4.tar", last modified: Wed Apr 19 18:51:42 2023, max compression
```

## Comparing `goodai-ltm-0.0.3.tar` & `goodai-ltm-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.652954 goodai-ltm-0.0.3/
--rw-rw-rw-   0        0        0      184 2023-04-19 18:24:52.651955 goodai-ltm-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-04-19 16:41:41.000000 goodai-ltm-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.581276 goodai-ltm-0.0.3/goodai/
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.592275 goodai-ltm-0.0.3/goodai/ltm/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.594274 goodai-ltm-0.0.3/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.595277 goodai-ltm-0.0.3/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     2000 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/names/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.603959 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     1518 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      323 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     2426 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      175 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    10899 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1861 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/qa_tok_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.605961 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0     2531 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     6800 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/data/query_passage/wiki.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.615108 goodai-ltm-0.0.3/goodai/ltm/embedding_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/__init__.py
--rw-rw-rw-   0        0        0      839 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/auto.py
--rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/contrast_classifier.py
--rw-rw-rw-   0        0        0     5290 2023-04-19 16:47:44.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/default.py
--rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     2648 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/openai_emb.py
--rw-rw-rw-   0        0        0     2081 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/st_emb.py
--rw-rw-rw-   0        0        0     5252 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/embedding_models/trainable.py
--rw-rw-rw-   0        0        0     1312 2023-04-19 16:11:12.000000 goodai-ltm-0.0.3/goodai/ltm/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.618108 goodai-ltm-0.0.3/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     3926 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     3006 2023-04-18 23:54:27.000000 goodai-ltm-0.0.3/goodai/ltm/eval/metrics.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.625434 goodai-ltm-0.0.3/goodai/ltm/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/collections_helper.py
--rw-rw-rw-   0        0        0      868 2023-04-18 21:34:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/json_helper.py
--rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/helpers/torch_helper.py
--rw-rw-rw-   0        0        0     1044 2023-04-19 16:11:46.000000 goodai-ltm-0.0.3/goodai/ltm/matching.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.629434 goodai-ltm-0.0.3/goodai/ltm/matching_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.3/goodai/ltm/matching_models/__init__.py
--rw-rw-rw-   0        0        0      187 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/matching_models/auto.py
--rw-rw-rw-   0        0        0    10023 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/matching_models/default.py
--rw-rw-rw-   0        0        0      623 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/matching_models/prob_model.py
--rw-rw-rw-   0        0        0     1144 2023-04-19 16:12:29.000000 goodai-ltm-0.0.3/goodai/ltm/memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.640438 goodai-ltm-0.0.3/goodai/ltm/memory_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/auto.py
--rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk.py
--rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk_mixin.py
--rw-rw-rw-   0        0        0    10289 2023-04-19 18:19:26.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk_queue.py
--rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/config.py
--rw-rw-rw-   0        0        0     5566 2023-04-19 18:20:54.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/default.py
--rw-rw-rw-   0        0        0     5723 2023-04-19 18:18:01.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/mem_foundation.py
--rw-rw-rw-   0        0        0     2896 2023-04-19 18:16:19.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.643863 goodai-ltm-0.0.3/goodai/ltm/memory_models/tests/
--rw-rw-rw-   0        0        0     3101 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/tests/TestChunkQueue.py
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/memory_models/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.644876 goodai-ltm-0.0.3/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.646874 goodai-ltm-0.0.3/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.3/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.3/goodai/ltm/training/query_passage/trainer.py
--rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.3/goodai/ltm/training/sched_opt.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:52.650940 goodai-ltm-0.0.3/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-19 18:24:52.000000 goodai-ltm-0.0.3/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2225 2023-04-19 18:24:52.000000 goodai-ltm-0.0.3/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:24:52.000000 goodai-ltm-0.0.3/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-04-19 18:24:52.000000 goodai-ltm-0.0.3/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 18:24:52.000000 goodai-ltm-0.0.3/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:24:52.652954 goodai-ltm-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      568 2023-04-19 17:18:11.000000 goodai-ltm-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/
+-rw-rw-rw-   0        0        0      184 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1984 2023-04-19 18:49:15.000000 goodai-ltm-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.929559 goodai-ltm-0.0.4/goodai/
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.952550 goodai-ltm-0.0.4/goodai/ltm/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.953550 goodai-ltm-0.0.4/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.954550 goodai-ltm-0.0.4/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     2000 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/names/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.963550 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     1518 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      323 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     2426 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      175 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    10899 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1861 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa_tok_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.965549 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0     2531 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     6800 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/data/query_passage/wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.974550 goodai-ltm-0.0.4/goodai/ltm/embedding_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/__init__.py
+-rw-rw-rw-   0        0        0      839 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/auto.py
+-rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5290 2023-04-19 16:47:44.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/default.py
+-rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     2648 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/openai_emb.py
+-rw-rw-rw-   0        0        0     2081 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/st_emb.py
+-rw-rw-rw-   0        0        0     5252 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/embedding_models/trainable.py
+-rw-rw-rw-   0        0        0     1312 2023-04-19 16:11:12.000000 goodai-ltm-0.0.4/goodai/ltm/embeddings.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.977550 goodai-ltm-0.0.4/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     3926 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     3006 2023-04-18 23:54:27.000000 goodai-ltm-0.0.4/goodai/ltm/eval/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.984550 goodai-ltm-0.0.4/goodai/ltm/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/collections_helper.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 21:34:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/helpers/torch_helper.py
+-rw-rw-rw-   0        0        0     1044 2023-04-19 16:11:46.000000 goodai-ltm-0.0.4/goodai/ltm/matching.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.988550 goodai-ltm-0.0.4/goodai/ltm/matching_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/auto.py
+-rw-rw-rw-   0        0        0    10023 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/default.py
+-rw-rw-rw-   0        0        0      623 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/matching_models/prob_model.py
+-rw-rw-rw-   0        0        0     1144 2023-04-19 16:12:29.000000 goodai-ltm-0.0.4/goodai/ltm/memory.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:41.997990 goodai-ltm-0.0.4/goodai/ltm/memory_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/auto.py
+-rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk.py
+-rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_mixin.py
+-rw-rw-rw-   0        0        0    10289 2023-04-19 18:19:26.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_queue.py
+-rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/config.py
+-rw-rw-rw-   0        0        0     5566 2023-04-19 18:20:54.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/default.py
+-rw-rw-rw-   0        0        0     5723 2023-04-19 18:18:01.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/mem_foundation.py
+-rw-rw-rw-   0        0        0     2896 2023-04-19 18:16:19.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.000988 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/
+-rw-rw-rw-   0        0        0     3101 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/TestChunkQueue.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.001987 goodai-ltm-0.0.4/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.003989 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.4/goodai/ltm/training/query_passage/trainer.py
+-rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.4/goodai/ltm/training/sched_opt.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:51:42.008988 goodai-ltm-0.0.4/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2225 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 18:51:41.000000 goodai-ltm-0.0.4/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 18:51:42.009989 goodai-ltm-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-04-19 18:51:37.000000 goodai-ltm-0.0.4/setup.py
```

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/cloud.py` & `goodai-ltm-0.0.4/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.0.4/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/dataset.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/tests/TestQueryPassageDataSource.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.0.4/goodai/ltm/data/query_passage/wiki.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/auto.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/contrast_classifier.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/default.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/emb_qp_prob_model.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/emb_qp_prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/openai_emb.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/openai_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/st_emb.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/st_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embedding_models/trainable.py` & `goodai-ltm-0.0.4/goodai/ltm/embedding_models/trainable.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/embeddings.py` & `goodai-ltm-0.0.4/goodai/ltm/embeddings.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/eval/mem.py` & `goodai-ltm-0.0.4/goodai/ltm/eval/mem.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.0.4/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/helpers/collections_helper.py` & `goodai-ltm-0.0.4/goodai/ltm/helpers/collections_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/helpers/file_helper.py` & `goodai-ltm-0.0.4/goodai/ltm/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/helpers/tokenizer_helper.py` & `goodai-ltm-0.0.4/goodai/ltm/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/matching.py` & `goodai-ltm-0.0.4/goodai/ltm/matching.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/matching_models/default.py` & `goodai-ltm-0.0.4/goodai/ltm/matching_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/matching_models/prob_model.py` & `goodai-ltm-0.0.4/goodai/ltm/matching_models/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory.py` & `goodai-ltm-0.0.4/goodai/ltm/memory.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/auto.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk_mixin.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_mixin.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/chunk_queue.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/default.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/mem_foundation.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/mem_foundation.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/simple_vector_db.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/simple_vector_db.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/memory_models/tests/TestChunkQueue.py` & `goodai-ltm-0.0.4/goodai/ltm/memory_models/tests/TestChunkQueue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/training/query_passage/trainer.py` & `goodai-ltm-0.0.4/goodai/ltm/training/query_passage/trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai/ltm/training/sched_opt.py` & `goodai-ltm-0.0.4/goodai/ltm/training/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.0.4/goodai_ltm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.3/setup.py` & `goodai-ltm-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 packages = find_namespace_packages(include=['goodai.*'])
 
 setup(name='goodai-ltm',
       description='A text memory meant to be used with conversational language models.',
       url='https://github.com/GoodAI/goodai-ltm',
-      version='0.0.3',
+      version='0.0.4',
       packages=packages,
       package_data={},
       install_requires=['torch>=1.8.0', 'pytest>=7.0.0', 'numpy>=1.19.0', 'transformers>=4.0.0',
-                        'openai>=0.27.0', 'faiss-cpu', 'datasets', 'boto3', 'python-dotenv']
+                        'openai>=0.27.0', 'faiss-cpu', 'datasets', 'boto3', 'python-dotenv',
+                        'sentence-transformers>=2.2.2']
 )
```

