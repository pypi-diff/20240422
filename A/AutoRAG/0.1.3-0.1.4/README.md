# Comparing `tmp/autorag-0.1.3.tar.gz` & `tmp/autorag-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.3.tar", last modified: Sun Apr 14 04:50:14 2024, max compression
+gzip compressed data, was "autorag-0.1.4.tar", last modified: Mon Apr 22 06:04:28 2024, max compression
```

## Comparing `autorag-0.1.3.tar` & `autorag-0.1.4.tar`

### file list

```diff
@@ -1,490 +1,499 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.211042 autorag-0.1.3/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.097929 autorag-0.1.3/.github/
--rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.098426 autorag-0.1.3/.github/workflows/
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.3/.github/workflows/sphinx.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)      862 2024-04-06 14:23:40.000000 autorag-0.1.3/.github/workflows/test.yml
--rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.3/.gitignore
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.210234 autorag-0.1.3/AutoRAG.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)    24163 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)    18745 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-14 04:50:14.000000 autorag-0.1.3/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.3/LICENSE
--rw-r--r--   0 jeffrey    (501) staff       (20)    24163 2024-04-14 04:50:14.210777 autorag-0.1.3/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     9163 2024-04-11 14:29:33.000000 autorag-0.1.3/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.101427 autorag-0.1.3/autorag/
--rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-14 04:47:22.000000 autorag-0.1.3/autorag/VERSION
--rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.3/autorag/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/cli.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.101744 autorag-0.1.3/autorag/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.3/autorag/data/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.102675 autorag-0.1.3/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.3/autorag/data/corpus/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 autorag-0.1.3/autorag/data/corpus/langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 autorag-0.1.3/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.104146 autorag-0.1.3/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.3/autorag/data/qacreation/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2754 2024-04-12 15:53:11.000000 autorag-0.1.3/autorag/data/qacreation/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7107 2024-03-23 03:44:06.000000 autorag-0.1.3/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.3/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/data/qacreation/ragas.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.104520 autorag-0.1.3/autorag/data/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/data/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/data/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.3/autorag/deploy.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.105953 autorag-0.1.3/autorag/evaluate/
--rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/generation.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.107098 autorag-0.1.3/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.108088 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)    11906 2024-04-05 14:53:42.000000 autorag-0.1.3/autorag/evaluate/metric/generation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.3/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.3/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/metric/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/retrieval.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.3/autorag/evaluate/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.3/autorag/evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/node_line.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.108276 autorag-0.1.3/autorag/nodes/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.109530 autorag-0.1.3/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.3/autorag/nodes/generator/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.3/autorag/nodes/generator/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.3/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.3/autorag/nodes/generator/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.3/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.110831 autorag-0.1.3/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)       88 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2433 2024-03-06 19:11:31.000000 autorag-0.1.3/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.3/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.112286 autorag-0.1.3/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      171 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1694 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.3/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3955 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.116264 autorag-0.1.3/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.3/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3625 2024-04-08 12:04:54.000000 autorag-0.1.3/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3548 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.3/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6838 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.3/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.3/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.3/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3889 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.117192 autorag-0.1.3/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4452 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.3/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.3/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.119246 autorag-0.1.3/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.3/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.3/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.120925 autorag-0.1.3/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.3/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.3/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.3/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.3/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.123150 autorag-0.1.3/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.3/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.3/autorag/nodes/retrieval/run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.3/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.123831 autorag-0.1.3/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/module.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/schema/node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3826 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/support.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.124457 autorag-0.1.3/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/utils/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 autorag-0.1.3/autorag/utils/preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9737 2024-04-14 04:47:06.000000 autorag-0.1.3/autorag/utils/util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.3/autorag/web.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-02-18 10:18:03.000000 autorag-0.1.3/dev_requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.125086 autorag-0.1.3/docs/
--rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.3/docs/Makefile
--rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.3/docs/make.bat
--rw-r--r--   0 jeffrey    (501) staff       (20)      110 2024-03-30 16:07:43.000000 autorag-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.127033 autorag-0.1.3/docs/source/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.134013 autorag-0.1.3/docs/source/_static/
--rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/data_creation.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/data_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_line_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_line_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_lines.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/node_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.3/docs/source/_static/project_folder_example.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/project_folders.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.138104 autorag-0.1.3/docs/source/_static/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.3/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_folder.png
--rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_json.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/_static/trial_summary.png
--rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.3/docs/source/_static/web_interface.png
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.140782 autorag-0.1.3/docs/source/api_spec/
--rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.3/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1091 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1277 2024-04-14 04:49:44.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     3229 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1688 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      432 2024-04-10 13:46:46.000000 autorag-0.1.3/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.3/docs/source/api_spec/autorag.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.3/docs/source/api_spec/modules.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1371 2024-03-30 16:07:43.000000 autorag-0.1.3/docs/source/conf.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.141424 autorag-0.1.3/docs/source/data_creation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.3/docs/source/data_creation/data_format.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/data_creation/ragas.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.3/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.141910 autorag-0.1.3/docs/source/deploy/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.3/docs/source/deploy/web.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/index.rst
--rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.3/docs/source/install.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/local_model.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.142136 autorag-0.1.3/docs/source/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.142796 autorag-0.1.3/docs/source/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.3/docs/source/nodes/generator/generator.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.3/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/index.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.143247 autorag-0.1.3/docs/source/nodes/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3036 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.143859 autorag-0.1.3/docs/source/nodes/passage_filter/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1747 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.3/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.147476 autorag-0.1.3/docs/source/nodes/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.148278 autorag-0.1.3/docs/source/nodes/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.3/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.148757 autorag-0.1.3/docs/source/nodes/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.3/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.150086 autorag-0.1.3/docs/source/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.3/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.151103 autorag-0.1.3/docs/source/optimization/
--rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.3/docs/source/optimization/custom_config.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/optimization/folder_structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.3/docs/source/optimization/optimization.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.151322 autorag-0.1.3/docs/source/roadmap/
--rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.3/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.3/docs/source/structure.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.3/docs/source/troubleshooting.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.3/docs/source/tutorial.md
--rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.3/pyproject.toml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.3/requirements.txt
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.152988 autorag-0.1.3/sample_config/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.3/sample_config/compact_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.3/sample_config/compact_openai.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.3/sample_config/config_korean.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.3/sample_config/extracted_sample.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     4291 2024-04-12 13:21:50.000000 autorag-0.1.3/sample_config/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.3/sample_config/simple_local.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.3/sample_config/simple_openai.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153222 autorag-0.1.3/sample_dataset/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153545 autorag-0.1.3/sample_dataset/eli5/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.153788 autorag-0.1.3/sample_dataset/msmarco/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.3/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.154140 autorag-0.1.3/sample_dataset/triviaqa/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.3/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-14 04:50:14.211093 autorag-0.1.3/setup.cfg
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.154892 autorag-0.1.3/tests/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.156437 autorag-0.1.3/tests/autorag/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.092163 autorag-0.1.3/tests/autorag/data/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.157572 autorag-0.1.3/tests/autorag/data/corpus/
--rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.3/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 autorag-0.1.3/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.158511 autorag-0.1.3/tests/autorag/data/qacreation/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1415 2024-04-12 15:50:36.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2720 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1931 2024-03-22 03:52:09.000000 autorag-0.1.3/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.159428 autorag-0.1.3/tests/autorag/evaluate/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.160118 autorag-0.1.3/tests/autorag/evaluate/metric/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.3/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3191 2024-02-23 12:23:14.000000 autorag-0.1.3/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.093041 autorag-0.1.3/tests/autorag/nodes/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.161099 autorag-0.1.3/tests/autorag/nodes/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.3/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.161857 autorag-0.1.3/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2525 2024-02-22 16:08:56.000000 autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.163053 autorag-0.1.3/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2476 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.166753 autorag-0.1.3/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.167623 autorag-0.1.3/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     7998 2024-03-31 10:29:05.000000 autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.168932 autorag-0.1.3/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.171883 autorag-0.1.3/tests/autorag/nodes/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.3/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.172384 autorag-0.1.3/tests/autorag/schema/
--rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.3/tests/autorag/test_cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/autorag/test_deploy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)    14194 2024-04-12 16:43:24.000000 autorag-0.1.3/tests/autorag/test_evaluator.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/test_strategy.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/test_support.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.3/tests/autorag/test_web.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.172779 autorag-0.1.3/tests/autorag/utils/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 autorag-0.1.3/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.3/tests/autorag/utils/test_util.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/conftest.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.3/tests/delete_tests.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.3/tests/mock.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.175432 autorag-0.1.3/tests/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/README.md
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.3/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.093444 autorag-0.1.3/tests/resources/data_creation/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.176645 autorag-0.1.3/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.3/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.3/tests/resources/full.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.3/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.177373 autorag-0.1.3/tests/resources/qa_gen_prompts/
--rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.3/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178179 autorag-0.1.3/tests/resources/result_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178645 autorag-0.1.3/tests/resources/result_project/0/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.178850 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.181316 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.182195 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.182443 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.183740 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.183879 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.184700 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.186144 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.187632 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.3/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.187859 autorag-0.1.3/tests/resources/result_project/1/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.188123 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.189446 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.095141 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.189622 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.190582 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192059 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192304 autorag-0.1.3/tests/resources/result_project/2/
--rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.095398 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.192575 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.193033 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.195497 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.195677 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.196559 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.198301 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.200063 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.200297 autorag-0.1.3/tests/resources/result_project/3/
--rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.3/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201331 autorag-0.1.3/tests/resources/result_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201634 autorag-0.1.3/tests/resources/result_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.3/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.201909 autorag-0.1.3/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.208141 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.3/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.3/tests/resources/result_project/trial.json
--rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.3/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.096489 autorag-0.1.3/tests/resources/sample_project/
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.209096 autorag-0.1.3/tests/resources/sample_project/data/
--rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.3/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.3/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-14 04:50:14.209387 autorag-0.1.3/tests/resources/sample_project/resources/
--rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.3/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.3/tests/resources/simple.yaml
--rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.3/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.186767 autorag-0.1.4/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.067275 autorag-0.1.4/.github/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      501 2024-01-13 07:55:28.000000 autorag-0.1.4/.github/dependabot.yml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.067903 autorag-0.1.4/.github/workflows/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-03-25 06:37:01.000000 autorag-0.1.4/.github/workflows/sphinx.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      927 2024-04-22 05:42:18.000000 autorag-0.1.4/.github/workflows/test.yml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3088 2024-01-13 07:55:28.000000 autorag-0.1.4/.gitignore
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.185949 autorag-0.1.4/AutoRAG.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19139 2024-04-22 06:04:28.000000 autorag-0.1.4/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       44 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      512 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        8 2024-04-22 06:04:27.000000 autorag-0.1.4/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2936 2024-04-22 05:42:18.000000 autorag-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6374 2024-04-22 05:42:18.000000 autorag-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11357 2024-01-13 07:55:28.000000 autorag-0.1.4/LICENSE
+-rw-r--r--   0 jeffrey    (501) staff       (20)    24161 2024-04-22 06:04:28.186490 autorag-0.1.4/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9161 2024-04-15 08:09:03.000000 autorag-0.1.4/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.071310 autorag-0.1.4/autorag/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        5 2024-04-22 06:00:49.000000 autorag-0.1.4/autorag/VERSION
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2686 2024-03-27 16:56:49.000000 autorag-0.1.4/autorag/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4400 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/cli.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.071520 autorag-0.1.4/autorag/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-04-01 09:28:42.000000 autorag-0.1.4/autorag/data/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.072262 autorag-0.1.4/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      134 2024-03-22 04:27:08.000000 autorag-0.1.4/autorag/data/corpus/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1625 2024-03-22 05:41:56.000000 autorag-0.1.4/autorag/data/corpus/langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2834 2024-03-22 04:27:08.000000 autorag-0.1.4/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.073794 autorag-0.1.4/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-04-11 07:54:19.000000 autorag-0.1.4/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3123 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/data/qacreation/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7473 2024-04-17 13:38:02.000000 autorag-0.1.4/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3190 2024-03-23 03:44:06.000000 autorag-0.1.4/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2924 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3289 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.074130 autorag-0.1.4/autorag/data/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/data/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1496 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/data/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8871 2024-03-06 00:03:36.000000 autorag-0.1.4/autorag/deploy.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.075680 autorag-0.1.4/autorag/evaluate/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      146 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2603 2024-04-05 14:53:42.000000 autorag-0.1.4/autorag/evaluate/generation.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.077004 autorag-0.1.4/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      252 2024-04-05 14:53:42.000000 autorag-0.1.4/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.078055 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1186 2024-02-23 11:07:36.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1015 2024-02-23 11:07:40.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      814 2024-02-23 11:07:43.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1005 2024-02-23 11:07:46.000000 autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)    12720 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1477 2024-02-23 18:16:58.000000 autorag-0.1.4/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2131 2024-02-23 18:16:58.000000 autorag-0.1.4/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      224 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/metric/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2052 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/retrieval.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2099 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1290 2024-02-18 20:58:37.000000 autorag-0.1.4/autorag/evaluate/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    17273 2024-04-12 13:21:55.000000 autorag-0.1.4/autorag/evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2248 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/node_line.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.078404 autorag-0.1.4/autorag/nodes/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.079594 autorag-0.1.4/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       68 2024-03-07 23:12:39.000000 autorag-0.1.4/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2215 2024-03-07 22:31:53.000000 autorag-0.1.4/autorag/nodes/generator/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1641 2024-03-30 16:26:48.000000 autorag-0.1.4/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4532 2024-03-31 04:56:43.000000 autorag-0.1.4/autorag/nodes/generator/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2810 2024-03-08 18:01:40.000000 autorag-0.1.4/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.081205 autorag-0.1.4/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      115 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2445 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      242 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2857 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6075 2024-02-15 17:28:32.000000 autorag-0.1.4/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3028 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.082746 autorag-0.1.4/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      207 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2242 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      417 2024-04-11 14:32:56.000000 autorag-0.1.4/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3922 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2476 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3955 2024-04-10 13:46:46.000000 autorag-0.1.4/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4022 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.087030 autorag-0.1.4/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      504 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2236 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3979 2024-03-17 04:13:16.000000 autorag-0.1.4/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3936 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2612 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2373 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3713 2024-04-06 14:23:40.000000 autorag-0.1.4/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4186 2024-03-06 19:44:35.000000 autorag-0.1.4/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5697 2024-04-19 15:05:28.000000 autorag-0.1.4/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      618 2024-04-10 15:52:33.000000 autorag-0.1.4/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4712 2024-04-05 03:16:26.000000 autorag-0.1.4/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4167 2024-04-10 13:46:46.000000 autorag-0.1.4/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2884 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.087897 autorag-0.1.4/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4983 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3864 2024-04-22 05:42:18.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4201 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-12 13:21:50.000000 autorag-0.1.4/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7555 2024-03-06 19:44:35.000000 autorag-0.1.4/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.089208 autorag-0.1.4/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       84 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1379 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1162 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2290 2024-04-09 15:31:49.000000 autorag-0.1.4/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8925 2024-03-31 10:20:41.000000 autorag-0.1.4/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.090776 autorag-0.1.4/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      123 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1663 2024-03-06 19:11:31.000000 autorag-0.1.4/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1572 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-22 15:32:30.000000 autorag-0.1.4/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3491 2024-02-14 10:09:21.000000 autorag-0.1.4/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     7932 2024-02-15 17:29:26.000000 autorag-0.1.4/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.093188 autorag-0.1.4/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      227 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6444 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5637 2024-03-25 04:14:52.000000 autorag-0.1.4/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3122 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3221 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2957 2024-02-13 22:39:30.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4148 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    10780 2024-04-11 14:29:33.000000 autorag-0.1.4/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4651 2024-03-25 07:44:05.000000 autorag-0.1.4/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.094165 autorag-0.1.4/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)       50 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      722 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/module.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4158 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/schema/node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3996 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3985 2024-04-15 08:09:03.000000 autorag-0.1.4/autorag/support.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.094604 autorag-0.1.4/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      161 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/utils/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2611 2024-02-13 20:12:31.000000 autorag-0.1.4/autorag/utils/preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11345 2024-04-19 08:38:15.000000 autorag-0.1.4/autorag/utils/util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2563 2024-03-06 00:03:36.000000 autorag-0.1.4/autorag/web.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       73 2024-04-19 08:38:15.000000 autorag-0.1.4/dev_requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.095404 autorag-0.1.4/docs/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      638 2024-01-17 16:38:11.000000 autorag-0.1.4/docs/Makefile
+-rw-r--r--   0 jeffrey    (501) staff       (20)      804 2024-01-17 11:55:21.000000 autorag-0.1.4/docs/make.bat
+-rw-r--r--   0 jeffrey    (501) staff       (20)      125 2024-04-19 08:38:15.000000 autorag-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.097257 autorag-0.1.4/docs/source/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.104281 autorag-0.1.4/docs/source/_static/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    57124 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/data_creation.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    30770 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/data_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31538 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    18941 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    42589 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    92939 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_lines.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    95669 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/node_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    36728 2024-02-07 10:54:42.000000 autorag-0.1.4/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    19853 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/project_folders.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    22432 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.108275 autorag-0.1.4/docs/source/_static/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   159068 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    38568 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    62853 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    75826 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    82200 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    69999 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   567356 2024-02-07 10:54:42.000000 autorag-0.1.4/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 jeffrey    (501) staff       (20)    37348 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_folder.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)    25499 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_json.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   177107 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/_static/trial_summary.png
+-rw-r--r--   0 jeffrey    (501) staff       (20)   269046 2024-03-06 00:03:36.000000 autorag-0.1.4/docs/source/_static/web_interface.png
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.112935 autorag-0.1.4/docs/source/api_spec/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      563 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      939 2024-04-14 04:49:44.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      287 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      358 2024-03-22 04:34:21.000000 autorag-0.1.4/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      984 2024-02-10 14:23:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      962 2024-02-10 14:23:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      941 2024-03-17 04:13:16.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1294 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1471 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3229 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      952 2024-02-01 16:32:39.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      995 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1254 2024-02-22 15:32:30.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1688 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      432 2024-04-10 13:46:46.000000 autorag-0.1.4/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1239 2024-03-07 15:58:42.000000 autorag-0.1.4/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      486 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)      489 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)       58 2024-01-17 15:59:52.000000 autorag-0.1.4/docs/source/api_spec/modules.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1454 2024-04-19 08:38:15.000000 autorag-0.1.4/docs/source/conf.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.113728 autorag-0.1.4/docs/source/data_creation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5072 2024-02-18 20:58:37.000000 autorag-0.1.4/docs/source/data_creation/data_format.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2206 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/data_creation/ragas.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5543 2024-03-25 11:47:15.000000 autorag-0.1.4/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.114364 autorag-0.1.4/docs/source/deploy/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1473 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      912 2024-03-06 00:03:36.000000 autorag-0.1.4/docs/source/deploy/web.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4124 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/index.rst
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1891 2024-02-15 09:50:25.000000 autorag-0.1.4/docs/source/install.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6153 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/local_model.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.114606 autorag-0.1.4/docs/source/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.115360 autorag-0.1.4/docs/source/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2703 2024-04-05 14:53:42.000000 autorag-0.1.4/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1306 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1358 2024-03-14 09:00:38.000000 autorag-0.1.4/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      172 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/index.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.116044 autorag-0.1.4/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3046 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1182 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1252 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.116986 autorag-0.1.4/docs/source/nodes/passage_filter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1765 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1127 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1028 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1085 2024-04-10 13:46:46.000000 autorag-0.1.4/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.120224 autorag-0.1.4/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1151 2024-03-17 04:13:16.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      521 2024-04-08 12:04:54.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      675 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      654 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1232 2024-04-06 14:23:40.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      366 2024-02-22 16:33:58.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1567 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2372 2024-04-15 08:09:03.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-04-05 03:16:26.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      645 2024-04-08 08:26:20.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      515 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      561 2024-04-12 13:21:50.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1435 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.121020 autorag-0.1.4/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      585 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)      815 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2689 2024-04-09 15:31:49.000000 autorag-0.1.4/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.121526 autorag-0.1.4/docs/source/nodes/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1178 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1330 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3272 2024-02-22 15:32:30.000000 autorag-0.1.4/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.123164 autorag-0.1.4/docs/source/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      625 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2216 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2294 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2053 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2304 2024-04-10 06:33:52.000000 autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1910 2024-04-11 14:29:33.000000 autorag-0.1.4/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1223 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.124265 autorag-0.1.4/docs/source/optimization/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4160 2024-02-15 10:23:20.000000 autorag-0.1.4/docs/source/optimization/custom_config.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3779 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4596 2024-02-07 21:46:19.000000 autorag-0.1.4/docs/source/optimization/optimization.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2580 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.124486 autorag-0.1.4/docs/source/roadmap/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6735 2024-02-07 21:45:07.000000 autorag-0.1.4/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3032 2024-02-08 11:27:02.000000 autorag-0.1.4/docs/source/structure.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3121 2024-02-18 20:58:37.000000 autorag-0.1.4/docs/source/troubleshooting.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8338 2024-03-29 05:05:10.000000 autorag-0.1.4/docs/source/tutorial.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1529 2024-02-18 20:58:37.000000 autorag-0.1.4/pyproject.toml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1149 2024-04-12 13:21:50.000000 autorag-0.1.4/requirements.txt
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126343 autorag-0.1.4/sample_config/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2101 2024-03-14 09:00:38.000000 autorag-0.1.4/sample_config/compact_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2420 2024-03-17 04:13:16.000000 autorag-0.1.4/sample_config/compact_openai.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1222 2024-03-17 04:13:16.000000 autorag-0.1.4/sample_config/config_korean.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      976 2024-03-06 00:03:36.000000 autorag-0.1.4/sample_config/extracted_sample.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4448 2024-04-15 08:09:03.000000 autorag-0.1.4/sample_config/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      896 2024-03-14 09:00:38.000000 autorag-0.1.4/sample_config/simple_local.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)      863 2024-02-08 11:27:02.000000 autorag-0.1.4/sample_config/simple_openai.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126595 autorag-0.1.4/sample_dataset/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1404 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.126959 autorag-0.1.4/sample_dataset/eli5/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1109 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.127211 autorag-0.1.4/sample_dataset/msmarco/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1167 2024-02-05 20:46:09.000000 autorag-0.1.4/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.127503 autorag-0.1.4/sample_dataset/triviaqa/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1171 2024-02-07 10:54:45.000000 autorag-0.1.4/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2024-04-22 06:04:28.186829 autorag-0.1.4/setup.cfg
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.128222 autorag-0.1.4/tests/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.129881 autorag-0.1.4/tests/autorag/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.060481 autorag-0.1.4/tests/autorag/data/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.130777 autorag-0.1.4/tests/autorag/data/corpus/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      620 2024-03-22 04:29:06.000000 autorag-0.1.4/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      642 2024-03-22 04:29:59.000000 autorag-0.1.4/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      977 2024-03-25 07:44:05.000000 autorag-0.1.4/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.131780 autorag-0.1.4/tests/autorag/data/qacreation/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1758 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3129 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      897 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2097 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.132712 autorag-0.1.4/tests/autorag/evaluate/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.133391 autorag-0.1.4/tests/autorag/evaluate/metric/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3551 2024-04-05 14:53:42.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1578 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1569 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1263 2024-03-08 17:59:53.000000 autorag-0.1.4/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4701 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1460 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2007 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.061334 autorag-0.1.4/tests/autorag/nodes/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.134396 autorag-0.1.4/tests/autorag/nodes/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      687 2024-03-08 18:01:40.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1372 2024-03-08 17:13:58.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3263 2024-03-31 05:05:12.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1004 2024-03-08 18:15:21.000000 autorag-0.1.4/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.135823 autorag-0.1.4/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      820 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1852 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5091 2024-02-22 16:01:50.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1933 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.137371 autorag-0.1.4/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      710 2024-04-11 14:32:56.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3615 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2999 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      981 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3799 2024-04-15 08:09:03.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      860 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.141569 autorag-0.1.4/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      795 2024-03-17 04:13:16.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1105 2024-04-08 12:04:54.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1078 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1159 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1524 2024-04-06 14:23:40.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1063 2024-02-22 16:33:58.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      818 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4364 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4830 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1795 2024-04-05 03:16:26.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1120 2024-04-08 08:26:20.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      963 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1210 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      956 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.142186 autorag-0.1.4/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1373 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1798 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      580 2024-04-09 15:31:49.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8310 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.143336 autorag-0.1.4/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      813 2024-02-22 15:48:12.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      544 2024-02-22 15:32:30.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      991 2024-02-22 15:56:28.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1586 2024-02-15 09:47:24.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6880 2024-02-22 16:17:25.000000 autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.145475 autorag-0.1.4/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2906 2024-03-25 03:54:12.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4013 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1525 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      879 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2989 2024-04-10 06:33:52.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      780 2024-04-11 14:29:33.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2976 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    11185 2024-03-23 14:00:14.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3757 2024-03-25 07:44:05.000000 autorag-0.1.4/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.146442 autorag-0.1.4/tests/autorag/schema/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1033 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5515 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3118 2024-03-29 05:05:10.000000 autorag-0.1.4/tests/autorag/test_cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6869 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/autorag/test_deploy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14669 2024-04-19 08:38:15.000000 autorag-0.1.4/tests/autorag/test_evaluator.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2081 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/test_strategy.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      306 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/test_support.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      878 2024-03-06 00:03:36.000000 autorag-0.1.4/tests/autorag/test_web.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.147040 autorag-0.1.4/tests/autorag/utils/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2491 2024-02-13 20:13:32.000000 autorag-0.1.4/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9696 2024-04-12 13:21:50.000000 autorag-0.1.4/tests/autorag/utils/test_util.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      124 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/conftest.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      672 2024-02-18 20:58:37.000000 autorag-0.1.4/tests/delete_tests.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2641 2024-02-22 16:04:39.000000 autorag-0.1.4/tests/mock.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.149649 autorag-0.1.4/tests/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      796 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/README.md
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.4/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.061800 autorag-0.1.4/tests/resources/data_creation/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.150554 autorag-0.1.4/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3379 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3243 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4563 2024-02-08 11:27:05.000000 autorag-0.1.4/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3235 2024-04-12 16:43:24.000000 autorag-0.1.4/tests/resources/full.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.4/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.151376 autorag-0.1.4/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      198 2024-04-17 01:53:11.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      186 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      202 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)     5910 2024-02-07 10:54:45.000000 autorag-0.1.4/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.152210 autorag-0.1.4/tests/resources/result_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.152692 autorag-0.1.4/tests/resources/result_project/0/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2297 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.153001 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.155530 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    23516 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26448 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    33716 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14618 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14683 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    13278 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    54234 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1155 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.156533 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8443 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    41557 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      513 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      368 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.156765 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.158056 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.158184 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.159101 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.160483 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.161889 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      845 2024-02-18 14:46:34.000000 autorag-0.1.4/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.162261 autorag-0.1.4/tests/resources/result_project/1/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.162840 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.164411 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.063587 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.164577 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.165637 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167245 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167489 autorag-0.1.4/tests/resources/result_project/2/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2458 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.063845 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.167724 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8548 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.168306 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.169746 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3100 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     3769 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    28924 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    14607 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      495 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      187 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.169898 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.170546 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9073 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    31124 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      340 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.173426 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67610 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    67719 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    84239 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      322 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.175403 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   103655 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)    86579 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)   117633 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)      307 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 jeffrey    (501) staff       (20)      321 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.175618 autorag-0.1.4/tests/resources/result_project/3/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      682 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2307 2024-03-29 05:05:10.000000 autorag-0.1.4/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176421 autorag-0.1.4/tests/resources/result_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176727 autorag-0.1.4/tests/resources/result_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-02-03 19:10:47.000000 autorag-0.1.4/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.176981 autorag-0.1.4/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.183652 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 jeffrey    (501) staff       (20)  6284000 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)      100 2024-02-18 14:41:00.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)     4000 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2024-02-18 14:41:00.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 jeffrey    (501) staff       (20)   352256 2024-02-18 14:41:41.000000 autorag-0.1.4/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 jeffrey    (501) staff       (20)      338 2024-03-25 11:47:36.000000 autorag-0.1.4/tests/resources/result_project/trial.json
+-rw-r--r--   0 jeffrey    (501) staff       (20)     8439 2024-03-23 03:44:06.000000 autorag-0.1.4/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.065081 autorag-0.1.4/tests/resources/sample_project/
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.184630 autorag-0.1.4/tests/resources/sample_project/data/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   111931 2024-01-31 17:28:04.000000 autorag-0.1.4/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 jeffrey    (501) staff       (20)     9928 2024-01-15 05:15:36.000000 autorag-0.1.4/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2024-04-22 06:04:28.184991 autorag-0.1.4/tests/resources/sample_project/resources/
+-rw-r--r--   0 jeffrey    (501) staff       (20)   109454 2024-01-13 07:56:04.000000 autorag-0.1.4/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 jeffrey    (501) staff       (20)      893 2024-04-10 13:46:46.000000 autorag-0.1.4/tests/resources/simple.yaml
+-rw-r--r--   0 jeffrey    (501) staff       (20)    26773 2024-01-13 07:56:04.000000 autorag-0.1.4/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.3/.github/workflows/sphinx.yml` & `autorag-0.1.4/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/.github/workflows/test.yml` & `autorag-0.1.4/.github/workflows/test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
+  pull_request_target:
+    branches:
+      - main
 
 env:
   OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
   COHERE_API_KEY: ${{ secrets.COHERE_API_KEY }}
   JINAAI_API_KEY: ${{ secrets.JINAAI_API_KEY }}
 
 jobs:
@@ -25,13 +28,13 @@
         run: |
           sudo apt-get install gcc
       - name: Install AutoRAG
         run: |
           pip install -e .
       - name: Install dependencies
         run: |
-          pip install pytest pytest-xdist
+          pip install pytest pytest-xdist pytest-asyncio
       - name: delete tests package
         run: python3 tests/delete_tests.py
       - name: Run tests
         run: |
           python3 -m pytest -o log_cli=true --log-cli-level=INFO -n auto tests/
```

### Comparing `autorag-0.1.3/.gitignore` & `autorag-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.4/AutoRAG.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -496,16 +496,14 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
-
-
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
 - [x] Token usage strategy
```

### Comparing `autorag-0.1.3/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.4/AutoRAG.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 dev_requirements.txt
 pyproject.toml
 requirements.txt
 .github/dependabot.yml
 .github/workflows/sphinx.yml
@@ -53,20 +55,22 @@
 autorag/nodes/generator/base.py
 autorag/nodes/generator/llama_index_llm.py
 autorag/nodes/generator/run.py
 autorag/nodes/generator/vllm.py
 autorag/nodes/passagecompressor/__init__.py
 autorag/nodes/passagecompressor/base.py
 autorag/nodes/passagecompressor/pass_compressor.py
+autorag/nodes/passagecompressor/refine.py
 autorag/nodes/passagecompressor/run.py
 autorag/nodes/passagecompressor/tree_summarize.py
 autorag/nodes/passagefilter/__init__.py
 autorag/nodes/passagefilter/base.py
 autorag/nodes/passagefilter/pass_passage_filter.py
 autorag/nodes/passagefilter/percentile_cutoff.py
+autorag/nodes/passagefilter/recency.py
 autorag/nodes/passagefilter/run.py
 autorag/nodes/passagefilter/threshold_cutoff.py
 autorag/nodes/passagereranker/__init__.py
 autorag/nodes/passagereranker/base.py
 autorag/nodes/passagereranker/cohere.py
 autorag/nodes/passagereranker/colbert.py
 autorag/nodes/passagereranker/flag_embedding.py
@@ -166,16 +170,18 @@
 docs/source/deploy/api_endpoint.md
 docs/source/deploy/web.md
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_compressor/passage_compressor.md
+docs/source/nodes/passage_compressor/refine.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_filter/passage_filter.md
+docs/source/nodes/passage_filter/recency_filter.md
 docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
 docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
 docs/source/nodes/passage_reranker/cohere.md
 docs/source/nodes/passage_reranker/colbert.md
 docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
 docs/source/nodes/passage_reranker/flag_embedding_reranker.md
 docs/source/nodes/passage_reranker/jina_reranker.md
@@ -239,21 +245,24 @@
 tests/autorag/evaluate/metric/test_generation_metric.py
 tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
 tests/autorag/evaluate/metric/test_retrieval_metric.py
 tests/autorag/nodes/generator/test_generator_base.py
 tests/autorag/nodes/generator/test_llama_index_llm.py
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
+tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
 tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+tests/autorag/nodes/passagecompressor/test_refine.py
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
 tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
 tests/autorag/nodes/passagefilter/test_passage_filter_base.py
 tests/autorag/nodes/passagefilter/test_passage_filter_run.py
 tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+tests/autorag/nodes/passagefilter/test_recency_filter.py
 tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
 tests/autorag/nodes/passagereranker/test_cohere_reranker.py
 tests/autorag/nodes/passagereranker/test_colbert_reranker.py
 tests/autorag/nodes/passagereranker/test_flag_embedding.py
 tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
 tests/autorag/nodes/passagereranker/test_jina_reranker.py
 tests/autorag/nodes/passagereranker/test_koreranker.py
```

### Comparing `autorag-0.1.3/AutoRAG.egg-info/requires.txt` & `autorag-0.1.4/AutoRAG.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/LICENSE` & `autorag-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/PKG-INFO` & `autorag-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -496,16 +496,14 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
-
-
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
 - [x] Token usage strategy
```

### Comparing `autorag-0.1.3/README.md` & `autorag-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,14 @@
 ```
 
 # ❗Supporting Nodes & modules
 
 You can check our all supporting Nodes & modules
 at [here](https://edai.notion.site/Supporting-Nodes-modules-0ebc7810649f4e41aead472a92976be4?pvs=4)
 
-
-
 # 🛣Roadmap
 
 - [ ] Policy Module for modular RAG pipeline
 - [ ] Visualize evaluation result
 - [ ] Visualize config yaml file
 - [ ] More RAG modules support
 - [x] Token usage strategy
```

### Comparing `autorag-0.1.3/autorag/__init__.py` & `autorag-0.1.4/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/cli.py` & `autorag-0.1.4/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/corpus/langchain.py` & `autorag-0.1.4/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/corpus/llama_index.py` & `autorag-0.1.4/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/qacreation/base.py` & `autorag-0.1.4/autorag/data/qacreation/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import uuid
 from typing import Callable, Optional
 
 import pandas as pd
 
 from autorag.utils.util import save_parquet_safe
 
+logger = logging.getLogger("AutoRAG")
+
 
 def make_single_content_qa(corpus_df: pd.DataFrame,
                            content_size: int,
                            qa_creation_func: Callable,
                            output_filepath: Optional[str] = None,
                            upsert: bool = False,
                            random_state: int = 42,
@@ -29,14 +32,19 @@
     :param upsert: If true, the function will overwrite the existing file if it exists.
         Default is False.
     :param random_state: The random state for sampling corpus from the given corpus_df.
     :param kwargs: The keyword arguments for qa_creation_func.
     :return: QA dataset dataframe.
         You can save this as parquet file to use at AutoRAG.
     """
+    assert content_size > 0, "content_size must be greater than 0."
+    if content_size > len(corpus_df):
+        logger.warning(f"content_size {content_size} is larger than the corpus size {len(corpus_df)}. "
+                       "Setting content_size to the corpus size.")
+        content_size = len(corpus_df)
     sampled_corpus = corpus_df.sample(n=content_size, random_state=random_state)
     sampled_corpus = sampled_corpus.reset_index(drop=True)
 
     qa = qa_creation_func(contents=sampled_corpus['contents'].tolist(), **kwargs)
     qa_data = pd.DataFrame({
         'qid': [str(uuid.uuid4()) for _ in range(len(qa))],
         'qa': qa,
```

### Comparing `autorag-0.1.3/autorag/data/qacreation/llama_index.py` & `autorag-0.1.4/autorag/data/qacreation/llama_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import os.path
 import random
 from typing import Optional, List, Dict, Any
 
+import pandas as pd
 from llama_index.core.service_context_elements.llm_predictor import LLMPredictorType
 
 from autorag.utils.util import process_batch
 
 package_dir = os.path.dirname(os.path.realpath(__file__))
 
 
@@ -85,22 +86,28 @@
     :param batch: The batch size to process asynchronously.
         Default is 4.
     :return: 2-d list of dictionaries containing the query and generation_gt.
     """
     prompts = list(map(lambda path: open(path, 'r').read(), prompts_ratio.keys()))
     assert all([validate_llama_index_prompt(prompt) for prompt in prompts])
 
+    content_indices = list(range(len(contents)))
     random.seed(random_state)
-    random.shuffle(contents)
+    random.shuffle(content_indices)
+
+    slice_content_indices: List[List[str]] = distribute_list_by_ratio(content_indices, list(prompts_ratio.values()))
+    temp_df = pd.DataFrame({'idx': slice_content_indices, 'prompt': prompts})
+    temp_df = temp_df.explode('idx', ignore_index=True)
+    temp_df = temp_df.sort_values(by='idx', ascending=True)
+
+    final_df = pd.DataFrame({'content': contents, 'prompt': temp_df['prompt'].tolist()})
 
-    slice_contents: List[List[str]] = distribute_list_by_ratio(contents, list(prompts_ratio.values()))
     tasks = [
         async_qa_gen_llama_index(content, llm, prompt, question_num_per_content, max_retries)
-        for prompt, type_contents in zip(prompts, slice_contents)
-        for content in type_contents
+        for content, prompt in zip(final_df['content'].tolist(), final_df['prompt'].tolist())
     ]
 
     loops = asyncio.get_event_loop()
     results = loops.run_until_complete(process_batch(tasks, batch))
 
     return results
```

### Comparing `autorag-0.1.3/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.4/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/qacreation/ragas.py` & `autorag-0.1.4/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/qacreation/simple.py` & `autorag-0.1.4/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/data/utils/util.py` & `autorag-0.1.4/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/deploy.py` & `autorag-0.1.4/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/generation.py` & `autorag-0.1.4/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.4/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/generation.py` & `autorag-0.1.4/autorag/evaluate/metric/generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import evaluate
 import pandas as pd
 import sacrebleu
 import torch
 from llama_index.core.embeddings import BaseEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
-from openai import OpenAI
+from openai import AsyncOpenAI
 from rouge_score import tokenizers
 from rouge_score.rouge_scorer import RougeScorer
 
 from autorag import embedding_models
 from autorag.evaluate.metric.util import calculate_cosine_similarity
 from autorag.utils.util import process_batch, openai_truncate_by_token
 
@@ -190,33 +190,47 @@
     del embedding_model
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
     return result
 
 
-@generation_metric
-def g_eval(generation_gt: List[str], pred: str,
+def g_eval(generation_gt: List[List[str]], generations: List[str],
            metrics: Optional[List[str]] = None,
            model: str = 'gpt-4-0125-preview',
-           ) -> float:
+           batch_size: int = 8) -> List[float]:
     """
-    Calculate G-Eval score.
-    G-eval is a metric that uses high-performance LLM model to evaluate generation performance.
-    It evaluates the generation result by coherence, consistency, fluency, and relevance.
-    It uses only 'openai' model, and we recommend to use gpt-4 for evaluation accuracy.
+        Calculate G-Eval score.
+        G-eval is a metric that uses high-performance LLM model to evaluate generation performance.
+        It evaluates the generation result by coherence, consistency, fluency, and relevance.
+        It uses only 'openai' model, and we recommend to use gpt-4 for evaluation accuracy.
 
-    :param generation_gt: A list of ground truth.
-    :param pred: Model generation.
-    :param metrics: A list of metrics to use for evaluation.
-        Default is all metrics, which is ['coherence', 'consistency', 'fluency', 'relevance'].
-    :param model: OpenAI model name.
-        Default is 'gpt-4-0125-preview'.
-    :return: G-Eval score.
+        :param generation_gt: A list of ground truth.
+            Must be 2-d list of string.
+            Because it can be a multiple ground truth.
+            It will get the max of g_eval score.
+        :param generations: A list of generations that LLM generated.
+        :param metrics: A list of metrics to use for evaluation.
+            Default is all metrics, which is ['coherence', 'consistency', 'fluency', 'relevance'].
+        :param model: OpenAI model name.
+            Default is 'gpt-4-0125-preview'.
+        :param batch_size: The batch size for processing.
+            Default is 8.
+        :return: G-Eval score.
     """
+    loop = asyncio.get_event_loop()
+    tasks = [async_g_eval(gt, pred, metrics, model) for gt, pred in zip(generation_gt, generations)]
+    result = loop.run_until_complete(process_batch(tasks, batch_size=batch_size))
+    return result
+
+
+async def async_g_eval(generation_gt: List[str], pred: str,
+                       metrics: Optional[List[str]] = None,
+                       model: str = 'gpt-4-0125-preview',
+                       ) -> float:
     available_metrics = ['coherence', 'consistency', 'fluency', 'relevance']
     if metrics is None:
         metrics = available_metrics
     else:
         assert len(metrics) > 0, "metrics must be a list of string"
         metrics = [metric for metric in metrics if metric in available_metrics]
 
@@ -225,21 +239,21 @@
     g_eval_prompts = {
         "coherence": open(os.path.join(prompt_path, "coh_detailed.txt")).read(),
         "consistency": open(os.path.join(prompt_path, "con_detailed.txt")).read(),
         "fluency": open(os.path.join(prompt_path, "flu_detailed.txt")).read(),
         "relevance": open(os.path.join(prompt_path, "rel_detailed.txt")).read(),
     }
 
-    client = OpenAI()
+    client = AsyncOpenAI()
 
-    def g_eval_score(prompt: str, gen_gt: List[str], pred: str):
+    async def g_eval_score(prompt: str, gen_gt: List[str], pred: str):
         scores = []
         for gt in gen_gt:
             input_prompt = prompt.replace('{{Document}}', gt).replace('{{Summary}}', pred)
-            response = client.chat.completions.create(
+            response = await client.chat.completions.create(
                 model=model,
                 messages=[
                     {"role": "system", "content": input_prompt}
                 ],
                 logprobs=True,
                 top_logprobs=5,
                 temperature=0,
@@ -261,15 +275,15 @@
             first_top_log_probs = choice.logprobs.content[0].top_logprobs
             for i, top_log_prob in enumerate(list(map(lambda x: x.token, first_top_log_probs))):
                 if top_log_prob in target_tokens:
                     target_tokens[top_log_prob] += (5 - i)
 
         return int(max(target_tokens, key=target_tokens.get))
 
-    g_eval_scores = list(map(lambda x: g_eval_score(g_eval_prompts[x], generation_gt, pred), metrics))
+    g_eval_scores = await asyncio.gather(*(g_eval_score(g_eval_prompts[x], generation_gt, pred) for x in metrics))
     return sum(g_eval_scores) / len(g_eval_scores)
 
 
 def bert_score(generation_gt: List[List[str]], generations: List[str],
                lang: str = 'en',
                batch: int = 128,
                n_threads: int = os.cpu_count()) -> List[float]:
```

### Comparing `autorag-0.1.3/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.4/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.4/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/retrieval.py` & `autorag-0.1.4/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/retrieval_contents.py` & `autorag-0.1.4/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluate/util.py` & `autorag-0.1.4/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/evaluator.py` & `autorag-0.1.4/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/node_line.py` & `autorag-0.1.4/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/generator/base.py` & `autorag-0.1.4/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.4/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/generator/run.py` & `autorag-0.1.4/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/generator/vllm.py` & `autorag-0.1.4/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.4/autorag/nodes/passagecompressor/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         assert len(previous_result) > 0, "previous_result must have at least one row."
 
         queries = previous_result['query'].tolist()
         retrieved_contents = previous_result['retrieved_contents'].tolist()
         retrieved_ids = previous_result['retrieved_ids'].tolist()
         retrieve_scores = previous_result['retrieve_scores'].tolist()
 
-        if func.__name__ == 'tree_summarize':
+        if func.__name__ in ['tree_summarize', 'refine']:
             param_list = ['prompt', 'chat_prompt', 'context_window', 'num_output', 'batch']
             param_dict = dict(filter(lambda x: x[0] in param_list, kwargs.items()))
             kwargs_dict = dict(filter(lambda x: x[0] not in param_list, kwargs.items()))
             llm_name = kwargs_dict.pop('llm')
             llm = make_llm(llm_name, kwargs_dict)
             result = func(
                 queries=queries,
```

### Comparing `autorag-0.1.3/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.4/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.4/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagefilter/base.py` & `autorag-0.1.4/autorag/nodes/passagereranker/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import functools
+import logging
+import os
 from pathlib import Path
-from typing import Union, Tuple, List
+from typing import List, Union, Tuple
 
 import pandas as pd
 
-from autorag.utils import result_to_dataframe, validate_qa_dataset
+from autorag.utils import result_to_dataframe, validate_qa_dataset, fetch_contents
 
+logger = logging.getLogger("AutoRAG")
 
-# same with passage filter from now
-def passage_filter_node(func):
+
+def passage_reranker_node(func):
     @functools.wraps(func)
-    @result_to_dataframe(['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
+    @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
         validate_qa_dataset(previous_result)
 
         # find queries columns
@@ -29,13 +32,21 @@
         assert "retrieve_scores" in previous_result.columns, "previous_result must have retrieve_scores column."
         scores = previous_result["retrieve_scores"].tolist()
 
         # find ids columns
         assert "retrieved_ids" in previous_result.columns, "previous_result must have retrieved_ids column."
         ids = previous_result["retrieved_ids"].tolist()
 
-        filtered_contents, filtered_ids, filtered_scores = func(queries=queries, contents_list=contents,
-                                                                scores_list=scores, ids_list=ids, *args, **kwargs)
+        # time rerankers
+        if func.__name__ == 'time_reranker':
+            corpus_df = pd.read_parquet(os.path.join(project_dir, "data", "corpus.parquet"))
+            metadatas = fetch_contents(corpus_df, ids, column_name='metadata')
+            times = [[time['last_modified_datetime'] for time in time_list] for time_list in metadatas]
+            reranked_contents, reranked_ids, reranked_scores \
+                = func(contents_list=contents, scores_list=scores, ids_list=ids, time_list=times, *args, **kwargs)
+        else:
+            reranked_contents, reranked_ids, reranked_scores \
+                = func(queries=queries, contents_list=contents, scores_list=scores, ids_list=ids, *args, **kwargs)
 
-        return filtered_contents, filtered_ids, filtered_scores
+        return reranked_contents, reranked_ids, reranked_scores
 
     return wrapper
```

### Comparing `autorag-0.1.3/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.4/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagefilter/run.py` & `autorag-0.1.4/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.4/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/base.py` & `autorag-0.1.4/autorag/nodes/passagefilter/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import functools
-import logging
 import os
 from pathlib import Path
-from typing import List, Union, Tuple
+from typing import Union, Tuple, List
 
 import pandas as pd
 
 from autorag.utils import result_to_dataframe, validate_qa_dataset, fetch_contents
 
-logger = logging.getLogger("AutoRAG")
 
-
-def passage_reranker_node(func):
+# same with passage filter from now
+def passage_filter_node(func):
     @functools.wraps(func)
-    @result_to_dataframe(["retrieved_contents", "retrieved_ids", "retrieve_scores"])
+    @result_to_dataframe(['retrieved_contents', 'retrieved_ids', 'retrieve_scores'])
     def wrapper(
             project_dir: Union[str, Path],
             previous_result: pd.DataFrame,
             *args, **kwargs) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
         validate_qa_dataset(previous_result)
 
         # find queries columns
@@ -32,21 +30,20 @@
         assert "retrieve_scores" in previous_result.columns, "previous_result must have retrieve_scores column."
         scores = previous_result["retrieve_scores"].tolist()
 
         # find ids columns
         assert "retrieved_ids" in previous_result.columns, "previous_result must have retrieved_ids column."
         ids = previous_result["retrieved_ids"].tolist()
 
-        # time rerankers
-        if func.__name__ == 'time_reranker':
+        if func.__name__ == 'recency_filter':
             corpus_df = pd.read_parquet(os.path.join(project_dir, "data", "corpus.parquet"))
             metadatas = fetch_contents(corpus_df, ids, column_name='metadata')
             times = [[time['last_modified_datetime'] for time in time_list] for time_list in metadatas]
-            reranked_contents, reranked_ids, reranked_scores \
+            filtered_contents, filtered_ids, filtered_scores \
                 = func(contents_list=contents, scores_list=scores, ids_list=ids, time_list=times, *args, **kwargs)
         else:
-            reranked_contents, reranked_ids, reranked_scores \
-                = func(queries=queries, contents_list=contents, scores_list=scores, ids_list=ids, *args, **kwargs)
+            filtered_contents, filtered_ids, filtered_scores = func(queries=queries, contents_list=contents,
+                                                                    scores_list=scores, ids_list=ids, *args, **kwargs)
 
-        return reranked_contents, reranked_ids, reranked_scores
+        return filtered_contents, filtered_ids, filtered_scores
 
     return wrapper
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.4/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.4/autorag/nodes/passagereranker/colbert.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import asyncio
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 from transformers import AutoModel, AutoTokenizer
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.utils.util import process_batch
+from autorag.utils.util import make_batch, select_top_k, flatten_apply, sort_by_scores
 
 
 @passage_reranker_node
 def colbert_reranker(queries: List[str], contents_list: List[List[str]],
                      scores_list: List[List[float]], ids_list: List[List[str]],
                      top_k: int, batch: int = 64,
                      model_name: str = "colbert-ir/colbertv2.0",
@@ -31,47 +31,56 @@
         Default is "colbert-ir/colbertv2.0".
     :return: Tuple of lists containing the reranked contents, ids, and scores
     """
     device = "cuda" if torch.cuda.is_available() else "cpu"
     model = AutoModel.from_pretrained(model_name).to(device)
     tokenizer = AutoTokenizer.from_pretrained(model_name)
 
-    # Run async cohere_rerank_pure function
-    tasks = [get_colbert_score(query, document, model, tokenizer) for query, document, ids in
-             zip(queries, contents_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    score_results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
+    nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
+
+    rerank_scores = flatten_apply(colbert_run_model, nested_list, model=model,
+                                  tokenizer=tokenizer, batch_size=batch, device=device)
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
+    if torch.cuda.is_available():
+        torch.cuda.empty_cache()
 
-    def rerank_results(contents, ids, scores, top_k):
-        reranked_content, reranked_id, reranked_score = zip(
-            *sorted(zip(contents, ids, scores), key=lambda x: x[2], reverse=True))
-        return list(reranked_content)[:top_k], list(reranked_id)[:top_k], list(reranked_score)[:top_k]
-
-    reranked_contents_list, reranked_ids_list, reranked_scores_list = zip(*list(map(
-        rerank_results, contents_list, ids_list, score_results, [top_k] * len(contents_list))))
-    return list(reranked_contents_list), list(reranked_ids_list), list(reranked_scores_list)
-
-
-async def get_colbert_score(query: str, content_list: List[str],
-                            model, tokenizer) -> List[float]:
-    query_encoding = tokenizer(query, return_tensors="pt")
-    query_embedding = model(**query_encoding).last_hidden_state
-    rerank_score_list = []
-
-    for document_text in content_list:
-        document_encoding = tokenizer(
-            document_text, return_tensors="pt", truncation=True, max_length=512
-        )
-        document_embedding = model(**document_encoding).last_hidden_state
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
+
+
+def colbert_run_model(contents_list, model, tokenizer, device, batch_size: int):
+    batch_contents_list = make_batch(contents_list, batch_size)
+    results = []
+
+    for batch_contents in batch_contents_list:
+        flattened_batch_queries, flattened_batch_contents = map(list, zip(*batch_contents))
+
+        # Tokenize both queries and contents together
+        feature = tokenizer(flattened_batch_queries, flattened_batch_contents, padding=True, truncation=True,
+                            return_tensors="pt").to(device)
+
+        # Process the combined feature through the model in one go
+        outputs = model(**feature)
+        last_hidden_state = outputs.last_hidden_state
+
+        # Split the embeddings back into query and content parts
+        num_queries = len(flattened_batch_queries)
+        query_embedding, content_embedding = last_hidden_state.split(
+            [num_queries, last_hidden_state.size(1) - num_queries], dim=1)
 
+        # Calculate cosine similarity between query and content embeddings
         sim_matrix = torch.nn.functional.cosine_similarity(
-            query_embedding.unsqueeze(2), document_embedding.unsqueeze(1), dim=-1
+            query_embedding.unsqueeze(2), content_embedding.unsqueeze(1), dim=-1
         )
 
         # Take the maximum similarity for each query token (across all document tokens)
-        # sim_matrix shape: [batch_size, query_length, doc_length]
         max_sim_scores, _ = torch.max(sim_matrix, dim=2)
-        rerank_score_list.append(torch.mean(max_sim_scores, dim=1))
+        results.extend(torch.mean(max_sim_scores, dim=1))
 
-    return list(map(float, rerank_score_list))
+    return list(map(float, results))
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import asyncio
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 from FlagEmbedding import FlagReranker
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.utils.util import process_batch
+from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 
 @passage_reranker_node
 def flag_embedding_reranker(queries: List[str], contents_list: List[List[str]],
                             scores_list: List[List[float]], ids_list: List[List[str]],
                             top_k: int, batch: int = 64, use_fp16: bool = False,
                             model_name: str = "BAAI/bge-reranker-large",
@@ -27,52 +27,33 @@
     :param model_name: The name of the BAAI Reranker normal-model name.
         Default is "BAAI/bge-reranker-large"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
     model = FlagReranker(
         model_name_or_path=model_name, use_fp16=use_fp16
     )
-    tasks = [flag_embedding_reranker_pure(query, contents, scores, top_k, ids, model)
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+    nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
+    rerank_scores = flatten_apply(flag_embedding_run_model, nested_list, model=model, batch_size=batch)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
-
-
-async def flag_embedding_reranker_pure(query: str, contents: List[str], scores: List[float], top_k: int,
-                                       ids: List[str], model) -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using BAAI Reranker model.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param model: BAAI Reranker model.
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-    input_texts = [(query, content) for content in contents]
-    with torch.no_grad():
-        pred_scores = model.compute_score(sentence_pairs=input_texts)
-
-    content_ids_probs = list(zip(contents, ids, pred_scores))
-
-    # Sort the list of pairs based on the relevance score in descending order
-    sorted_content_ids_probs = sorted(content_ids_probs, key=lambda x: x[2], reverse=True)
-
-    # crop with top_k
-    if len(contents) < top_k:
-        top_k = len(contents)
-    sorted_content_ids_probs = sorted_content_ids_probs[:top_k]
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
-    content_result, id_result, score_result = zip(*sorted_content_ids_probs)
 
-    return list(content_result), list(id_result), list(score_result)
+def flag_embedding_run_model(input_texts, model, batch_size: int):
+    batch_input_texts = make_batch(input_texts, batch_size)
+    results = []
+    for batch_texts in batch_input_texts:
+        with torch.no_grad():
+            pred_scores = model.compute_score(sentence_pairs=batch_texts)
+        results.extend(pred_scores)
+    return results
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.4/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import asyncio
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 from FlagEmbedding import FlagLLMReranker
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.nodes.passagereranker.flag_embedding import flag_embedding_reranker_pure
-from autorag.utils.util import process_batch
+from autorag.nodes.passagereranker.flag_embedding import flag_embedding_run_model
+from autorag.utils.util import flatten_apply, sort_by_scores, select_top_k
 
 
 @passage_reranker_node
 def flag_embedding_llm_reranker(queries: List[str], contents_list: List[List[str]],
                                 scores_list: List[List[float]], ids_list: List[List[str]],
                                 top_k: int, batch: int = 64, use_fp16: bool = False,
                                 model_name: str = "BAAI/bge-reranker-v2-gemma",
@@ -28,20 +28,23 @@
     :param model_name: The name of the BAAI Reranker LLM-based-model name.
         Default is "BAAI/bge-reranker-v2-gemma"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
     model = FlagLLMReranker(
         model_name_or_path=model_name, use_fp16=use_fp16
     )
-    tasks = [flag_embedding_reranker_pure(query, contents, scores, top_k, ids, model)
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+    nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
+    rerank_scores = flatten_apply(flag_embedding_run_model, nested_list, model=model, batch_size=batch)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.4/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.4/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.4/autorag/nodes/passagereranker/monot5.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import asyncio
+from itertools import chain
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 from transformers import T5Tokenizer, T5ForConditionalGeneration
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
+from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 prediction_tokens = {
     'castorini/monot5-base-msmarco': ['▁false', '▁true'],
     'castorini/monot5-base-msmarco-10k': ['▁false', '▁true'],
     'castorini/monot5-large-msmarco': ['▁false', '▁true'],
     'castorini/monot5-large-msmarco-10k': ['▁false', '▁true'],
     'castorini/monot5-base-med-msmarco': ['▁false', '▁true'],
@@ -29,104 +31,81 @@
     'unicamp-dl/mt5-13b-mmarco-100k': ['▁', '▁true'],
 }
 
 
 @passage_reranker_node
 def monot5(queries: List[str], contents_list: List[List[str]],
            scores_list: List[List[float]], ids_list: List[List[str]],
-           top_k: int, model_name: str = 'castorini/monot5-3b-msmarco-10k') \
+           top_k: int, model_name: str = 'castorini/monot5-3b-msmarco-10k',
+           batch: int = 64, ) \
         -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
     Rerank a list of contents based on their relevance to a query using MonoT5.
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
     :param model_name: The name of the MonoT5 model to use for reranking
         Note: default model name is 'castorini/monot5-3b-msmarco-10k'
             If there is a '/' in the model name parameter,
             when we create the file to store the results, the path will be twisted because of the '/'.
             Therefore, it will be received as '_' instead of '/'.
+    :param batch: The number of queries to be processed in a batch
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
     # replace '_' to '/'
     if '_' in model_name:
         model_name = model_name.replace('_', '/')
     # Load the tokenizer and model from the pre-trained MonoT5 model
     tokenizer = T5Tokenizer.from_pretrained(model_name)
     model = T5ForConditionalGeneration.from_pretrained(model_name).eval()
     # Retrieve the tokens used by the model to represent false and true predictions
     token_false, token_true = prediction_tokens[model_name]
     token_false_id = tokenizer.convert_tokens_to_ids(token_false)
     token_true_id = tokenizer.convert_tokens_to_ids(token_true)
     # Determine the device to run the model on (GPU if available, otherwise CPU)
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    device = "cuda" if torch.cuda.is_available() else "cpu"
     model.to(device)
-    # Run async mono_t5_rerank_pure function
-    tasks = [mono_t5_pure(query, contents, scores, top_k, ids, model, device, tokenizer, token_false_id, token_true_id) \
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(asyncio.gather(*tasks))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+    nested_list = [list(map(lambda x: [f'Query: {query} Document: {x}'], content_list))
+                   for query, content_list in zip(queries, contents_list)]
+
+    rerank_scores = flatten_apply(monot5_run_model, nested_list, model=model, batch_size=batch, tokenizer=tokenizer,
+                                  device=device, token_false_id=token_false_id, token_true_id=token_true_id)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     del tokenizer
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
-
-
-async def mono_t5_pure(query: str, contents: List[str], scores: List[float], top_k: int,
-                       ids: List[str], model, device, tokenizer, token_false_id, token_true_id)\
-        -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using MonoT5.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param model: The MonoT5 model to use for reranking
-    :param device: The device to run the model on (GPU if available, otherwise CPU)
-    :param tokenizer: The tokenizer to use for the model
-    :param token_false_id: The id of the token used by the model to represent a false prediction
-    :param token_true_id: The id of the token used by the model to represent a true prediction
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-
-    # Format the input for the model by combining each content with the query
-    input_texts = [f'Query: {query} Document: {content}' for content in contents]
-    # Tokenize the input texts and prepare for model input
-    input_encodings = tokenizer(input_texts, padding=True, truncation=True, max_length=512, return_tensors='pt').to(
-        device)
-
-    # Generate model predictions without updating model weights
-    with torch.no_grad():
-        outputs = model.generate(input_ids=input_encodings['input_ids'],
-                                 attention_mask=input_encodings['attention_mask'],
-                                 output_scores=True,
-                                 return_dict_in_generate=True)
-
-    # Extract logits for the 'false' and 'true' tokens from the model's output
-    logits = outputs.scores[-1][:, [token_false_id, token_true_id]]
-    # Calculate the softmax probability of the 'true' token
-    probs = torch.nn.functional.softmax(logits, dim=-1)[:, 1]  # Get the probability of the 'true' token
-
-    # Create a list of tuples pairing each content with its relevance probability
-    content_ids_probs = list(zip(contents, ids, probs.tolist()))
-
-    # Sort the list of pairs based on the relevance score in descending order
-    sorted_content_ids_probs = sorted(content_ids_probs, key=lambda x: x[2], reverse=True)
-
-    # crop with top_k
-    if len(contents) < top_k:
-        top_k = len(contents)
-    sorted_content_ids_probs = sorted_content_ids_probs[:top_k]
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
-    content_result, id_result, score_result = zip(*sorted_content_ids_probs)
 
-    return list(content_result), list(id_result), list(score_result)
+def monot5_run_model(input_texts, model, batch_size: int, tokenizer, device, token_false_id, token_true_id):
+    batch_input_texts = make_batch(input_texts, batch_size)
+    results = []
+    for batch_texts in batch_input_texts:
+        flattened_batch_texts = list(chain.from_iterable(batch_texts))
+        input_encodings = tokenizer(flattened_batch_texts, padding=True, truncation=True, max_length=512,
+                                    return_tensors='pt').to(
+            device)
+        with torch.no_grad():
+            outputs = model.generate(input_ids=input_encodings['input_ids'],
+                                     attention_mask=input_encodings['attention_mask'],
+                                     output_scores=True,
+                                     return_dict_in_generate=True)
+
+        # Extract logits for the 'false' and 'true' tokens from the model's output
+        logits = outputs.scores[-1][:, [token_false_id, token_true_id]]
+        # Calculate the softmax probability of the 'true' token
+        probs = torch.nn.functional.softmax(logits, dim=-1)[:, 1]
+        results.extend(probs.tolist())
+    return results
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.4/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.4/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/run.py` & `autorag-0.1.4/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.4/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import asyncio
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 from sentence_transformers import CrossEncoder
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
-from autorag.utils.util import process_batch
+from autorag.utils.util import flatten_apply, make_batch, select_top_k, sort_by_scores
 
 
 @passage_reranker_node
 def sentence_transformer_reranker(queries: List[str], contents_list: List[List[str]],
                                   scores_list: List[List[float]], ids_list: List[List[str]],
                                   top_k: int, batch: int = 64, sentence_transformer_max_length: int = 512,
                                   model_name: str = "cross-encoder/ms-marco-MiniLM-L-2-v2",
@@ -24,56 +24,38 @@
     :param top_k: The number of passages to be retrieved
     :param batch: The number of queries to be processed in a batch
     :param sentence_transformer_max_length: The maximum length of the input text for the Sentence Transformer model
     :param model_name: The name of the Sentence Transformer model to use for reranking
         Default is "cross-encoder/ms-marco-MiniLM-L-2-v2"
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    device = "cuda" if torch.cuda.is_available() else "cpu"
     model = CrossEncoder(
         model_name, max_length=sentence_transformer_max_length, device=device
     )
-    tasks = [sentence_transformer_reranker_pure(query, contents, scores, top_k, ids, model)
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+
+    nested_list = [list(map(lambda x: [query, x], content_list)) for query, content_list in zip(queries, contents_list)]
+    rerank_scores = flatten_apply(sentence_transformer_run_model, nested_list, model=model, batch_size=batch)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
-
-
-async def sentence_transformer_reranker_pure(query: str, contents: List[str], scores: List[float], top_k: int,
-                                             ids: List[str], model) -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using Sentence Transformer model.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param model: The name of the Sentence Transformer model to use for reranking
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-    input_texts = [(query, content) for content in contents]
-    with torch.no_grad():
-        pred_scores = model.predict(sentences=input_texts, apply_softmax=True)
-
-    content_ids_probs = list(zip(contents, ids, pred_scores.tolist()))
-
-    # Sort the list of pairs based on the relevance score in descending order
-    sorted_content_ids_probs = sorted(content_ids_probs, key=lambda x: x[2], reverse=True)
-
-    # crop with top_k
-    if len(contents) < top_k:
-        top_k = len(contents)
-    sorted_content_ids_probs = sorted_content_ids_probs[:top_k]
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
-    content_result, id_result, score_result = zip(*sorted_content_ids_probs)
 
-    return list(content_result), list(id_result), list(score_result)
+def sentence_transformer_run_model(input_texts, model, batch_size: int):
+    batch_input_texts = make_batch(input_texts, batch_size)
+    results = []
+    for batch_texts in batch_input_texts:
+        with torch.no_grad():
+            pred_scores = model.predict(sentences=batch_texts, apply_softmax=True)
+        results.extend(pred_scores.tolist())
+    return results
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.4/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.1.4/autorag/nodes/passagereranker/tart/tart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import asyncio
+from itertools import chain
 from typing import List, Tuple
 
+import pandas as pd
 import torch
 import torch.nn.functional as F
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
 from autorag.nodes.passagereranker.tart.modeling_enc_t5 import EncT5ForSequenceClassification
 from autorag.nodes.passagereranker.tart.tokenization_enc_t5 import EncT5Tokenizer
+from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 
 @passage_reranker_node
 def tart(queries: List[str], contents_list: List[List[str]],
          scores_list: List[List[float]], ids_list: List[List[str]],
-         top_k: int, instruction: str = "Find passage to answer given question") \
-        -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+         top_k: int, instruction: str = "Find passage to answer given question",
+         batch: int = 64) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
     Rerank a list of contents based on their relevance to a query using Tart.
     TART is a reranker based on TART (https://github.com/facebookresearch/tart).
     You can rerank the passages with the instruction using TARTReranker.
     The default model is facebook/tart-full-flan-t5-xl.
 
     :param queries: The list of queries to use for reranking
@@ -25,69 +27,52 @@
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
     :param instruction: The instruction for reranking.
         Note: default instruction is "Find passage to answer given question"
             The default instruction from the TART paper is being used.
             If you want to use a different instruction, you can change the instruction through this parameter
+    :param batch: The number of queries to be processed in a batch
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
     model_name = "facebook/tart-full-flan-t5-xl"
     model = EncT5ForSequenceClassification.from_pretrained(model_name)
     tokenizer = EncT5Tokenizer.from_pretrained(model_name)
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    device = "cuda" if torch.cuda.is_available() else "cpu"
     model = model.to(device)
-    # Run async tart_rerank_pure function
-    tasks = [tart_pure(query, contents, scores, ids, top_k, model, tokenizer, instruction, device) \
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(asyncio.gather(*tasks))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+
+    nested_list = [[['{} [SEP] {}'.format(instruction, query)] for _ in contents] for query, contents in
+                   zip(queries, contents_list)]
+
+    rerank_scores = flatten_apply(tart_run_model, nested_list, model=model, batch_size=batch,
+                                  tokenizer=tokenizer, device=device, contents_list=contents_list)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     del tokenizer
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
-
-
-async def tart_pure(query: str, contents: List[str], scores: List[float],
-                    ids: List[str], top_k: int, model, tokenizer, instruction: str, device) \
-        -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using Tart.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param model: The Tart model to use for reranking
-    :param tokenizer: The tokenizer to use for the model
-    :param instruction: The instruction for reranking.
-    :param device: The device to run the model on (GPU if available, otherwise CPU)
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-
-    instruction_queries: List[str] = ['{0} [SEP] {1}'.format(instruction, query) for _ in range(len(contents))]
-    features = tokenizer(instruction_queries, contents, padding=True, truncation=True, return_tensors="pt")
-    features = features.to(device)
-
-    with torch.no_grad():
-        scores = model(**features).logits
-        normalized_scores = [float(score[1]) for score in F.softmax(scores, dim=1)]
-
-    contents_ids_scores = list(zip(contents, ids, normalized_scores))
-
-    sorted_contents_ids_scores = sorted(contents_ids_scores, key=lambda x: x[2], reverse=True)
-
-    # crop with top_k
-    if len(contents) < top_k:
-        top_k = len(contents)
-    sorted_contents_ids_scores = sorted_contents_ids_scores[:top_k]
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
-    content_result, id_result, score_result = zip(*sorted_contents_ids_scores)
 
-    return list(content_result), list(id_result), list(score_result)
+def tart_run_model(input_texts, contents_list, model, batch_size: int, tokenizer, device):
+    batch_input_texts = make_batch(input_texts, batch_size)
+    batch_contents_list = make_batch(contents_list, batch_size)
+    results = []
+    for batch_texts, batch_contents in zip(batch_input_texts, batch_contents_list):
+        flattened_batch_texts = list(chain.from_iterable(batch_texts))
+        flattened_batch_contents = list(chain.from_iterable(batch_contents))
+        feature = tokenizer(flattened_batch_texts, flattened_batch_contents, padding=True, truncation=True,
+                            return_tensors="pt").to(device)
+        with torch.no_grad():
+            pred_scores = model(**feature).logits
+            normalized_scores = [float(score[1]) for score in F.softmax(pred_scores, dim=1)]
+        results.extend(normalized_scores)
+    return results
```

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.4/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.4/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.4/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/promptmaker/base.py` & `autorag-0.1.4/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.4/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.4/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/promptmaker/run.py` & `autorag-0.1.4/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.4/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.4/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.4/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.4/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/base.py` & `autorag-0.1.4/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.4/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.4/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.4/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.4/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.4/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/run.py` & `autorag-0.1.4/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.4/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/schema/module.py` & `autorag-0.1.4/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/schema/node.py` & `autorag-0.1.4/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/strategy.py` & `autorag-0.1.4/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/support.py` & `autorag-0.1.4/autorag/support.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def dynamically_find_function(key: str, target_dict: Dict) -> Callable:
     if key in target_dict:
         module_path, func_name = target_dict[key]
         module = importlib.import_module(module_path)
         func = getattr(module, func_name)
         return func
     else:
-        raise KeyError(f"Key {key} is not supported.")
+        raise KeyError(f"Input module or node {key} is not supported.")
 
 
 def get_support_modules(module_name: str) -> Callable:
     support_modules = {
         # query_expansion
         'query_decompose': ('autorag.nodes.queryexpansion', 'query_decompose'),
         'hyde': ('autorag.nodes.queryexpansion', 'hyde'),
@@ -39,17 +39,19 @@
         'flag_embedding_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_reranker'),
         'flag_embedding_llm_reranker': ('autorag.nodes.passagereranker', 'flag_embedding_llm_reranker'),
         'time_reranker': ('autorag.nodes.passagereranker', 'time_reranker'),
         # passage_filter
         'pass_passage_filter': ('autorag.nodes.passagefilter', 'pass_passage_filter'),
         'similarity_threshold_cutoff': ('autorag.nodes.passagefilter', 'similarity_threshold_cutoff'),
         'similarity_percentile_cutoff': ('autorag.nodes.passagefilter', 'similarity_percentile_cutoff'),
+        'recency_filter': ('autorag.nodes.passagefilter', 'recency_filter'),
         # passage_compressor
         'tree_summarize': ('autorag.nodes.passagecompressor', 'tree_summarize'),
         'pass_compressor': ('autorag.nodes.passagecompressor', 'pass_compressor'),
+        'refine': ('autorag.nodes.passagecompressor', 'refine'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
         'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
         # generator
         'llama_index_llm': ('autorag.nodes.generator', 'llama_index_llm'),
         'vllm': ('autorag.nodes.generator', 'vllm'),
     }
```

### Comparing `autorag-0.1.3/autorag/utils/preprocess.py` & `autorag-0.1.4/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/autorag/utils/util.py` & `autorag-0.1.4/autorag/utils/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -237,14 +237,21 @@
         batch = tasks[i:i + batch_size]
         batch_results = await asyncio.gather(*batch)
         results.extend(batch_results)
 
     return results
 
 
+def make_batch(elems: List[Any], batch_size: int) -> List[List[Any]]:
+    """
+    Make a batch of elems with batch_size.
+    """
+    return [elems[i:i + batch_size] for i in range(0, len(elems), batch_size)]
+
+
 def save_parquet_safe(df: pd.DataFrame, filepath: str,
                       upsert: bool = False):
     output_file_dir = os.path.dirname(filepath)
     if not os.path.isdir(output_file_dir):
         raise NotADirectoryError(f"directory {output_file_dir} not found.")
     if not filepath.endswith("parquet"):
         raise NameError(f'file path: {filepath}  filename extension need to be ".parquet"')
@@ -272,7 +279,40 @@
 def reconstruct_list(flat_list: List[Any], lengths: List[int]) -> List[List[Any]]:
     result = []
     start = 0
     for length in lengths:
         result.append(flat_list[start:start + length])
         start += length
     return result
+
+
+def flatten_apply(func: Callable, nested_list: List[List[Any]], **kwargs) -> List[List[Any]]:
+    """
+    This function flattens the input list and applies the function to the elements.
+    After that, it reconstructs the list to the original shape.
+    Its speciality is that the first dimension length of the list can be different from each other.
+
+    :param func: The function that applies to the flattened list.
+    :param nested_list: The nested list to be flattened.
+    :return: The list that is reconstructed after applying the function.
+    """
+    df = pd.DataFrame({'col1': nested_list})
+    df = df.explode('col1')
+    df['result'] = func(df['col1'].tolist(), **kwargs)
+    return df.groupby(level=0, sort=False)['result'].apply(list).tolist()
+
+
+def sort_by_scores(row, reverse=True):
+    """
+    Sorts each row by 'scores' column.
+    The input column names must be 'contents', 'ids', and 'scores'.
+    And its elements must be list type.
+    """
+    results = sorted(zip(row['contents'], row['ids'], row['scores']), key=lambda x: x[2], reverse=reverse)
+    reranked_contents, reranked_ids, reranked_scores = zip(*results)
+    return list(reranked_contents), list(reranked_ids), list(reranked_scores)
+
+
+def select_top_k(df, column_names: List[str], top_k: int):
+    for column_name in column_names:
+        df[column_name] = df[column_name].apply(lambda x: x[:top_k])
+    return df
```

### Comparing `autorag-0.1.3/autorag/web.py` & `autorag-0.1.4/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/Makefile` & `autorag-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/make.bat` & `autorag-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/data_creation.png` & `autorag-0.1.4/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/data_folder.png` & `autorag-0.1.4/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/node_folder.png` & `autorag-0.1.4/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/node_line_folder.png` & `autorag-0.1.4/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/node_line_summary.png` & `autorag-0.1.4/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/node_lines.png` & `autorag-0.1.4/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/node_summary.png` & `autorag-0.1.4/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/project_folder_example.png` & `autorag-0.1.4/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/project_folders.png` & `autorag-0.1.4/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/resources_folder.png` & `autorag-0.1.4/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.4/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.4/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.4/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/merger.png` & `autorag-0.1.4/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.4/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/roadmap/policy.png` & `autorag-0.1.4/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.4/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/trial_folder.png` & `autorag-0.1.4/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/trial_json.png` & `autorag-0.1.4/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/trial_summary.png` & `autorag-0.1.4/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/_static/web_interface.png` & `autorag-0.1.4/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 -------------------------------------------------------
 
 .. automodule:: autorag.nodes.passagecompressor.pass_compressor
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagecompressor.refine module
+---------------------------------------------
+
+.. automodule:: autorag.nodes.passagecompressor.refine
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagecompressor.run module
 ------------------------------------------
 
 .. automodule:: autorag.nodes.passagecompressor.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,37 @@
-autorag.nodes.passagefilter package
-===================================
+autorag.nodes.passagereranker.tart package
+==========================================
 
 Submodules
 ----------
 
-autorag.nodes.passagefilter.base module
----------------------------------------
+autorag.nodes.passagereranker.tart.modeling\_enc\_t5 module
+-----------------------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.base
+.. automodule:: autorag.nodes.passagereranker.tart.modeling_enc_t5
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.pass\_passage\_filter module
---------------------------------------------------------
+autorag.nodes.passagereranker.tart.tart module
+----------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.pass_passage_filter
+.. automodule:: autorag.nodes.passagereranker.tart.tart
    :members:
    :undoc-members:
    :show-inheritance:
 
-autorag.nodes.passagefilter.percentile\_cutoff module
------------------------------------------------------
+autorag.nodes.passagereranker.tart.tokenization\_enc\_t5 module
+---------------------------------------------------------------
 
-.. automodule:: autorag.nodes.passagefilter.percentile_cutoff
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-autorag.nodes.passagefilter.run module
---------------------------------------
-
-.. automodule:: autorag.nodes.passagefilter.run
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-autorag.nodes.passagefilter.threshold\_cutoff module
-----------------------------------------------------
-
-.. automodule:: autorag.nodes.passagefilter.threshold_cutoff
+.. automodule:: autorag.nodes.passagereranker.tart.tokenization_enc_t5
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: autorag.nodes.passagefilter
+.. automodule:: autorag.nodes.passagereranker.tart
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/api_spec/autorag.rst` & `autorag-0.1.4/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/conf.py` & `autorag-0.1.4/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "myst_parser",
     "sphinx_copybutton",
     "sphinx_design",
     "sphinx_inline_tabs",
     "sphinxcontrib.googleanalytics",
+    "sphinx_sitemap",
 ]
 source_suffix = {
     '.rst': 'restructuredtext',
     '.md': 'markdown',
 }
 
 templates_path = ['_templates']
@@ -40,7 +41,8 @@
 googleanalytics_id = 'G-T8ZKQM6RT9'
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'furo'
 html_static_path = ['_static']
+html_baseurl = 'https://marker-inc-korea.github.io/AutoRAG/'
```

### Comparing `autorag-0.1.3/docs/source/data_creation/data_format.md` & `autorag-0.1.4/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/data_creation/ragas.md` & `autorag-0.1.4/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/data_creation/tutorial.md` & `autorag-0.1.4/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/deploy/api_endpoint.md` & `autorag-0.1.4/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/deploy/web.md` & `autorag-0.1.4/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/index.rst` & `autorag-0.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/install.md` & `autorag-0.1.4/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/local_model.md` & `autorag-0.1.4/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/generator/generator.md` & `autorag-0.1.4/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.4/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/generator/vllm.md` & `autorag-0.1.4/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.4/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,9 @@
 #### Supported Modules
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 tree_summarize.md
+refine.md
 ```
```

### Comparing `autorag-0.1.3/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.4/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.4/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files 3% similar despite different names*

```diff
@@ -47,8 +47,9 @@
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 similarity_threshold_cutoff.md
 similarity_percentile_cutoff.md
+recency_filter.md
 ```
```

### Comparing `autorag-0.1.3/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.4/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.4/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 koreranker.md
 cohere.md
 rankgpt.md
 jina_reranker.md
 colbert.md
 sentence_transformer_reranker.md
 flag_embedding_reranker.md
-time_reranker.md
 flag_embedding_llm_reranker.md
+time_reranker.md
 ```
```

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.4/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.4/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.4/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.4/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.4/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.4/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.4/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.4/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.4/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.4/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.4/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/optimization/custom_config.md` & `autorag-0.1.4/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/optimization/folder_structure.md` & `autorag-0.1.4/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/optimization/optimization.md` & `autorag-0.1.4/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.4/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/roadmap/modular_rag.md` & `autorag-0.1.4/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/structure.md` & `autorag-0.1.4/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/troubleshooting.md` & `autorag-0.1.4/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/docs/source/tutorial.md` & `autorag-0.1.4/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/pyproject.toml` & `autorag-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/requirements.txt` & `autorag-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/compact_local.yaml` & `autorag-0.1.4/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/compact_openai.yaml` & `autorag-0.1.4/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/config_korean.yaml` & `autorag-0.1.4/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/extracted_sample.yaml` & `autorag-0.1.4/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/full.yaml` & `autorag-0.1.4/sample_config/full.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -72,23 +72,28 @@
       strategy:
         metrics: [ retrieval_f1, retrieval_recall, retrieval_precision ]
         speed_threshold: 5
       modules:
         - module_type: pass_passage_filter
         - module_type: similarity_threshold_cutoff
           threshold: 0.85
+        - module_type: recency_filter
+          threshold: 2015-01-01
     - node_type: passage_compressor
       strategy:
         metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
         speed_threshold: 10
       modules:
         - module_type: pass_compressor
         - module_type: tree_summarize
           llm: openai
           model: gpt-3.5-turbo-16k
+        - module_type: refine
+          llm: openai
+          model: gpt-3.5-turbo-16k
 - node_line_name: post_retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: prompt_maker
       strategy:
         metrics:
           - metric_name: bleu
           - metric_name: meteor
```

### Comparing `autorag-0.1.3/sample_config/simple_local.yaml` & `autorag-0.1.4/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_config/simple_openai.yaml` & `autorag-0.1.4/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_dataset/README.md` & `autorag-0.1.4/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.4/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.4/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.4/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.4/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.4/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.4/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.4/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import asyncio
 import os
 import pathlib
+import re
+from unittest.mock import patch
 
 import pandas as pd
 import pytest
-from llama_index.llms.openai import OpenAI
+from llama_index.core.base.llms.types import CompletionResponse
+from llama_index.core.llms import MockLLM
 
 from autorag.data.qacreation.llama_index import async_qa_gen_llama_index, generate_qa_llama_index_by_ratio, \
     generate_qa_llama_index
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 resource_dir = os.path.join(root_dir, "resources")
 
@@ -24,39 +26,49 @@
 
 @pytest.fixture
 def contents():
     df = pd.read_csv(os.path.join(resource_dir, "sample_contents_nqa.csv"))
     yield df['passage'].tolist()[:6]
 
 
-def test_async_qa_gen_llama_index():
-    result = asyncio.run(async_qa_gen_llama_index(content, llm=OpenAI(model="gpt-3.5-turbo",
-                                                                      temperature=1.0),
-                                                  prompt=sample_prompt, question_num=3))
+async def acomplete_qa_creation(self, messages, **kwargs):
+    pattern = r'Number of questions to generate: (\d+)'
+    matches = re.findall(pattern, messages)
+    num_questions = int(matches[-1])
+    return CompletionResponse(text=
+                              "[Q]: Is this the test question?\n[A]: Yes, this is the test answer." * num_questions)
+
+
+@patch.object(MockLLM, "acomplete", acomplete_qa_creation)
+@pytest.mark.asyncio()
+async def test_async_qa_gen_llama_index():
+    result = await async_qa_gen_llama_index(content, llm=MockLLM(), prompt=sample_prompt, question_num=3)
     assert len(result) == 3
     for res in result:
         assert "query" in res
         assert "generation_gt" in res
         assert bool(res['query'])
         assert bool(res['generation_gt'])
 
 
+@patch.object(MockLLM, "acomplete", acomplete_qa_creation)
 def test_qa_gen_llama_index(contents):
-    llm = OpenAI(model='gpt-3.5-turbo', temperature=1.0)
+    llm = MockLLM()
     result = generate_qa_llama_index(llm, contents, sample_prompt)
     check_multi_qa_gen(result)
 
 
+@patch.object(MockLLM, "acomplete", acomplete_qa_creation)
 def test_qa_gen_llama_index_by_ratio(contents):
     ratio_dict = {
         str(os.path.join(prompt_dir, "prompt1.txt")): 1,
         str(os.path.join(prompt_dir, "prompt2.txt")): 2,
         str(os.path.join(prompt_dir, "prompt3.txt")): 3,
     }
-    llm = OpenAI(model='gpt-3.5-turbo', temperature=1.0)
+    llm = MockLLM()
     result = generate_qa_llama_index_by_ratio(llm, contents, ratio_dict, batch=8)
     check_multi_qa_gen(result)
 
 
 def check_multi_qa_gen(result):
     assert len(result) == 6
     for res in result:
```

### Comparing `autorag-0.1.3/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.4/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.4/tests/autorag/data/qacreation/test_simple.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from guidance import models
 from llama_index.core import SimpleDirectoryReader
 
 from autorag.data.corpus.llama_index import llama_documents_to_parquet
 from autorag.data.qacreation.simple import generate_simple_qa_dataset, generate_qa_row
 from autorag.data.utils.util import get_file_metadata
 from autorag.utils.preprocess import validate_qa_dataset, validate_corpus_dataset
+from tests.delete_tests import is_github_action
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 
 raw_dir = os.path.join(root_dir, "resources", "data_creation", "raw_dir")
 
 load_file_name = "test_corpus.parquet"
 
@@ -27,14 +28,15 @@
 
 @pytest.fixture
 def output_filedir():
     with tempfile.TemporaryDirectory() as temp_dir:
         yield temp_dir
 
 
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions because it will be deprecated.")
 def test_generate_simple_qa_dataset(load_dir, output_filedir):
     loader = SimpleDirectoryReader(
         file_metadata=get_file_metadata,
         input_dir=raw_dir
     )
 
     documents = loader.load_data(
```

### Comparing `autorag-0.1.3/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.4/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.1.4/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.4/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.4/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.4/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.4/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.4/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.4/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.4/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.4/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,15 @@
-from typing import List
-
 import pandas as pd
 
 from autorag import generator_models
 from autorag.nodes.passagecompressor import tree_summarize
+from tests.autorag.nodes.passagecompressor.test_base_passage_compressor import (queries, retrieved_contents, df,
+                                                                                check_result)
 from tests.mock import MockLLM
 
-queries = [
-    "What is the capital of France?",
-    "What is the meaning of life?",
-]
-retrieved_contents = [
-    ["Paris is the capital of France.", "France is a country in Europe.", "France is a member of the EU."],
-    ["The meaning of life is 42.", "The meaning of life is to be happy.", "The meaning of life is to be kind."],
-]
-
-
-def check_result(result: List[str]):
-    assert len(result) == len(queries)
-    for r in result:
-        assert isinstance(r, str)
-        assert len(r) > 0
-        assert bool(r) is True
-
 
 def test_tree_summarize_default():
     llm = MockLLM()
     result = tree_summarize.__wrapped__(queries, retrieved_contents, [], [], llm)
     check_result(result)
 
 
@@ -50,20 +33,14 @@
     result = tree_summarize.__wrapped__(queries, retrieved_contents, [], [], gpt_3, chat_prompt=prompt)
     check_result(result)
     assert 'What is the capital of France?' in result[0]
 
 
 def test_tree_summarize_node():
     generator_models['mock'] = MockLLM
-    df = pd.DataFrame({
-        'query': queries,
-        'retrieved_contents': retrieved_contents,
-        'retrieved_ids': [['id-1', 'id-2', 'id-3'], ['id-4', 'id-5', 'id-6']],
-        'retrieve_scores': [[0.1, 0.2, 0.3], [0.4, 0.5, 0.6]],
-    })
     result = tree_summarize(
         "project_dir",
         df,
         llm='mock',
         prompt="This is a custom prompt. {context_str} {query_str}",
         max_tokens=64,
     )
```

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 import os
 import pathlib
+import tempfile
+from datetime import datetime
 from uuid import uuid4
 
 import pandas as pd
+import pytest
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 project_dir = os.path.join(root_dir, "resources", "sample_project")
 qa_data = pd.read_parquet(os.path.join(project_dir, "data", "qa.parquet"))
 corpus_data = pd.read_parquet(os.path.join(project_dir, "data", "corpus.parquet"))
 previous_result = qa_data.sample(2)
 
 queries_example = ["What is the capital of France?",
                    "How many members are in Newjeans?"]
 contents_example = [["NomaDamas is Great Team", "Paris is the capital of France.", "havertz is suck at soccer",
                      "Paris is one of the capital from France. Isn't it?"],
                     ["i am hungry", "LA is a country in the United States.", "Newjeans has 5 members.",
                      "Danielle is one of the members of Newjeans."]]
+time_list = [[datetime(2015, 1, 1), datetime(2021, 9, 3),
+              datetime(2022, 3, 5, 12, 30), datetime(2022, 3, 5, 12, 45, 00)],
+             [datetime(2015, 1, 1), datetime(2021, 1, 1),
+              datetime(2022, 3, 5, 12, 40), datetime(2022, 3, 5, 12, 45, 00)]]
 ids_example = [[str(uuid4()) for _ in range(len(contents_example[0]))],
                [str(uuid4()) for _ in range(len(contents_example[1]))]]
 scores_example = [[0.1, 0.8, 0.1, 0.5], [0.1, 0.2, 0.7, 0.3]]
 f1_example = [0.4, 1.0]
 recall_example = [1.0, 0.3]
 
 previous_result['query'] = queries_example
 previous_result['retrieved_contents'] = contents_example
 previous_result['retrieved_ids'] = ids_example
 previous_result['retrieve_scores'] = scores_example
 previous_result['retrieval_f1'] = f1_example
 previous_result['retrieval_recall'] = recall_example
 
 
+@pytest.fixture
+def project_dir_with_corpus():
+    with tempfile.TemporaryDirectory() as temp_dir:
+        data_dir = os.path.join(temp_dir, "data")
+        os.makedirs(data_dir, exist_ok=True)
+        qa_data.to_parquet(os.path.join(data_dir, "qa.parquet"), index=False)
+        new_rows = pd.DataFrame({
+            'doc_id': ids_example[0] + ids_example[1],
+            'contents': contents_example[0] + contents_example[1],
+            'metadata': list(map(lambda x: {'last_modified_datetime': x}, time_list[0])) + list(
+                map(lambda x: {'last_modified_datetime': x}, time_list[1]))
+        })
+        new_corpus = pd.concat([corpus_data, new_rows], ignore_index=True, axis=0)
+        new_corpus.to_parquet(os.path.join(data_dir, "corpus.parquet"), index=False)
+        yield temp_dir
+
+
 def base_passage_filter_test(contents, ids, scores):
     assert len(contents) == len(ids) == len(scores) == 2
     for content_list, id_list, score_list in zip(contents, ids, scores):
         assert isinstance(content_list, list)
         assert isinstance(id_list, list)
         assert isinstance(score_list, list)
         for content, _id, score in zip(content_list, id_list, score_list):
```

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.4/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.4/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.4/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
 import tempfile
+from unittest.mock import patch
 
 import numpy as np
 import pandas as pd
 import pytest
+from llama_index.core.base.llms.types import CompletionResponse
+from llama_index.llms.openai import OpenAI
 
 from autorag import generator_models
 from autorag.evaluate.util import cast_metrics
 from autorag.nodes.generator import llama_index_llm
 from autorag.nodes.promptmaker import fstring
 from autorag.nodes.promptmaker.run import evaluate_generator_result, evaluate_one_prompt_maker_node, \
     run_prompt_maker_node
@@ -115,14 +118,19 @@
     best_result_path = os.path.join(node_line_dir, "prompt_maker", f"best_{best_filename}")
     assert os.path.exists(best_result_path)
 
     assert os.path.exists(os.path.join(node_line_dir, "prompt_maker", "0.parquet"))
     assert os.path.exists(os.path.join(node_line_dir, "prompt_maker", "1.parquet"))
 
 
+async def acomplete_qa_creation(*args, **kwargs):
+    return CompletionResponse(text="This is the test answer.")
+
+
+@patch.object(OpenAI, "acomplete", acomplete_qa_creation)
 def test_run_prompt_maker_node_default(node_line_dir):
     modules = [fstring, fstring]
     params = [{'prompt': 'Tell me something about the question: {query} \n\n {retrieved_contents}'},
               {'prompt': 'Question: {query} \n Something to read: {retrieved_contents} \n What\'s your answer?'}]
     strategies = {
         'metrics': metrics
     }
```

### Comparing `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.4/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.4/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.4/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.4/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/test_cli.py` & `autorag-0.1.4/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/test_deploy.py` & `autorag-0.1.4/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/test_evaluator.py` & `autorag-0.1.4/tests/autorag/test_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os.path
 import pathlib
 import tempfile
 from distutils.dir_util import copy_tree
+from unittest.mock import patch
 
 import pandas as pd
 import pytest
+from llama_index.core.base.llms.types import CompletionResponse
+from llama_index.llms.openai import OpenAI
 
 from autorag.deploy import extract_best_config
 from autorag.evaluator import Evaluator
 from autorag.nodes.retrieval import bm25, vectordb, hybrid_rrf
 from autorag.nodes.retrieval.run import run_retrieval_node
 from autorag.schema import Node
 from autorag.utils import validate_qa_dataset, validate_corpus_dataset
@@ -213,19 +216,30 @@
     assert os.path.exists(os.path.join(error_path, 'pre_retrieve_node_line', 'summary.csv'))
     assert os.path.exists(os.path.join(error_path, 'retrieve_node_line'))
     assert os.path.exists(os.path.join(error_path, 'retrieve_node_line', 'summary.csv'))
     assert os.path.exists(os.path.join(error_path, 'post_retrieve_node_line'))
     assert os.path.exists(os.path.join(error_path, 'post_retrieve_node_line', 'summary.csv'))
 
 
+async def mock_acomplete(self, messages, **kwargs):
+    return CompletionResponse(text=messages)
+
+
+async def mock_apredict(self, prompt, **kwargs):
+    return prompt.format(**kwargs)
+
+
+@patch.object(OpenAI, "acomplete", mock_acomplete)
+@patch.object(OpenAI, "apredict", mock_apredict)
 def test_restart_last_node(evaluator):
     compressor_error_folder_path = os.path.join(resource_dir, 'result_project', '1')
     base_restart_trial(evaluator, compressor_error_folder_path)
 
 
+@patch.object(OpenAI, "acomplete", mock_acomplete)
 def test_restart_first_node(evaluator):
     prompt_error_folder_path = os.path.join(resource_dir, 'result_project', '2')
     base_restart_trial(evaluator, prompt_error_folder_path)
 
 
 def test_restart_leads_start_trial(evaluator):
     start_error_folder_path = os.path.join(resource_dir, 'result_project')
```

### Comparing `autorag-0.1.3/tests/autorag/test_strategy.py` & `autorag-0.1.4/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/test_web.py` & `autorag-0.1.4/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.4/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/autorag/utils/test_util.py` & `autorag-0.1.4/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/delete_tests.py` & `autorag-0.1.4/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/mock.py` & `autorag-0.1.4/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/README.md` & `autorag-0.1.4/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.4/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.4/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/full.yaml` & `autorag-0.1.4/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/qa_data_sample.parquet` & `autorag-0.1.4/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.4/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/config.yaml` & `autorag-0.1.4/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.4/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/0/summary.csv` & `autorag-0.1.4/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/config.yaml` & `autorag-0.1.4/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/config.yaml` & `autorag-0.1.4/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.4/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/3/config.yaml` & `autorag-0.1.4/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/best.yaml` & `autorag-0.1.4/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.4/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.4/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.4/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.4/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.4/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.4/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.4/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.4/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.4/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/simple.yaml` & `autorag-0.1.4/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.3/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.4/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

