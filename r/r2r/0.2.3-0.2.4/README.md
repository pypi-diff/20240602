# Comparing `tmp/r2r-0.2.3.tar.gz` & `tmp/r2r-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.2.3.tar", max compression
+gzip compressed data, was "r2r-0.2.4.tar", max compression
```

## Comparing `r2r-0.2.3.tar` & `r2r-0.2.4.tar`

### file list

```diff
@@ -1,97 +1,107 @@
--rw-r--r--   0        0        0     1082 2024-05-30 01:12:00.176957 r2r-0.2.3/LICENSE.md
--rw-r--r--   0        0        0    12944 2024-05-30 01:12:00.176957 r2r-0.2.3/README.md
--rw-r--r--   0        0        0     1151 2024-05-30 01:12:00.176957 r2r-0.2.3/config.json
--rw-r--r--   0        0        0     1980 2024-05-30 01:12:00.192957 r2r-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2047 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/__init__.py
--rw-r--r--   0        0        0     3083 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      186 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/abstractions/llm.py
--rw-r--r--   0        0        0     1083 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/abstractions/prompt.py
--rw-r--r--   0        0        0      813 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/abstractions/search.py
--rw-r--r--   0        0        0     1934 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/abstractions/vector.py
--rw-r--r--   0        0        0      538 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/parsers/__init__.py
--rw-r--r--   0        0        0      334 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/parsers/base_parser.py
--rw-r--r--   0        0        0    14096 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/parsers/parser_impls.py
--rw-r--r--   0        0        0     9358 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/pipeline/base_pipeline.py
--rw-r--r--   0        0        0     3949 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/pipes/base_pipe.py
--rw-r--r--   0        0        0     2409 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/pipes/loggable_pipe.py
--rw-r--r--   0        0        0    16417 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/pipes/pipe_logging.py
--rw-r--r--   0        0        0     1306 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/base_provider.py
--rw-r--r--   0        0        0     2267 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/embedding_provider.py
--rw-r--r--   0        0        0     1029 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/eval_provider.py
--rw-r--r--   0        0        0     2328 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/llm_provider.py
--rw-r--r--   0        0        0     1456 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/prompt_provider.py
--rw-r--r--   0        0        0     2550 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/providers/vector_db_provider.py
--rw-r--r--   0        0        0      363 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/utils/base_utils.py
--rw-r--r--   0        0        0       95 2024-05-30 01:12:00.192957 r2r-0.2.3/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66643 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      332 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     2363 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/embeddings/dummy/provider.py
--rw-r--r--   0        0        0     6309 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/embeddings/openai/openai_base.py
--rw-r--r--   0        0        0     6238 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/embeddings/setence_transformer/sentence_transformer_base.py
--rw-r--r--   0        0        0       78 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/eval/llm/base_llm_eval.py
--rw-r--r--   0        0        0        0 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/__init__.py
--rw-r--r--   0        0        0      385 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/base_app.py
--rw-r--r--   0        0        0     3091 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/custom_rag.py
--rw-r--r--   0        0        0    73353 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/data/aristotle.txt
--rw-r--r--   0        0        0       49 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/data/example_postgres_logger_config.json
--rw-r--r--   0        0        0       91 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/data/example_qdrant_config.json
--rw-r--r--   0        0        0      455 2024-05-30 01:12:00.196957 r2r-0.2.3/r2r/examples/data/example_rerank_config.json
--rw-r--r--   0        0        0  1440303 2024-05-30 01:12:00.200958 r2r-0.2.3/r2r/examples/data/lyft_2021.pdf
--rw-r--r--   0        0        0   131542 2024-05-30 01:12:00.200958 r2r-0.2.3/r2r/examples/data/pg_essay_1.html
--rw-r--r--   0        0        0   125150 2024-05-30 01:12:00.204958 r2r-0.2.3/r2r/examples/data/pg_essay_2.html
--rw-r--r--   0        0        0   124948 2024-05-30 01:12:00.204958 r2r-0.2.3/r2r/examples/data/pg_essay_3.html
--rw-r--r--   0        0        0   118147 2024-05-30 01:12:00.204958 r2r-0.2.3/r2r/examples/data/pg_essay_4.html
--rw-r--r--   0        0        0   123820 2024-05-30 01:12:00.204958 r2r-0.2.3/r2r/examples/data/pg_essay_5.html
--rw-r--r--   0        0        0   791764 2024-05-30 01:12:00.208958 r2r-0.2.3/r2r/examples/data/screen_shot.png
--rw-r--r--   0        0        0       19 2024-05-30 01:12:00.208958 r2r-0.2.3/r2r/examples/data/test.txt
--rw-r--r--   0        0        0  1880483 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/examples/data/uber_2021.pdf
--rw-r--r--   0        0        0    11992 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/examples/demo.py
--rw-r--r--   0        0        0        0 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0     1569 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/examples/servers/configurable_pipeline.py
--rw-r--r--   0        0        0      147 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1535 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3940 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/integrations/serper.py
--rw-r--r--   0        0        0      232 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3315 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/llms/litellm/base_litellm.py
--rw-r--r--   0        0        0     3919 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/llms/llama_cpp/base_llama_cpp.py
--rw-r--r--   0        0        0        0 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3462 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/llms/openai/base_openai.py
--rw-r--r--   0        0        0      410 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/__init__.py
--rw-r--r--   0        0        0     1102 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/r2r_abstractions.py
--rw-r--r--   0        0        0    24571 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/r2r_app.py
--rw-r--r--   0        0        0     5529 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/r2r_client.py
--rw-r--r--   0        0        0     4599 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/r2r_config.py
--rw-r--r--   0        0        0    11331 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/main/r2r_factory.py
--rw-r--r--   0        0        0      593 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/__init__.py
--rw-r--r--   0        0        0     1266 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/abstractions/generator_pipe.py
--rw-r--r--   0        0        0     1552 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/abstractions/search_pipe.py
--rw-r--r--   0        0        0     7244 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/embedding_pipe.py
--rw-r--r--   0        0        0     1272 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/eval_pipe.py
--rw-r--r--   0        0        0     7590 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/parsing_pipe.py
--rw-r--r--   0        0        0     3050 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/query_transform_pipe.py
--rw-r--r--   0        0        0     2738 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/rag_pipe.py
--rw-r--r--   0        0        0     3307 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/streaming_rag_pipe.py
--rw-r--r--   0        0        0     2808 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/vector_search_pipe.py
--rw-r--r--   0        0        0     3166 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/pipes/vector_storage_pipe.py
--rw-r--r--   0        0        0       90 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/prompts/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/prompts/local/__init__.py
--rw-r--r--   0        0        0     4390 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/prompts/local/defaults.jsonl
--rw-r--r--   0        0        0     1900 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/prompts/local/r2r_prompt_provider.py
--rw-r--r--   0        0        0      539 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3263 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5317 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9350 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/client.py
--rw-r--r--   0        0        0    36863 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vecs/exc.py
--rw-r--r--   0        0        0      213 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     6379 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vector_dbs/local/r2r_local_vector_db.py
--rw-r--r--   0        0        0     6268 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vector_dbs/pgvector/pgvector_db.py
--rw-r--r--   0        0        0     7412 2024-05-30 01:12:00.216958 r2r-0.2.3/r2r/vector_dbs/qdrant/qdrant_db.py
--rw-r--r--   0        0        0    14924 1970-01-01 00:00:00.000000 r2r-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-06-02 17:53:07.328614 r2r-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0    13278 2024-06-02 17:53:07.328614 r2r-0.2.4/README.md
+-rw-r--r--   0        0        0     1151 2024-06-02 17:53:07.328614 r2r-0.2.4/config.json
+-rw-r--r--   0        0        0     1944 2024-06-02 17:53:07.348615 r2r-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2241 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/__init__.py
+-rw-r--r--   0        0        0     3154 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/__init__.py
+-rw-r--r--   0        0        0     1371 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      186 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/abstractions/llm.py
+-rw-r--r--   0        0        0     1083 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/abstractions/prompt.py
+-rw-r--r--   0        0        0      813 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/abstractions/search.py
+-rw-r--r--   0        0        0     1934 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/abstractions/vector.py
+-rw-r--r--   0        0        0    16040 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/logging/kv_logger.py
+-rw-r--r--   0        0        0     1678 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/logging/run_manager.py
+-rw-r--r--   0        0        0      538 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/parsers/__init__.py
+-rw-r--r--   0        0        0      334 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/parsers/base_parser.py
+-rw-r--r--   0        0        0    14096 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/parsers/parser_impls.py
+-rw-r--r--   0        0        0     9552 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0     1364 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/pipeline/pipeline_router.py
+-rw-r--r--   0        0        0     3317 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/pipes/base_pipe.py
+-rw-r--r--   0        0        0     2895 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/pipes/loggable_pipe.py
+-rw-r--r--   0        0        0     1306 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/base_provider.py
+-rw-r--r--   0        0        0     2267 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/embedding_provider.py
+-rw-r--r--   0        0        0      998 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/eval_provider.py
+-rw-r--r--   0        0        0     2328 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/llm_provider.py
+-rw-r--r--   0        0        0     1494 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/prompt_provider.py
+-rw-r--r--   0        0        0     2756 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/providers/vector_db_provider.py
+-rw-r--r--   0        0        0      411 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0     1059 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/utils/base_utils.py
+-rw-r--r--   0        0        0       95 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66643 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      332 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     2363 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/embeddings/dummy/provider.py
+-rw-r--r--   0        0        0     7679 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/embeddings/openai/openai_base.py
+-rw-r--r--   0        0        0     6238 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/embeddings/setence_transformer/sentence_transformer_base.py
+-rw-r--r--   0        0        0       78 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2857 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/eval/llm/base_llm_eval.py
+-rw-r--r--   0        0        0        0 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/examples/__init__.py
+-rw-r--r--   0        0        0      397 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/examples/base_app.py
+-rw-r--r--   0        0        0     3067 2024-06-02 17:53:07.348615 r2r-0.2.4/r2r/examples/custom_rag.py
+-rw-r--r--   0        0        0    73353 2024-06-02 17:53:07.352615 r2r-0.2.4/r2r/examples/data/aristotle.txt
+-rw-r--r--   0        0        0     7442 2024-06-02 17:53:07.352615 r2r-0.2.4/r2r/examples/data/aristotle_v2.txt
+-rw-r--r--   0        0        0       49 2024-06-02 17:53:07.352615 r2r-0.2.4/r2r/examples/data/example_postgres_logger_config.json
+-rw-r--r--   0        0        0       91 2024-06-02 17:53:07.352615 r2r-0.2.4/r2r/examples/data/example_qdrant_config.json
+-rw-r--r--   0        0        0      455 2024-06-02 17:53:07.352615 r2r-0.2.4/r2r/examples/data/example_rerank_config.json
+-rw-r--r--   0        0        0  1440303 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/lyft_2021.pdf
+-rw-r--r--   0        0        0   131542 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/pg_essay_1.html
+-rw-r--r--   0        0        0   125150 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/pg_essay_2.html
+-rw-r--r--   0        0        0   124948 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/pg_essay_3.html
+-rw-r--r--   0        0        0   118147 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/pg_essay_4.html
+-rw-r--r--   0        0        0   123820 2024-06-02 17:53:07.356615 r2r-0.2.4/r2r/examples/data/pg_essay_5.html
+-rw-r--r--   0        0        0   791764 2024-06-02 17:53:07.360615 r2r-0.2.4/r2r/examples/data/screen_shot.png
+-rw-r--r--   0        0        0       19 2024-06-02 17:53:07.360615 r2r-0.2.4/r2r/examples/data/test.txt
+-rw-r--r--   0        0        0  1880483 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/data/uber_2021.pdf
+-rw-r--r--   0        0        0    16168 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/demo.py
+-rw-r--r--   0        0        0      831 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/scripts/run_hyde.py
+-rw-r--r--   0        0        0     1972 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/scripts/run_web_multi_search.py
+-rw-r--r--   0        0        0      613 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/scripts/run_web_search.py
+-rw-r--r--   0        0        0        0 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1569 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/examples/servers/configurable_pipeline.py
+-rw-r--r--   0        0        0      147 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1535 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3940 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      232 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3315 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/llms/litellm/base_litellm.py
+-rw-r--r--   0        0        0     3919 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/llms/llama_cpp/base_llama_cpp.py
+-rw-r--r--   0        0        0        0 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3462 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/llms/openai/base_openai.py
+-rw-r--r--   0        0        0      470 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/__init__.py
+-rw-r--r--   0        0        0     1102 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_abstractions.py
+-rw-r--r--   0        0        0    33777 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_app.py
+-rw-r--r--   0        0        0     6470 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_builder.py
+-rw-r--r--   0        0        0     7754 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_client.py
+-rw-r--r--   0        0        0     5434 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_config.py
+-rw-r--r--   0        0        0    13428 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/main/r2r_factory.py
+-rw-r--r--   0        0        0      730 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/__init__.py
+-rw-r--r--   0        0        0     1305 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/abstractions/generator_pipe.py
+-rw-r--r--   0        0        0     1468 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/abstractions/search_pipe.py
+-rw-r--r--   0        0        0     7282 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/embedding_pipe.py
+-rw-r--r--   0        0        0     1344 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/eval_pipe.py
+-rw-r--r--   0        0        0     7934 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/parsing_pipe.py
+-rw-r--r--   0        0        0     3111 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/query_transform_pipe.py
+-rw-r--r--   0        0        0     2758 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/rag_pipe.py
+-rw-r--r--   0        0        0     3327 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/streaming_rag_pipe.py
+-rw-r--r--   0        0        0     2852 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/vector_search_pipe.py
+-rw-r--r--   0        0        0     3181 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/vector_storage_pipe.py
+-rw-r--r--   0        0        0     3108 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/pipes/web_search_pipe.py
+-rw-r--r--   0        0        0      137 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prebuilts/__init__.py
+-rw-r--r--   0        0        0     5141 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prebuilts/multi_search.py
+-rw-r--r--   0        0        0       90 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prompts/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prompts/local/__init__.py
+-rw-r--r--   0        0        0     4399 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prompts/local/defaults.jsonl
+-rw-r--r--   0        0        0     1900 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/prompts/local/r2r_prompt_provider.py
+-rw-r--r--   0        0        0      539 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3263 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5317 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9350 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/client.py
+-rw-r--r--   0        0        0    36564 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      213 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     6713 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vector_dbs/local/r2r_local_vector_db.py
+-rw-r--r--   0        0        0     6393 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vector_dbs/pgvector/pgvector_db.py
+-rw-r--r--   0        0        0     7629 2024-06-02 17:53:07.372615 r2r-0.2.4/r2r/vector_dbs/qdrant/qdrant_db.py
+-rw-r--r--   0        0        0    15212 1970-01-01 00:00:00.000000 r2r-0.2.4/PKG-INFO
```

### Comparing `r2r-0.2.3/LICENSE.md` & `r2r-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/README.md` & `r2r-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
 <h3 align="center">
 Build, deploy, observe, and optimize your RAG system.
 </h3>
 
 # About
 
-R2R, short for RAG to Riches, provides the fastest and most efficient way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+R2R, short for RAG to Riches, provides the fastest and most efficient way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is built around customizable pipelines and ships with a feature-rich REST API.
 
 ## Why?
 
 R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. It is built with observability and customization in mind, ensuring that users can seamlessly transition from development to deployment.
 
 ## Key Features
 - **🔧 Build**: Use the framework to build arbitrary asynchronous pipelines.
@@ -49,16 +49,14 @@
 
 [Join the Discord server](https://discord.gg/p6KqD2kjtB)
 
 [R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
 
 [SciPhi Cloud Docs](https://docs.sciphi.ai/)
 
-[Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/local_rag)
-
 # R2R Demo
 
 The R2R demo offers a step-by-step guide on running the default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests a list of provided provided documents and demonstrates search, RAG, and advanced functionality. The script at `r2r/examples/demo.py`, which powers the demo, can be configured and extended with sufficient developer familiarity.
 
 ## Ingest Demo Files
 
 To comprehensively demonstrate the RAG functionalities of the R2R framework, we must start by ingesting a realistic set of documents. Running the command below will parse, chunk, embed, and store a preset list of files. The included file types cover HTML, PDF, PNG, and TXT examples:
@@ -79,15 +77,15 @@
 ```
 
 ### Confirm User Data
 
 To verify the successful ingestion of the demo documents, you can fetch the metadata for the uploaded documents associated with the default demo user ID:
 
 ```bash
-python -m r2r.examples.demo get_user_document_data --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
+python -m r2r.examples.demo get_user_documents_metadata --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
 ```
 
 **Demo Output:**
 
 ```plaintext
 ...
 Time taken to get user document data: 0.21 seconds
@@ -203,29 +201,37 @@
 <search>["{\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... </search>
 <completion>Lyft reported a net loss of $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit in 2020.</completion>                                                      
 Time taken to stream RAG response: 2.79 seconds
 ```
 
 ## Document Management Demo
 
+### Update Document 
+
+To update document(s) we may use the `update_as_files` or `update_as_documents` endpoints. Running the demo with `update_as_files` overwrites the data associated with 'aristotle.txt' with new data corresponding to 'aristotle_v2.txt' and increments the file version.
+
+```bash
+poetry run python -m r2r.examples.demo update_as_files
+```
+
 ### Document Deletion
 
-To delete a document by its ID, or any other metadata field, use the delete command. For example, to delete all chunks corresponding to the uploaded file `aristotle.txt`, we can call delete on the associated document ID with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
+To delete a document by its ID, or any other metadata field, use the delete command. For example, to delete all chunks corresponding to the uploaded file `aristotle.txt`, we can call delete on the metadata field `document_id` with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
 
 ```bash
-python -m r2r.examples.demo delete --key=document_id --value=15255e98-e245-5b58-a57f-6c51babf72dd
+poetry run python -m r2r.examples.demo delete --keys="['document_id']" --values="['c9bdbac7-0ea3-5c9e-b590-018bd09b127b']"
 ```
 
 ### User Deletion
 
 To delete all documents associated with a given user, run the delete command on the `user_id`:
 
 ```bash
 run the following command with care, as it will erase all ingested user data
-python -m r2r.examples.demo delete --key=user_id --value=063edaf8-3e63-4cb9-a4d6-a855f36376c3
+python -m r2r.examples.demo delete --keys="['user_id']" --values="['063edaf8-3e63-4cb9-a4d6-a855f36376c3']"
 ```
 
 ## R2R Server-Client Demo
 
 This section extends the previous demo by showing how to set up and use the R2R framework with a server-client architecture. The R2R server can be stood up to handle requests, while the client can communicate with the server to perform various operations.
 
 ### Launch the Server
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 [Sciphi Framework]
         ******** BBuuiilldd,, ddeeppllooyy,, oobbsseerrvvee,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
 # About R2R, short for RAG to Riches, provides the fastest and most efficient
 way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users.
-The framework is built around customizable pipelines and a feature-rich FastAPI
-implementation. ## Why? R2R was conceived to bridge the gap between local LLM
+The framework is built around customizable pipelines and ships with a feature-
+rich REST API. ## Why? R2R was conceived to bridge the gap between local LLM
 experimentation and scalable production solutions. It is built with
 observability and customization in mind, ensuring that users can seamlessly
 transition from development to deployment. ## Key Features - **ð§ Build**:
 Use the framework to build arbitrary asynchronous pipelines. - **ð Deploy**:
 Instantly launch production-ready asynchronous RAG pipelines with streaming
 capabilities. - **ð§© Customize**: Tailor your multimodal pipeline with
 intuitive configuration files. - **ð Extend**: Enhance your pipeline with
@@ -17,53 +17,52 @@
 Contents 1. [Quick Install](#quick-install) 2. [Links](#links) 3. [R2R Demo]
 (#r2r-demo) 4. [R2R Server-Client Demo](#r2r-server-client-demo) 5. [Core
 Abstractions](#core-abstractions) 6. [Summary](#summary) # Quick Install:
 ```bash # use the `'r2r[all]'` to download all required deps pip install r2r #
 setup env export OPENAI_API_KEY=sk-... ``` ## Links [Join the Discord server]
 (https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
 docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud Docs](https://
-docs.sciphi.ai/) [Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/
-local_rag) # R2R Demo The R2R demo offers a step-by-step guide on running the
-default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests a
-list of provided provided documents and demonstrates search, RAG, and advanced
-functionality. The script at `r2r/examples/demo.py`, which powers the demo, can
-be configured and extended with sufficient developer familiarity. ## Ingest
-Demo Files To comprehensively demonstrate the RAG functionalities of the R2R
-framework, we must start by ingesting a realistic set of documents. Running the
-command below will parse, chunk, embed, and store a preset list of files. The
-included file types cover HTML, PDF, PNG, and TXT examples: ```bash python -
-m r2r.examples.demo ingest_as_files ``` **Demo Output:** ```plaintext ...
+docs.sciphi.ai/) # R2R Demo The R2R demo offers a step-by-step guide on running
+the default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests
+a list of provided provided documents and demonstrates search, RAG, and
+advanced functionality. The script at `r2r/examples/demo.py`, which powers the
+demo, can be configured and extended with sufficient developer familiarity. ##
+Ingest Demo Files To comprehensively demonstrate the RAG functionalities of the
+R2R framework, we must start by ingesting a realistic set of documents. Running
+the command below will parse, chunk, embed, and store a preset list of files.
+The included file types cover HTML, PDF, PNG, and TXT examples: ```bash python
+-m r2r.examples.demo ingest_as_files ``` **Demo Output:** ```plaintext ...
 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'pg_essay_1.html', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3'} and
 id=4a4fb848-fc03-5487-a7e5-33c9fdfb73cc in t=0.00 seconds. - 2024-05-21 08:39:
 59,003 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'lyft_2021.pdf', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3'} and
 id=c5abc0b7-b9e5-54d9-b3d3-fdb14af4d065 in t=3.47 seconds. - 2024-05-21 08:40:
 02,477 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'screen_shot.png', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3',
 'image_type': 'png'} and id=74f1506a-9a37-59d7-b288-5ef3683dca8f in t=18.37
 seconds. - 2024-05-21 08:40:32,310 ... Time taken to ingest files: 28.49
 seconds ``` ### Confirm User Data To verify the successful ingestion of the
 demo documents, you can fetch the metadata for the uploaded documents
 associated with the default demo user ID: ```bash python -m r2r.examples.demo
-get_user_document_data --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3" ```
-**Demo Output:** ```plaintext ... Time taken to get user document data: 0.21
-seconds {'results': [ { 'document_id': '327f6110-edd1-5fe3-b6b3-49b55f1cbc28',
-'title': 'pg_essay_3.html' }, { 'document_id': '946859f0-da5c-5db7-9b5c-
-c586be76d709', 'title': 'pg_essay_5.html' }, { 'document_id': '64c1c913-be06-
-548f-acbc-3618b00d3616', 'title': 'lyft_2021.pdf' }, ... ] } ``` ## Search Demo
-Documents Documents are stored by default in a local vector database. The
-vector database provider and settings can be specified via an input
-`config.json`. To perform a search query on the ingested user documents, use
-the following command: ```bash python -m r2r.examples.demo search --query="Who
-was Aristotle?" ``` **Demo Output:** ```plaintext ... Time taken to search:
-0.39 seconds { 'id': UUID('93c44e73-8e95-50c2-84af-6a42f070b552'), 'score':
-0.7739712385010018, 'metadata': { 'document_id': '15255e98-e245-5b58-a57f-
-6c51babf72dd', 'extraction_id': '5c61f9b9-b468-5fd7-8eb1-5d797a15c484', 'text':
-'Aristotle[A] (Greek: á¼ÏÎ¹ÏÏÎ¿ÏÎ­Î»Î·Ï AristotÃ©lÄs, pronounced
+get_user_documents_metadata --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
+``` **Demo Output:** ```plaintext ... Time taken to get user document data:
+0.21 seconds {'results': [ { 'document_id': '327f6110-edd1-5fe3-b6b3-
+49b55f1cbc28', 'title': 'pg_essay_3.html' }, { 'document_id': '946859f0-da5c-
+5db7-9b5c-c586be76d709', 'title': 'pg_essay_5.html' }, { 'document_id':
+'64c1c913-be06-548f-acbc-3618b00d3616', 'title': 'lyft_2021.pdf' }, ... ] } ```
+## Search Demo Documents Documents are stored by default in a local vector
+database. The vector database provider and settings can be specified via an
+input `config.json`. To perform a search query on the ingested user documents,
+use the following command: ```bash python -m r2r.examples.demo search --
+query="Who was Aristotle?" ``` **Demo Output:** ```plaintext ... Time taken to
+search: 0.39 seconds { 'id': UUID('93c44e73-8e95-50c2-84af-6a42f070b552'),
+'score': 0.7739712385010018, 'metadata': { 'document_id': '15255e98-e245-5b58-
+a57f-6c51babf72dd', 'extraction_id': '5c61f9b9-b468-5fd7-8eb1-5d797a15c484',
+'text': 'Aristotle[A] (Greek: á¼ÏÎ¹ÏÏÎ¿ÏÎ­Î»Î·Ï AristotÃ©lÄs, pronounced
 [aristotÃ©lÉËs]; 384â322 BC) was an Ancient Greek philosopher and polymath.
 His writings cover a broad range of subjects spanning the natural sciences,
 philosophy, linguistics, economics, politics, psychology, and the arts. As the
 founder of the Peripatetic school of philosophy in the Lyceum in Athens, he
 began the wider Aristotelian tradition that followed, which set the groundwork
 for the development of modern science.', 'title': 'aristotle.txt', 'user_id':
 '063edaf8-3e63-4cb9-a4d6-a855f36376c3', 'query': 'Who was Aristotle?' } } ...
@@ -81,48 +80,53 @@
 streaming results from a RAG query, use the following command: ```bash python -
 m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
 streaming=true ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
 Loading configuration from /config.json - 2024-05-20 22:27:31,890 ... ["
 {\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... Lyft reported a net loss of
 $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit
 in 2020. Time taken to stream RAG response: 2.79 seconds ``` ## Document
-Management Demo ### Document Deletion To delete a document by its ID, or any
-other metadata field, use the delete command. For example, to delete all chunks
-corresponding to the uploaded file `aristotle.txt`, we can call delete on the
-associated document ID with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
-```bash python -m r2r.examples.demo delete --key=document_id --value=15255e98-
-e245-5b58-a57f-6c51babf72dd ``` ### User Deletion To delete all documents
-associated with a given user, run the delete command on the `user_id`: ```bash
-run the following command with care, as it will erase all ingested user data
-python -m r2r.examples.demo delete --key=user_id --value=063edaf8-3e63-4cb9-
-a4d6-a855f36376c3 ``` ## R2R Server-Client Demo This section extends the
-previous demo by showing how to set up and use the R2R framework with a server-
-client architecture. The R2R server can be stood up to handle requests, while
-the client can communicate with the server to perform various operations. ###
-Launch the Server Use the following command to start the server: ```bash python
--m r2r.examples.demo serve ``` This command starts the R2R server on the
-default host `0.0.0.0` and port `8000`. ### Example Commands 1. **Ingest
-Documents as Files**: ```bash python -m r2r.examples.demo ingest_as_files --
-base_url=http://localhost:8000 ``` This command will send the ingestion request
-to the server running at `http://localhost:8000`. 2. **Perform a Search**:
-```bash python -m r2r.examples.demo search --query="Who was Aristotle?" --
-base_url=http://localhost:8000 ``` This command sends the search query to the
-server and retrieves the results. 3. **Run a RAG Completion**: ```bash python -
-m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --
-base_url=http://localhost:8000 ``` This command sends the RAG query to the
-server and retrieves the generated response. 4. **Run a RAG Stream**: ```bash
-python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=true --base_url=http://localhost:8000 ``` This command streams the
-RAG query results from the server. ### Server-Client Summary By using the
-server-client model, you can extend the basic R2R demo to support more scalable
-and modular deployments. The server handles requests and performs heavy
-computations, while clients can communicate with the server to perform
-ingestion, search, RAG, and other operations, as shown in the examples above.
-For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-
-demo). # Core Abstractions The framework revolves around three core
+Management Demo ### Update Document To update document(s) we may use the
+`update_as_files` or `update_as_documents` endpoints. Running the demo with
+`update_as_files` overwrites the data associated with 'aristotle.txt' with new
+data corresponding to 'aristotle_v2.txt' and increments the file version.
+```bash poetry run python -m r2r.examples.demo update_as_files ``` ### Document
+Deletion To delete a document by its ID, or any other metadata field, use the
+delete command. For example, to delete all chunks corresponding to the uploaded
+file `aristotle.txt`, we can call delete on the metadata field `document_id`
+with the value `15255e98-e245-5b58-a57f-6c51babf72dd`: ```bash poetry run
+python -m r2r.examples.demo delete --keys="['document_id']" --values="
+['c9bdbac7-0ea3-5c9e-b590-018bd09b127b']" ``` ### User Deletion To delete all
+documents associated with a given user, run the delete command on the
+`user_id`: ```bash run the following command with care, as it will erase all
+ingested user data python -m r2r.examples.demo delete --keys="['user_id']" --
+values="['063edaf8-3e63-4cb9-a4d6-a855f36376c3']" ``` ## R2R Server-Client Demo
+This section extends the previous demo by showing how to set up and use the R2R
+framework with a server-client architecture. The R2R server can be stood up to
+handle requests, while the client can communicate with the server to perform
+various operations. ### Launch the Server Use the following command to start
+the server: ```bash python -m r2r.examples.demo serve ``` This command starts
+the R2R server on the default host `0.0.0.0` and port `8000`. ### Example
+Commands 1. **Ingest Documents as Files**: ```bash python -m r2r.examples.demo
+ingest_as_files --base_url=http://localhost:8000 ``` This command will send the
+ingestion request to the server running at `http://localhost:8000`. 2.
+**Perform a Search**: ```bash python -m r2r.examples.demo search --query="Who
+was Aristotle?" --base_url=http://localhost:8000 ``` This command sends the
+search query to the server and retrieves the results. 3. **Run a RAG
+Completion**: ```bash python -m r2r.examples.demo rag --query="What was Uber's
+profit in 2020?" --base_url=http://localhost:8000 ``` This command sends the
+RAG query to the server and retrieves the generated response. 4. **Run a RAG
+Stream**: ```bash python -m r2r.examples.demo rag --query="What was Lyft's
+profit in 2020?" --streaming=true --base_url=http://localhost:8000 ``` This
+command streams the RAG query results from the server. ### Server-Client
+Summary By using the server-client model, you can extend the basic R2R demo to
+support more scalable and modular deployments. The server handles requests and
+performs heavy computations, while clients can communicate with the server to
+perform ingestion, search, RAG, and other operations, as shown in the examples
+above. For detailed setup and basic functionality, refer back to the [R2R Demo]
+(#r2r-demo). # Core Abstractions The framework revolves around three core
 abstractions: Providers, Pipes, and Pipelines. ## Providers Providers supply
 the necessary resources and capabilities to the pipes and pipelines. Key
 provider types include: - **Vector Database Provider**: Manages the storage and
 retrieval of vector embeddings. Examples include Qdrant, PGVector, and
 LocalVectorDB. - **Embedding Provider**: Converts text into vector embeddings.
 Supported providers include OpenAI, SentenceTransformers, and
 DummyEmbeddingProvider. - **LLM Provider**: Interfaces with large language
```

### Comparing `r2r-0.2.3/config.json` & `r2r-0.2.4/config.json`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/pyproject.toml` & `r2r-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.2.03"
+version = "0.2.04"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
@@ -61,16 +61,16 @@
 ionic-api-sdk = {version = "0.9.3", optional = true}
 exa-py = {version = "^1.0.9", optional = true}
 
 [tool.poetry.extras]
 all = ["tiktoken", "qdrant_client", "llama-cpp-python", "sentence-transformers"]
 exa = ["exa-py"]
 ionic = ["ionic-api-sdk"]
-local-llm = ["llama-cpp-python", "sentence-transformers"]
-sentence-transformers-only = ["sentence-transformers"]
+local-llm = ["llama-cpp-python"]
+local-embedding = ["sentence-transformers"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "6.1.0"
 isort = "5.12.0"
 mypy = "^1.5.1"
 pytest = "^8.2.0"
```

### Comparing `r2r-0.2.3/r2r/__init__.py` & `r2r-0.2.4/r2r/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 
 from .core import *
 from .eval import *
+from .integrations import *
 from .main import *
 from .pipes import *
+from .prebuilts import *
 from .prompts import *
 
 logger = logging.getLogger("r2r")
 logger.setLevel(logging.INFO)
 
 # Create a console handler and set the level to info
 ch = logging.StreamHandler()
@@ -23,37 +25,37 @@
 logger.addHandler(ch)
 
 # Optional: Prevent propagation to the root logger
 logger.propagate = False
 
 __all__ = [
     "LoggingConfig",
-    "LocalPipeLoggingProvider",
+    "LocalKVLoggingProvider",
     "PostgresLoggingConfig",
-    "PostgresPipeLoggingProvider",
+    "PostgresKVLoggingProvider",
     "RedisLoggingConfig",
-    "RedisPipeLoggingProvider",
-    "PipeLoggingConnectionSingleton",
+    "RedisKVLoggingProvider",
+    "KVLoggingSingleton",
     "VectorEntry",
     "VectorType",
     "Vector",
     "SearchRequest",
     "SearchResult",
     "AsyncPipe",
-    "PipeRunInfo",
     "PipeType",
     "AsyncState",
     "Prompt",
     "DataType",
     "DocumentType",
     "Document",
     "Extraction",
     "ExtractionType",
     "Fragment",
     "FragmentType",
+    "SearchPipe",
     # Parsers
     "AsyncParser",
     "CSVParser",
     "DOCXParser",
     "HTMLParser",
     "JSONParser",
     "MarkdownParser",
@@ -89,8 +91,15 @@
     "R2RDocumentParsingPipe",
     "R2RQueryTransformPipe",
     "R2RRAGPipe",
     "R2RStreamingRAGPipe",
     "R2RVectorSearchPipe",
     "R2RVectorStoragePipe",
     "R2RPromptProvider",
+    "R2RWebSearchPipe",
+    "R2RAppBuilder",
+    # Prebuilts
+    "MultiSearchPipe",
+    "R2RPipeFactoryWithMultiSearch",
+    # Integrations
+    "SerperClient",
 ]
```

### Comparing `r2r-0.2.3/r2r/core/__init__.py` & `r2r-0.2.4/r2r/core/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,24 @@
     Fragment,
     FragmentType,
 )
 from .abstractions.llm import LLMChatCompletion, LLMChatCompletionChunk
 from .abstractions.prompt import Prompt
 from .abstractions.search import SearchRequest, SearchResult
 from .abstractions.vector import Vector, VectorEntry, VectorType
+from .logging.kv_logger import (
+    KVLoggingSingleton,
+    LocalKVLoggingProvider,
+    LoggingConfig,
+    PostgresKVLoggingProvider,
+    PostgresLoggingConfig,
+    RedisKVLoggingProvider,
+    RedisLoggingConfig,
+)
+from .logging.run_manager import RunManager, manage_run
 from .parsers import (
     AsyncParser,
     AudioParser,
     CSVParser,
     DOCXParser,
     HTMLParser,
     ImageParser,
@@ -29,56 +39,49 @@
 from .pipeline.base_pipeline import (
     EvalPipeline,
     IngestionPipeline,
     Pipeline,
     RAGPipeline,
     SearchPipeline,
 )
-from .pipes.base_pipe import AsyncPipe, AsyncState, PipeRunInfo, PipeType
+from .pipes.base_pipe import AsyncPipe, AsyncState, PipeType
 from .pipes.loggable_pipe import LoggableAsyncPipe
-from .pipes.pipe_logging import (
-    LocalPipeLoggingProvider,
-    LoggingConfig,
-    PipeLoggingConnectionSingleton,
-    PostgresLoggingConfig,
-    PostgresPipeLoggingProvider,
-    RedisLoggingConfig,
-    RedisPipeLoggingProvider,
-)
 from .providers.embedding_provider import EmbeddingConfig, EmbeddingProvider
 from .providers.eval_provider import EvalConfig, EvalProvider
 from .providers.llm_provider import GenerationConfig, LLMConfig, LLMProvider
 from .providers.prompt_provider import PromptConfig, PromptProvider
 from .providers.vector_db_provider import VectorDBConfig, VectorDBProvider
 from .utils import (
     RecursiveCharacterTextSplitter,
     TextSplitter,
     generate_id_from_label,
     generate_run_id,
+    increment_version,
     run_pipeline,
     to_async_generator,
 )
 
 __all__ = [
     # Logging
     "LoggingConfig",
-    "LocalPipeLoggingProvider",
+    "LocalKVLoggingProvider",
     "PostgresLoggingConfig",
-    "PostgresPipeLoggingProvider",
+    "PostgresKVLoggingProvider",
     "RedisLoggingConfig",
-    "RedisPipeLoggingProvider",
-    "PipeLoggingConnectionSingleton",
+    "RedisKVLoggingProvider",
+    "KVLoggingSingleton",
+    "RunManager",
+    "manage_run",
     # Abstractions
     "VectorEntry",
     "VectorType",
     "Vector",
     "SearchRequest",
     "SearchResult",
     "AsyncPipe",
-    "PipeRunInfo",
     "PipeType",
     "AsyncState",
     "LoggableAsyncPipe",
     "Prompt",
     "DataType",
     "DocumentType",
     "Document",
@@ -120,11 +123,12 @@
     "LLMProvider",
     "VectorDBConfig",
     "VectorDBProvider",
     # Other
     "TextSplitter",
     "RecursiveCharacterTextSplitter",
     "to_async_generator",
+    "increment_version",
     "run_pipeline",
     "generate_run_id",
     "generate_id_from_label",
 ]
```

### Comparing `r2r-0.2.3/r2r/core/abstractions/document.py` & `r2r-0.2.4/r2r/core/abstractions/document.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/abstractions/prompt.py` & `r2r-0.2.4/r2r/core/abstractions/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/abstractions/search.py` & `r2r-0.2.4/r2r/core/abstractions/search.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/abstractions/vector.py` & `r2r-0.2.4/r2r/core/abstractions/vector.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/parsers/__init__.py` & `r2r-0.2.4/r2r/core/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/parsers/parser_impls.py` & `r2r-0.2.4/r2r/core/parsers/parser_impls.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/pipeline/base_pipeline.py` & `r2r-0.2.4/r2r/core/pipeline/base_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 """Base pipeline class for running a sequence of pipes."""
 import asyncio
-from contextlib import asynccontextmanager
 import logging
-import uuid
 from enum import Enum
 from typing import Any, AsyncGenerator, Optional
 
+from ..logging.kv_logger import KVLoggingSingleton
+from ..logging.run_manager import RunManager, manage_run
 from ..pipes.base_pipe import AsyncPipe, AsyncState
-from ..pipes.pipe_logging import PipeLoggingConnectionSingleton
-from ..utils import generate_run_id
 
 logger = logging.getLogger(__name__)
 
 
 class PipelineTypes(Enum):
     EVAL = "eval"
     INGESTION = "ingestion"
     SEARCH = "search"
     RAG = "rag"
     OTHER = "other"
 
 
-@asynccontextmanager
-async def manage_run_id(pipeline: "Pipeline"):
-    try:
-        pipeline.run_id = generate_run_id()
-        yield
-    finally:
-        pipeline.run_id = None
-
-
 class Pipeline:
     """Pipeline class for running a sequence of pipes."""
 
     pipeline_type: str = "other"
 
     def __init__(
-        self, pipe_logger: Optional[PipeLoggingConnectionSingleton] = None
+        self,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
+        run_manager: Optional[RunManager] = None,
     ):
         self.pipes: list[AsyncPipe] = []
         self.upstream_outputs: list[list[dict[str, str]]] = []
-        self.pipe_logger = pipe_logger or PipeLoggingConnectionSingleton()
+        self.pipe_logger = pipe_logger or KVLoggingSingleton()
+        self.run_manager = run_manager or RunManager(self.pipe_logger)
         self.futures = {}
         self.level = 0
-        # self.run_id = None
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
@@ -59,58 +50,57 @@
         self.upstream_outputs.append(add_upstream_outputs)
 
     async def run(
         self,
         input: Any,
         state: Optional[AsyncState] = None,
         streaming: bool = False,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ):
         """Run the pipeline."""
+        run_manager = run_manager or self.run_manager
+
         try:
             PipelineTypes(self.pipeline_type)
         except ValueError:
             raise ValueError(
                 f"Invalid pipeline type: {self.pipeline_type}, must be one of {PipelineTypes.__members__.keys()}"
             )
 
         self.state = state or AsyncState()
         current_input = input
-        async with manage_run_id(self):
-            await self.pipe_logger.log(
-                pipe_run_id=self.run_id,
+        async with manage_run(run_manager, self.pipeline_type) as run_id:
+            await run_manager.log_run_info(
                 key="pipeline_type",
                 value=self.pipeline_type,
-                is_pipeline_info=True,
+                is_info_log=True,
             )
             try:
                 for pipe_num in range(len(self.pipes)):
                     config_name = self.pipes[pipe_num].config.name
                     self.futures[config_name] = asyncio.Future()
 
                     current_input = self._run_pipe(
                         pipe_num,
-                        self.run_id,
                         current_input,
+                        run_manager,
                         *args,
-                        **kwargs,  # pass run_id to retain value throughout execution.
+                        **kwargs,
                     )
                     self.futures[config_name].set_result(current_input)
-
                 if not streaming:
                     final_result = await self._consume_all(current_input)
                     return final_result
                 else:
                     return current_input
             except Exception as error:
                 logger.error(f"Pipeline failed with error: {error}")
                 raise error
-            finally:
-                pass
 
     async def _consume_all(self, gen: AsyncGenerator) -> list[Any]:
         result = []
         async for item in gen:
             if hasattr(
                 item, "__aiter__"
             ):  # Check if the item is an async generator
@@ -119,16 +109,16 @@
             else:
                 result.append(item)
         return result
 
     async def _run_pipe(
         self,
         pipe_num: int,
-        run_id: uuid.UUID,
         input: Any,
+        run_manager: RunManager,
         *args: Any,
         **kwargs: Any,
     ):
         # Collect inputs, waiting for the necessary futures
         pipe = self.pipes[pipe_num]
         add_upstream_outputs = self.sort_upstream_outputs(
             self.upstream_outputs[pipe_num]
@@ -176,15 +166,15 @@
                     prev_output_field
                 ]
 
         # Handle the pipe generator
         async for ele in await pipe.run(
             pipe.Input(**input_dict),
             self.state,
-            run_id=run_id,
+            run_manager,
             *args,
             **kwargs,
         ):
             yield ele
 
     def sort_upstream_outputs(
         self, add_upstream_outputs: list[dict[str, str]]
@@ -208,18 +198,21 @@
     pipeline_type: str = "eval"
 
     async def run(
         self,
         input: Any,
         state: Optional[AsyncState] = None,
         streaming: bool = False,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ):
-        return await super().run(input, state, streaming, *args, **kwargs)
+        return await super().run(
+            input, state, streaming, run_manager, *args, **kwargs
+        )
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
@@ -234,18 +227,21 @@
     pipeline_type: str = "ingestion"
 
     async def run(
         self,
         input: Any,
         state: Optional[AsyncState] = None,
         streaming: bool = False,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ):
-        return await super().run(input, state, streaming, *args, **kwargs)
+        return await super().run(
+            input, state, streaming, run_manager, *args, **kwargs
+        )
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
@@ -262,18 +258,21 @@
     pipeline_type: str = "rag"
 
     async def run(
         self,
         input: Any,
         state: Optional[AsyncState] = None,
         streaming: bool = False,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ):
-        return await super().run(input, state, streaming, *args, **kwargs)
+        return await super().run(
+            input, state, streaming, run_manager, *args, **kwargs
+        )
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
@@ -288,18 +287,21 @@
     pipeline_type: str = "search"
 
     async def run(
         self,
         input: Any,
         state: Optional[AsyncState] = None,
         streaming: bool = False,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ):
-        return await super().run(input, state, streaming, *args, **kwargs)
+        return await super().run(
+            input, state, streaming, run_manager, *args, **kwargs
+        )
 
     def add_pipe(
         self,
         pipe: AsyncPipe,
         add_upstream_outputs: Optional[list[dict[str, str]]] = None,
         *args,
         **kwargs,
```

### Comparing `r2r-0.2.3/r2r/core/pipes/base_pipe.py` & `r2r-0.2.4/r2r/core/pipes/base_pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-from contextlib import asynccontextmanager
 import asyncio
 import logging
 import uuid
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, AsyncGenerator, Optional
 
 from pydantic import BaseModel
 
-from ..utils import generate_run_id
-
 logger = logging.getLogger(__name__)
 
 
 class PipeType(Enum):
     INGESTOR = "ingestor"
     EVAL = "eval"
     GENERATOR = "generator"
     SEARCH = "search"
     TRANSFORM = "transform"
     OTHER = "other"
 
 
-class PipeRunInfo(BaseModel):
-    """Information about a pipe run."""
-
-    run_id: uuid.UUID
-
-
 class AsyncState:
     """A state object for storing data between pipes."""
 
     def __init__(self):
         self.data = {}
         self.lock = asyncio.Lock()
 
@@ -65,26 +56,14 @@
                 if inner_key not in self.data[outer_key]:
                     raise ValueError(
                         f"Key {inner_key} does not exist in the state."
                     )
                 del self.data[outer_key][inner_key]
 
 
-@asynccontextmanager
-async def manage_run_info(
-    pipe: "AsyncPipe", run_id: Optional[uuid.UUID] = None
-):
-    try:
-        run_id = run_id or generate_run_id()
-        pipe._run_info = PipeRunInfo(run_id=run_id)
-        yield
-    finally:
-        pipe.run_id = None
-
-
 class AsyncPipe(ABC):
     """An asynchronous pipe for processing data."""
 
     class PipeConfig(BaseModel):
         """Configuration for a pipe."""
 
         name: str = "default_pipe"
@@ -117,28 +96,22 @@
     def config(self) -> PipeConfig:
         return self._config
 
     @property
     def type(self) -> PipeType:
         return self._type
 
-    @property
-    def run_info(self) -> PipeRunInfo:
-        return self._run_info
-
     async def run(
         self,
         input: Input,
         state: AsyncState,
-        run_id: Optional[uuid.UUID] = None,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[Any, None]:
-        async with manage_run_info(self, run_id):
-            result = self._run_logic(input, state)
-            return result
+        result = self._run_logic(input, state)
+        return result
 
     @abstractmethod
     async def _run_logic(
         self, input: Input, state: AsyncState, *args: Any, **kwargs: Any
     ) -> AsyncGenerator[Any, None]:
         pass
```

### Comparing `r2r-0.2.3/r2r/core/pipes/loggable_pipe.py` & `r2r-0.2.4/r2r/core/pipes/loggable_pipe.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,70 +1,86 @@
 import asyncio
 import uuid
+from abc import ABC, abstractmethod
 from typing import Any, AsyncGenerator, Optional
 
-from .base_pipe import AsyncPipe, AsyncState, PipeType, manage_run_info
-from .pipe_logging import PipeLoggingConnectionSingleton
+from ..logging.kv_logger import KVLoggingSingleton
+from ..logging.run_manager import RunManager, manage_run
+from .base_pipe import AsyncPipe, AsyncState, PipeType
 
 
 class LoggableAsyncPipe(AsyncPipe):
     """An asynchronous pipe for processing data with logging capabilities."""
 
     class PipeConfig(AsyncPipe.PipeConfig):
         """Configuration for a loggable pipe."""
 
         name: str = "default_loggable_pipe"
         max_log_queue_size: int = 100
 
     def __init__(
         self,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.OTHER,
         config: Optional[AsyncPipe.PipeConfig] = None,
+        run_manager: Optional[RunManager] = None,
         *args,
         **kwargs,
     ):
         if not pipe_logger:
-            pipe_logger = PipeLoggingConnectionSingleton()
+            pipe_logger = KVLoggingSingleton()
         self.pipe_logger = pipe_logger
         self.log_queue = asyncio.Queue()
         self.log_worker_task = None
-
+        self._run_manager = run_manager or RunManager(pipe_logger)
         super().__init__(type=type, config=config, *args, **kwargs)
 
     async def log_worker(self):
         while True:
             log_data = await self.log_queue.get()
-            pipe_run_id, key, value = log_data
-            await self.pipe_logger.log(pipe_run_id, key, value)
+            run_id, key, value = log_data
+            await self.pipe_logger.log(run_id, key, value)
             self.log_queue.task_done()
 
-    async def enqueue_log(self, pipe_run_id: str, key: str, value: str):
+    async def enqueue_log(self, run_id: uuid.UUID, key: str, value: str):
         if self.log_queue.qsize() < self.config.max_log_queue_size:
-            await self.log_queue.put((pipe_run_id, key, value))
+            await self.log_queue.put((run_id, key, value))
 
     async def run(
         self,
         input: AsyncPipe.Input,
         state: AsyncState,
-        run_id: Optional[uuid.UUID] = None,
+        run_manager: Optional[RunManager] = None,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[Any, None]:
         """Run the pipe with logging capabilities."""
 
+        run_manager = run_manager or self._run_manager
+
         async def wrapped_run() -> AsyncGenerator[Any, None]:
-            async with manage_run_info(self, run_id):
+            async with manage_run(run_manager, self.config.name) as run_id:
                 self.log_worker_task = asyncio.create_task(
                     self.log_worker(), name=f"log-worker-{self.config.name}"
                 )
                 try:
                     async for result in self._run_logic(
-                        input, state, *args, **kwargs
+                        input, state, run_id=run_id, *args, **kwargs
                     ):
                         yield result
                 finally:
                     await self.log_queue.join()
                     self.log_worker_task.cancel()
                     self.log_queue = asyncio.Queue()
 
         return wrapped_run()
+
+    @abstractmethod
+    async def _run_logic(
+        self,
+        input: AsyncPipe.Input,
+        state: AsyncState,
+        run_id: uuid.UUID,
+        *args: Any,
+        **kwargs: Any,
+    ) -> AsyncGenerator[Any, None]:
+        pass
```

### Comparing `r2r-0.2.3/r2r/core/pipes/pipe_logging.py` & `r2r-0.2.4/r2r/core/logging/kv_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..providers.base_provider import Provider, ProviderConfig
 
 logger = logging.getLogger(__name__)
 
 
 class RunInfo(BaseModel):
     run_id: uuid.UUID
-    pipeline_type: str
+    log_type: str
 
 
 class LoggingConfig(ProviderConfig):
     provider: str = "local"
     log_table: str = "logs"
     log_info_table: str = "logs_pipeline_info"
     logging_path: Optional[str] = None
@@ -29,37 +29,39 @@
         pass
 
     @property
     def supported_providers(self) -> list[str]:
         return ["local", "postgres", "redis"]
 
 
-class PipeLoggingProvider(Provider):
+class KVLoggingProvider(Provider):
     @abstractmethod
     async def close(self):
         pass
 
     @abstractmethod
-    async def log(self, pipe_run_id: uuid.UUID, key: str, value: str):
+    async def log(self, log_id: uuid.UUID, key: str, value: str):
         pass
 
     @abstractmethod
     async def get_run_info(
-        self, key: Optional[str] = None, pipeline_type: Optional[str] = None
+        self,
+        log_type: Optional[str] = None,
+        log_type_filter: Optional[str] = None,
     ) -> list[RunInfo]:
         pass
 
     @abstractmethod
     async def get_logs(
         self, run_ids: list[uuid.UUID], limit_per_run: int
     ) -> list:
         pass
 
 
-class LocalPipeLoggingProvider(PipeLoggingProvider):
+class LocalKVLoggingProvider(KVLoggingProvider):
     def __init__(self, config: LoggingConfig):
         self.log_table = config.log_table
         self.log_info_table = config.log_info_table
         self.logging_path = config.logging_path or os.getenv(
             "LOCAL_DB_PATH", "local.sqlite"
         )
         if not self.logging_path:
@@ -69,35 +71,35 @@
         self.conn = None
         try:
             import aiosqlite
 
             self.aiosqlite = aiosqlite
         except ImportError:
             raise ImportError(
-                "Please install aiosqlite to use the LocalPipeLoggingProvider."
+                "Please install aiosqlite to use the LocalKVLoggingProvider."
             )
 
     async def init(self):
         self.conn = await self.aiosqlite.connect(self.logging_path)
         await self.conn.execute(
             f"""
             CREATE TABLE IF NOT EXISTS {self.log_table} (
                 timestamp DATETIME,
-                pipe_run_id TEXT,
+                log_id TEXT,
                 key TEXT,
                 value TEXT
             )
             """
         )
         await self.conn.execute(
             f"""
             CREATE TABLE IF NOT EXISTS {self.log_info_table} (
                 timestamp DATETIME,
-                pipe_run_id TEXT UNIQUE,
-                pipeline_type TEXT
+                log_id TEXT UNIQUE,
+                log_type TEXT
             )
         """
         )
         await self.conn.commit()
 
     async def __aenter__(self):
         if self.conn is None:
@@ -110,71 +112,68 @@
     async def close(self):
         if self.conn:
             await self.conn.close()
             self.conn = None
 
     async def log(
         self,
-        pipe_run_id: uuid.UUID,
+        log_id: uuid.UUID,
         key: str,
         value: str,
-        is_pipeline_info=False,
+        is_info_log=False,
     ):
-        collection = (
-            self.log_info_table if is_pipeline_info else self.log_table
-        )
+        collection = self.log_info_table if is_info_log else self.log_table
 
-        if is_pipeline_info:
-            if key != "pipeline_type":
-                raise ValueError("Metadata keys must be 'pipeline_type'")
+        if is_info_log:
+            if "type" not in key:
+                raise ValueError("Info log keys must contain the text 'type'")
             await self.conn.execute(
-                f"INSERT INTO {collection} (timestamp, pipe_run_id, pipeline_type) VALUES (datetime('now'), ?, ?)",
-                (str(pipe_run_id), value),
+                f"INSERT INTO {collection} (timestamp, log_id, log_type) VALUES (datetime('now'), ?, ?)",
+                (str(log_id), value),
             )
         else:
             await self.conn.execute(
-                f"INSERT INTO {collection} (timestamp, pipe_run_id, key, value) VALUES (datetime('now'), ?, ?, ?)",
-                (str(pipe_run_id), key, value),
+                f"INSERT INTO {collection} (timestamp, log_id, key, value) VALUES (datetime('now'), ?, ?, ?)",
+                (str(log_id), key, value),
             )
         await self.conn.commit()
 
     async def get_run_info(
-        self, pipeline_type: Optional[str] = None, limit: int = 10
+        self, limit: int = 10, log_type_filter: Optional[str] = None
     ) -> list[RunInfo]:
         cursor = await self.conn.cursor()
-        query = f"SELECT pipe_run_id, pipeline_type FROM {self.log_info_table}"
+        query = f"SELECT log_id, log_type FROM {self.log_info_table}"
         conditions = []
         params = []
-        if pipeline_type:
-            conditions.append("pipeline_type = ?")
-            params.append(pipeline_type)
+        if log_type_filter:
+            conditions.append("log_type = ?")
+            params.append(log_type_filter)
         if conditions:
             query += " WHERE " + " AND ".join(conditions)
         query += " ORDER BY timestamp DESC LIMIT ?"
         params.append(limit)
         await cursor.execute(query, params)
         rows = await cursor.fetchall()
         return [
-            RunInfo(run_id=uuid.UUID(row[0]), pipeline_type=row[1])
-            for row in rows
+            RunInfo(run_id=uuid.UUID(row[0]), log_type=row[1]) for row in rows
         ]
 
     async def get_logs(
         self, run_ids: list[uuid.UUID], limit_per_run: int = 10
     ) -> list:
         if not run_ids:
             raise ValueError("No run ids provided.")
         cursor = await self.conn.cursor()
         placeholders = ",".join(["?" for _ in run_ids])
         query = f"""
         SELECT *
         FROM (
-            SELECT *, ROW_NUMBER() OVER (PARTITION BY pipe_run_id ORDER BY timestamp DESC) as rn
+            SELECT *, ROW_NUMBER() OVER (PARTITION BY log_id ORDER BY timestamp DESC) as rn
             FROM {self.log_table}
-            WHERE pipe_run_id IN ({placeholders})
+            WHERE log_id IN ({placeholders})
         )
         WHERE rn <= ?
         ORDER BY timestamp DESC
         """
         params = [str(ele) for ele in run_ids] + [limit_per_run]
         await cursor.execute(query, params)
         rows = await cursor.fetchall()
@@ -207,15 +206,15 @@
                 raise ValueError(f"Environment variable {var} is not set.")
 
     @property
     def supported_providers(self) -> list[str]:
         return ["postgres"]
 
 
-class PostgresPipeLoggingProvider(PipeLoggingProvider):
+class PostgresKVLoggingProvider(KVLoggingProvider):
     def __init__(self, config: PostgresLoggingConfig):
         self.log_table = config.log_table
         self.log_info_table = config.log_info_table
         self.config = config
         self.conn = None
         if not os.getenv("POSTGRES_DBNAME"):
             raise ValueError(
@@ -246,26 +245,26 @@
             host=os.getenv("POSTGRES_HOST"),
             port=os.getenv("POSTGRES_PORT"),
         )
         await self.conn.execute(
             f"""
             CREATE TABLE IF NOT EXISTS {self.log_table} (
                 timestamp TIMESTAMPTZ,
-                pipe_run_id UUID,
+                log_id UUID,
                 key TEXT,
                 value TEXT
             )
             """
         )
         await self.conn.execute(
             f"""
             CREATE TABLE IF NOT EXISTS {self.log_info_table} (
                 timestamp TIMESTAMPTZ,
-                pipe_run_id UUID UNIQUE,
-                pipeline_type TEXT
+                log_id UUID UNIQUE,
+                log_type TEXT
             )
         """
         )
 
     async def __aenter__(self):
         if self.conn is None:
             await self.init()
@@ -277,72 +276,70 @@
     async def close(self):
         if self.conn:
             await self.conn.close()
             self.conn = None
 
     async def log(
         self,
-        pipe_run_id: uuid.UUID,
+        log_id: uuid.UUID,
         key: str,
         value: str,
-        is_pipeline_info=False,
+        is_info_log=False,
     ):
-        collection = (
-            self.log_info_table if is_pipeline_info else self.log_table
-        )
+        collection = self.log_info_table if is_info_log else self.log_table
 
-        if is_pipeline_info:
-            if key != "pipeline_type":
-                raise ValueError("Metadata keys must be 'pipeline_type'")
+        if is_info_log:
+            if "type" not in key:
+                raise ValueError(
+                    "Info log key must contain the string `type`."
+                )
             await self.conn.execute(
-                f"INSERT INTO {collection} (timestamp, pipe_run_id, pipeline_type) VALUES (NOW(), $1, $2)",
-                pipe_run_id,
+                f"INSERT INTO {collection} (timestamp, log_id, log_type) VALUES (NOW(), $1, $2)",
+                log_id,
                 value,
             )
         else:
             await self.conn.execute(
-                f"INSERT INTO {collection} (timestamp, pipe_run_id, key, value) VALUES (NOW(), $1, $2, $3)",
-                pipe_run_id,
+                f"INSERT INTO {collection} (timestamp, log_id, key, value) VALUES (NOW(), $1, $2, $3)",
+                log_id,
                 key,
                 value,
             )
 
     async def get_run_info(
-        self, pipeline_type: Optional[str] = None, limit: int = 10
+        self, limit: int = 10, log_type_filter: Optional[str] = None
     ) -> list[RunInfo]:
-        query = f"SELECT pipe_run_id, pipeline_type FROM {self.log_info_table}"
+        query = f"SELECT log_id, log_type FROM {self.log_info_table}"
         conditions = []
         params = []
-        if pipeline_type:
-            conditions.append("pipeline_type = $1")
-            params.append(pipeline_type)
+        if log_type_filter:
+            conditions.append("log_type = $1")
+            params.append(log_type_filter)
         if conditions:
             query += " WHERE " + " AND ".join(conditions)
         query += " ORDER BY timestamp DESC LIMIT $2"
         params.append(limit)
         rows = await self.conn.fetch(query, *params)
         return [
-            RunInfo(
-                run_id=row["pipe_run_id"], pipeline_type=row["pipeline_type"]
-            )
+            RunInfo(run_id=row["log_id"], log_type=row["log_type"])
             for row in rows
         ]
 
     async def get_logs(
         self, run_ids: list[uuid.UUID], limit_per_run: int = 10
     ) -> list:
         if not run_ids:
             raise ValueError("No run ids provided.")
 
         placeholders = ",".join([f"${i+1}" for i in range(len(run_ids))])
         query = f"""
         SELECT * FROM (
-            SELECT *, ROW_NUMBER() OVER (PARTITION BY pipe_run_id ORDER BY timestamp DESC) as rn
+            SELECT *, ROW_NUMBER() OVER (PARTITION BY log_id ORDER BY timestamp DESC) as rn
             FROM {self.log_table}
-            WHERE pipe_run_id::text IN ({placeholders})
+            WHERE log_id::text IN ({placeholders})
         ) sub
         WHERE sub.rn <= ${len(run_ids) + 1}
         ORDER BY sub.timestamp DESC
         """
         params = [str(run_id) for run_id in run_ids] + [limit_per_run]
         rows = await self.conn.fetch(query, *params)
         return [{key: row[key] for key in row.keys()} for row in rows]
@@ -360,15 +357,15 @@
                 raise ValueError(f"Environment variable {var} is not set.")
 
     @property
     def supported_providers(self) -> list[str]:
         return ["redis"]
 
 
-class RedisPipeLoggingProvider(PipeLoggingProvider):
+class RedisKVLoggingProvider(KVLoggingProvider):
     def __init__(self, config: RedisLoggingConfig):
         if not all(
             [
                 os.getenv("REDIS_CLUSTER_IP"),
                 os.getenv("REDIS_CLUSTER_PORT"),
             ]
         ):
@@ -389,131 +386,129 @@
         self.log_info_key = config.log_info_table
 
     async def close(self):
         await self.redis.close()
 
     async def log(
         self,
-        pipe_run_id: uuid.UUID,
+        log_id: uuid.UUID,
         key: str,
         value: str,
-        is_pipeline_info=False,
+        is_info_log=False,
     ):
         timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         log_entry = {
             "timestamp": timestamp,
-            "pipe_run_id": str(pipe_run_id),
+            "log_id": str(log_id),
             "key": key,
             "value": value,
         }
-        if is_pipeline_info:
-            if key != "pipeline_type":
-                raise ValueError("Metadata keys must be 'pipeline_type'")
-            log_entry["pipeline_type"] = value
+        if is_info_log:
+            if "type" not in key:
+                raise ValueError("Metadata keys must contain the text 'type'")
+            log_entry["log_type"] = value
             await self.redis.hset(
-                self.log_info_key, str(pipe_run_id), json.dumps(log_entry)
+                self.log_info_key, str(log_id), json.dumps(log_entry)
             )
         else:
             await self.redis.lpush(
-                f"{self.log_key}:{str(pipe_run_id)}", json.dumps(log_entry)
+                f"{self.log_key}:{str(log_id)}", json.dumps(log_entry)
             )
 
     async def get_run_info(
-        self, pipeline_type: Optional[str] = None, limit: int = 10
+        self, log_type_filter: Optional[str] = None, limit: int = 10
     ) -> list[RunInfo]:
-        if pipeline_type:
+        if log_type_filter:
             keys = await self.redis.hkeys(self.log_info_key)
             matched_ids = []
             for key in keys:
                 log_entry = json.loads(
                     await self.redis.hget(self.log_info_key, key)
                 )
-                if log_entry["pipeline_type"] == pipeline_type:
+                if log_entry["log_type"] == log_type_filter:
                     matched_ids.append(
                         RunInfo(
-                            run_id=uuid.UUID(log_entry["pipe_run_id"]),
-                            pipeline_type=log_entry["pipeline_type"],
+                            run_id=uuid.UUID(log_entry["log_id"]),
+                            log_type=log_entry["log_type"],
                         )
                     )
             return matched_ids[:limit]
         else:
             keys = await self.redis.hkeys(self.log_info_key)
             return [
                 RunInfo(
                     run_id=uuid.UUID(key),
-                    pipeline_type=json.loads(
+                    log_type=json.loads(
                         await self.redis.hget(self.log_info_key, key)
-                    )["pipeline_type"],
+                    )["log_type"],
                 )
                 for key in keys[:limit]
             ]
 
     async def get_logs(
         self, run_ids: list[uuid.UUID], limit_per_run: int = 10
     ) -> list:
         logs = []
         for run_id in run_ids:
             raw_logs = await self.redis.lrange(
                 f"{self.log_key}:{str(run_id)}", 0, limit_per_run - 1
             )
             for raw_log in raw_logs:
                 json_log = json.loads(raw_log)
-                json_log["pipe_run_id"] = uuid.UUID(json_log["pipe_run_id"])
+                json_log["log_id"] = uuid.UUID(json_log["log_id"])
                 logs.append(json_log)
         return logs
 
 
-class PipeLoggingConnectionSingleton:
+class KVLoggingSingleton:
     _instance = None
     _is_configured = False
 
     SUPPORTED_PROVIDERS = {
-        "local": LocalPipeLoggingProvider,
-        "postgres": PostgresPipeLoggingProvider,
-        "redis": RedisPipeLoggingProvider,
+        "local": LocalKVLoggingProvider,
+        "postgres": PostgresKVLoggingProvider,
+        "redis": RedisKVLoggingProvider,
     }
 
     @classmethod
     def get_instance(cls):
         return cls.SUPPORTED_PROVIDERS[cls._config.provider](cls._config)
 
     @classmethod
     def configure(
         cls, logging_config: Optional[LoggingConfig] = LoggingConfig()
     ):
         if not cls._is_configured:
             cls._config = logging_config
             cls._is_configured = True
         else:
-            raise Exception(
-                "PipeLoggingConnectionSingleton is already configured."
-            )
+            raise Exception("KVLoggingSingleton is already configured.")
 
     @classmethod
     async def log(
         cls,
-        pipe_run_id: uuid.UUID,
+        log_id: uuid.UUID,
         key: str,
         value: str,
-        is_pipeline_info=False,
+        is_info_log=False,
     ):
         try:
             async with cls.get_instance() as provider:
-                await provider.log(
-                    pipe_run_id, key, value, is_pipeline_info=is_pipeline_info
-                )
+                await provider.log(log_id, key, value, is_info_log=is_info_log)
         except Exception as e:
             logger.error(f"Error logging data: {e}")
 
     @classmethod
     async def get_run_info(
-        cls, pipeline_type: Optional[str] = None, limit: int = 10
+        cls, limit: int = 10, log_type_filter: Optional[str] = None
     ) -> list[RunInfo]:
         async with cls.get_instance() as provider:
-            return await provider.get_run_info(pipeline_type, limit)
+            return await provider.get_run_info(
+                limit, log_type_filter=log_type_filter
+            )
 
     @classmethod
     async def get_logs(
         cls, run_ids: list[uuid.UUID], limit_per_run: int = 10
     ) -> list:
         async with cls.get_instance() as provider:
             return await provider.get_logs(run_ids, limit_per_run)
```

### Comparing `r2r-0.2.3/r2r/core/providers/base_provider.py` & `r2r-0.2.4/r2r/core/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/providers/embedding_provider.py` & `r2r-0.2.4/r2r/core/providers/embedding_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/providers/eval_provider.py` & `r2r-0.2.4/r2r/core/providers/eval_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from abc import abstractmethod
 from typing import Union
 
 from .base_provider import Provider, ProviderConfig
 from .llm_provider import LLMConfig
 
 
 class EvalConfig(ProviderConfig):
```

### Comparing `r2r-0.2.3/r2r/core/providers/llm_provider.py` & `r2r-0.2.4/r2r/core/providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/core/providers/prompt_provider.py` & `r2r-0.2.4/r2r/core/providers/prompt_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,17 @@
             raise ValueError(
                 "PromptProvider must be initialized with a `PromptConfig`."
             )
         logger.info(f"Initializing PromptProvider with config {config}.")
         super().__init__(config)
 
     @abstractmethod
-    def add_prompt(self, prompt_name: str, prompt: str) -> None:
+    def add_prompt(
+        self, name: str, template: str, input_types: dict[str, str]
+    ) -> None:
         pass
 
     @abstractmethod
     def get_prompt(
         self, prompt_name: str, inputs: Optional[dict[str, Any]] = None
     ) -> str:
         pass
```

### Comparing `r2r-0.2.3/r2r/core/providers/vector_db_provider.py` & `r2r-0.2.4/r2r/core/providers/vector_db_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,22 @@
         self, entries: list[VectorEntry], commit: bool = True
     ) -> None:
         for entry in entries:
             self.copy(entry, commit=commit)
 
     @abstractmethod
     def delete_by_metadata(
-        self, metadata_field: str, metadata_value: Union[bool, int, str]
+        self,
+        metadata_fields: list[str],
+        metadata_values: list[Union[bool, int, str]],
     ) -> None:
+        if len(metadata_fields) != len(metadata_values):
+            raise ValueError(
+                "The number of metadata fields and values must be equal."
+            )
         pass
 
     @abstractmethod
     def get_metadatas(
         self,
         metadata_fields: list[str],
         filter_field: Optional[str] = None,
```

### Comparing `r2r-0.2.3/r2r/core/utils/base_utils.py` & `r2r-0.2.4/r2r/core/utils/base_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,7 +27,13 @@
     elif not isinstance(input, AsyncGenerator):
         input = to_async_generator(input)
 
     async def _run_pipeline(input, *args, **kwargs):
         return await pipeline.run(input, *args, **kwargs)
 
     return asyncio.run(_run_pipeline(input, *args, **kwargs))
+
+
+def increment_version(version: str) -> str:
+    prefix = version[:-1]
+    suffix = int(version[-1])
+    return f"{prefix}{suffix + 1}"
```

### Comparing `r2r-0.2.3/r2r/core/utils/splitter/text.py` & `r2r-0.2.4/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/embeddings/dummy/provider.py` & `r2r-0.2.4/r2r/embeddings/dummy/provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/embeddings/openai/openai_base.py` & `r2r-0.2.4/r2r/embeddings/openai/openai_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 
-from openai import AsyncOpenAI, OpenAI
+from openai import AsyncOpenAI, OpenAI, AuthenticationError
 
 from r2r.core import EmbeddingConfig, EmbeddingProvider, SearchResult
 
 logger = logging.getLogger(__name__)
 
 
 class OpenAIEmbeddingProvider(EmbeddingProvider):
@@ -32,19 +32,20 @@
             )
 
         if provider != "openai":
             raise ValueError(
                 "OpenAIEmbeddingProvider must be initialized with provider `openai`."
             )
         if not os.getenv("OPENAI_API_KEY"):
-            raise ValueError(
-                "Must set OPENAI_API_KEY in order to initialize OpenAIEmbeddingProvider."
-            )
-        self.client = OpenAI()
-        self.async_client = AsyncOpenAI()
+            logger.warning("OPENAI_API_KEY not set. OpenAIEmbeddingProvider will not be used.")
+            self.client = None
+            self.async_client = None
+        else:
+            self.client = OpenAI()
+            self.async_client = AsyncOpenAI()
 
         if config.rerank_model:
             raise ValueError(
                 "OpenAIEmbeddingProvider does not support separate reranking."
             )
         self.search_model = config.search_model
         self.search_dimension = config.search_dimension
@@ -75,93 +76,111 @@
             )
 
     def get_embedding(
         self,
         text: str,
         stage: EmbeddingProvider.PipeStage = EmbeddingProvider.PipeStage.SEARCH,
     ) -> list[float]:
+        if not self.client:
+            raise ValueError("OpenAIEmbeddingProvider not initialized due to missing OPENAI_API_KEY.")
         if stage != EmbeddingProvider.PipeStage.SEARCH:
             raise ValueError(
                 "OpenAIEmbeddingProvider only supports search stage."
             )
-
-        return (
-            self.client.embeddings.create(
-                input=[text],
-                model=self.search_model,
-                dimensions=self.search_dimension
-                or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[
-                    self.search_model
-                ][-1],
+        
+        try:
+            return (
+                self.client.embeddings.create(
+                    input=[text],
+                    model=self.search_model,
+                    dimensions=self.search_dimension
+                    or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[
+                        self.search_model
+                    ][-1],
+                )
+                .data[0]
+                .embedding
             )
-            .data[0]
-            .embedding
-        )
+        except AuthenticationError as e:
+            raise ValueError("Invalid OpenAI API key provided. Please check your OPENAI_API_KEY environment variable.") from e
 
     async def async_get_embedding(
         self,
         text: str,
         stage: EmbeddingProvider.PipeStage = EmbeddingProvider.PipeStage.SEARCH,
     ) -> list[float]:
+        if not self.client:
+            raise ValueError("OpenAIEmbeddingProvider not initialized due to missing OPENAI_API_KEY.")
         if stage != EmbeddingProvider.PipeStage.SEARCH:
             raise ValueError(
                 "OpenAIEmbeddingProvider only supports search stage."
             )
 
-        response = await self.async_client.embeddings.create(
-            input=[text],
-            model=self.search_model,
-            dimensions=self.search_dimension
-            or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[self.search_model][
-                -1
-            ],
-        )
-        return response.data[0].embedding
+        try:
+            response = await self.async_client.embeddings.create(
+                input=[text],
+                model=self.search_model,
+                dimensions=self.search_dimension
+                or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[self.search_model][
+                    -1
+                ],
+            )
+            return response.data[0].embedding
+        except AuthenticationError as e:
+            raise ValueError("Invalid OpenAI API key provided. Please check your OPENAI_API_KEY environment variable.") from e
 
     def get_embeddings(
         self,
         texts: list[str],
         stage: EmbeddingProvider.PipeStage = EmbeddingProvider.PipeStage.SEARCH,
     ) -> list[list[float]]:
+        if not self.client:
+            raise ValueError("OpenAIEmbeddingProvider not initialized due to missing OPENAI_API_KEY.")
         if stage != EmbeddingProvider.PipeStage.SEARCH:
             raise ValueError(
                 "OpenAIEmbeddingProvider only supports search stage."
             )
 
-        return [
-            ele.embedding
-            for ele in self.client.embeddings.create(
-                input=texts,
-                model=self.search_model,
-                dimensions=self.search_dimension
-                or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[
-                    self.search_model
-                ][-1],
-            ).data
-        ]
+        try:
+            return [
+                ele.embedding
+                for ele in self.client.embeddings.create(
+                    input=texts,
+                    model=self.search_model,
+                    dimensions=self.search_dimension
+                    or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[
+                        self.search_model
+                    ][-1],
+                ).data
+            ]
+        except AuthenticationError as e:
+            raise ValueError("Invalid OpenAI API key provided. Please check your OPENAI_API_KEY environment variable.") from e
 
     async def async_get_embeddings(
         self,
         texts: list[str],
         stage: EmbeddingProvider.PipeStage = EmbeddingProvider.PipeStage.SEARCH,
     ) -> list[list[float]]:
         if stage != EmbeddingProvider.PipeStage.SEARCH:
             raise ValueError(
                 "OpenAIEmbeddingProvider only supports search stage."
             )
-
-        response = await self.async_client.embeddings.create(
-            input=texts,
-            model=self.search_model,
-            dimensions=self.search_dimension
-            or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[self.search_model][
-                -1
-            ],
-        )
-        return [ele.embedding for ele in response.data]
+        
+        try:
+            response = await self.async_client.embeddings.create(
+                input=texts,
+                model=self.search_model,
+                dimensions=self.search_dimension
+                or OpenAIEmbeddingProvider.MODEL_TO_DIMENSIONS[self.search_model][
+                    -1
+                ],
+            )
+            return [ele.embedding for ele in response.data]
+        except AuthenticationError as e:
+            raise ValueError("Invalid OpenAI API key provided. Please check your OPENAI_API_KEY environment variable.") from e
 
     def rerank(
         self,
         transformed_message: str,
         texts: list[SearchResult],
         stage: EmbeddingProvider.PipeStage = EmbeddingProvider.PipeStage.RERANK,
         limit: int = 10,
```

### Comparing `r2r-0.2.3/r2r/embeddings/setence_transformer/sentence_transformer_base.py` & `r2r-0.2.4/r2r/embeddings/setence_transformer/sentence_transformer_base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/eval/llm/base_llm_eval.py` & `r2r-0.2.4/r2r/eval/llm/base_llm_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from fractions import Fraction
-from typing import Optional, Union
+from typing import Union
 
 from r2r import (
     EvalConfig,
     EvalProvider,
     GenerationConfig,
     LLMProvider,
     PromptProvider,
```

### Comparing `r2r-0.2.3/r2r/examples/custom_rag.py` & `r2r-0.2.4/r2r/examples/custom_rag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """A custom RAG pipeline that includes a custom query transformation prompt."""
 
 from r2r import (
     GenerationConfig,
-    PipeLoggingConnectionSingleton,
+    KVLoggingSingleton,
     R2RConfig,
     R2RPipeFactory,
-    R2RProviderFactory,
     R2RPipelineFactory,
+    R2RProviderFactory,
     R2RQueryTransformPipe,
     RAGPipeline,
     run_pipeline,
 )
 
 if __name__ == "__main__":
     # Load the default configuration
     config = R2RConfig.from_json()
-    PipeLoggingConnectionSingleton().configure(config.logging)
+    KVLoggingSingleton().configure(config.logging)
 
     # Create input providers and pipes
     providers = R2RProviderFactory(config).create_providers()
     pipes = R2RPipeFactory(config, providers).create_pipes()
 
     # Add a custom prompt for transforming the user query
     transform_prompt = {
```

### Comparing `r2r-0.2.3/r2r/examples/data/aristotle.txt` & `r2r-0.2.4/r2r/examples/data/aristotle.txt`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/lyft_2021.pdf` & `r2r-0.2.4/r2r/examples/data/lyft_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/pg_essay_1.html` & `r2r-0.2.4/r2r/examples/data/pg_essay_1.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/pg_essay_2.html` & `r2r-0.2.4/r2r/examples/data/pg_essay_2.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/pg_essay_3.html` & `r2r-0.2.4/r2r/examples/data/pg_essay_3.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/pg_essay_4.html` & `r2r-0.2.4/r2r/examples/data/pg_essay_4.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/pg_essay_5.html` & `r2r-0.2.4/r2r/examples/data/pg_essay_5.html`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/screen_shot.png` & `r2r-0.2.4/r2r/examples/data/screen_shot.png`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/data/uber_2021.pdf` & `r2r-0.2.4/r2r/examples/data/uber_2021.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/examples/demo.py` & `r2r-0.2.4/r2r/examples/demo.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,17 @@
 
 import fire
 from fastapi.datastructures import UploadFile
 
 from r2r import (
     Document,
     GenerationConfig,
-    R2RApp,
+    R2RAppBuilder,
     R2RClient,
     R2RConfig,
-    R2RPipeFactory,
-    R2RPipelineFactory,
-    R2RProviderFactory,
     generate_id_from_label,
 )
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
@@ -31,48 +28,50 @@
 
     DEMO_USER_ID = "063edaf8-3e63-4cb9-a4d6-a855f36376c3"
 
     def __init__(
         self,
         config_path: Optional[str] = None,
         file_list: Optional[list[str]] = None,
+        file_tuples: Optional[list[tuple]] = None,
         user_id: str = DEMO_USER_ID,
         base_url: Optional[str] = None,
     ):
         if base_url:
             self.client = R2RClient(base_url)
         else:
             config = R2RConfig.from_json(config_path=config_path)
-
-            providers = R2RProviderFactory(config).create_providers()
-            pipes = R2RPipeFactory(config, providers).create_pipes()
-            pipelines = R2RPipelineFactory(config, pipes).create_pipelines()
-            self.r2r = R2RApp(config, providers, pipelines)
+            self.r2r = R2RAppBuilder(config).build()
 
         root_path = os.path.dirname(os.path.abspath(__file__))
         self.user_id = user_id
         self.default_files = file_list or [
-            os.path.join(root_path, "data", "screen_shot.png"),
             os.path.join(root_path, "data", "aristotle.txt"),
+            os.path.join(root_path, "data", "screen_shot.png"),
             os.path.join(root_path, "data", "pg_essay_1.html"),
             os.path.join(root_path, "data", "pg_essay_2.html"),
             os.path.join(root_path, "data", "pg_essay_3.html"),
             os.path.join(root_path, "data", "pg_essay_4.html"),
             os.path.join(root_path, "data", "pg_essay_5.html"),
             os.path.join(root_path, "data", "lyft_2021.pdf"),
             os.path.join(root_path, "data", "uber_2021.pdf"),
         ]
+        self.file_tuples = file_tuples or [
+            (
+                os.path.join(root_path, "data", "aristotle.txt"),
+                os.path.join(root_path, "data", "aristotle_v2.txt"),
+            )
+        ]
 
     def ingest_as_documents(self, file_paths: Optional[list[str]] = None):
         file_paths = file_paths or self.default_files
         documents = []
         for file_path in file_paths:
             with open(file_path, "rb") as f:
                 data = f.read()
-
             documents.append(
                 Document(
                     id=generate_id_from_label(file_path),
                     data=data,
                     type=file_path.split(".")[-1],
                     metadata={
                         "title": file_path.split(os.path.sep)[-1],
@@ -91,16 +90,56 @@
         else:
             t0 = time.time()
             response = self.r2r.ingest_documents(documents)
             t1 = time.time()
             print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
             print(response)
 
+    def update_as_documents(self, file_tuples: Optional[list[tuple]] = None):
+        file_tuples = file_tuples or self.file_tuples
+
+        documents = []
+        for old_file, new_file in file_tuples:
+            with open(new_file, "rb") as f:
+                data = f.read()
+
+            documents.append(
+                Document(
+                    id=generate_id_from_label(old_file),
+                    data=data,
+                    type=new_file.split(".")[-1],
+                    metadata={
+                        "title": old_file.split(os.path.sep)[-1],
+                        "user_id": self.user_id,
+                    },
+                )
+            )
+
+        if hasattr(self, "client"):
+            documents_dicts = [doc.dict() for doc in documents]
+            t0 = time.time()
+            response = self.client.update_documents(documents_dicts)
+            t1 = time.time()
+            print(f"Time taken to update documents: {t1-t0:.2f} seconds")
+            print(response)
+        else:
+            t0 = time.time()
+            response = self.r2r.update_documents(documents)
+            t1 = time.time()
+            print(f"Time taken to update documents: {t1-t0:.2f} seconds")
+            print(response)
+
     def ingest_as_files(self, file_paths: Optional[list[str]] = None):
         file_paths = file_paths or self.default_files
+
+        ids = [
+            generate_id_from_label(file_path.split(os.path.sep)[-1])
+            for file_path in file_paths
+        ]
+
         files = [
             UploadFile(
                 filename=file_path.split(os.path.sep)[-1],
                 file=open(file_path, "rb"),
             )
             for file_path in file_paths
         ]
@@ -118,22 +157,82 @@
             }
             for file_path in file_paths
         ]
 
         if hasattr(self, "client"):
             t0 = time.time()
             response = self.client.ingest_files(
-                metadatas=metadatas, files=file_paths
+                metadatas=metadatas, files=file_paths, ids=ids
             )
             t1 = time.time()
             print(f"Time taken to ingest files: {t1-t0:.2f} seconds")
             print(response)
         else:
             t0 = time.time()
-            response = self.r2r.ingest_files(files=files, metadatas=metadatas)
+            response = self.r2r.ingest_files(
+                files=files, metadatas=metadatas, ids=ids
+            )
+            t1 = time.time()
+            print("response = ", response)
+
+    def update_as_files(self, file_tuples: Optional[list[tuple]] = None):
+        file_tuples = file_tuples or self.file_tuples
+
+        new_files = [
+            UploadFile(
+                filename=new_file.split(os.path.sep)[-1],
+                file=open(new_file, "rb"),
+            )
+            for old_file, new_file in file_tuples
+        ]
+
+        # Set file size manually
+        for file in new_files:
+            file.file.seek(0, 2)  # Move to the end of the file
+            file.size = file.file.tell()  # Get the file size
+            file.file.seek(0)  # Move back to the start of the file
+
+        metadatas = [
+            {
+                "title": old_file.split(os.path.sep)[-1],
+                "user_id": self.user_id,
+            }
+            for old_file, new_file in file_tuples
+        ]
+
+        if hasattr(self, "client"):
+            t0 = time.time()
+            response = self.client.update_files(
+                metadatas=metadatas,
+                files=[new for old, new in file_tuples],
+                ids=[
+                    generate_id_from_label(old_file.split(os.path.sep)[-1])
+                    for old_file, new_file in file_tuples
+                ],
+            )
+            t1 = time.time()
+            print(f"Time taken to update files: {t1-t0:.2f} seconds")
+            print(response)
+        else:
+            t0 = time.time()
+            print(
+                "ids = ",
+                [
+                    generate_id_from_label(old_file.split(os.path.sep)[-1])
+                    for old_file, new_file in file_tuples
+                ],
+            )
+            response = self.r2r.update_files(
+                files=new_files,
+                metadatas=metadatas,
+                ids=[
+                    generate_id_from_label(old_file.split(os.path.sep)[-1])
+                    for old_file, new_file in file_tuples
+                ],
+            )
             t1 = time.time()
             print("response = ", response)
 
     def search(self, query: str):
         if hasattr(self, "client"):
             t0 = time.time()
             results = self.client.search(
@@ -267,26 +366,30 @@
             )
             t1 = time.time()
             print(f"Time taken to evaluate: {t1-t0:.2f} seconds")
             print(response)
 
     def delete(
         self,
-        key: str = "document_id",
-        value: str = "15255e98-e245-5b58-a57f-6c51babf72dd",
+        keys: list[str] = ["document_id"],
+        values: list[str] = ["c9bdbac7-0ea3-5c9e-b590-018bd09b127b"],
+        version: Optional[str] = None,
     ):
+        if version:
+            keys.append("version")
+            values.append(version)
         if hasattr(self, "client"):
             t0 = time.time()
-            response = self.client.delete(key, value)
+            response = self.client.delete(keys, values)
             t1 = time.time()
             print(f"Time taken to delete: {t1-t0:.2f} seconds")
             print(response)
         else:
             t0 = time.time()
-            response = self.r2r.delete(key, value)
+            response = self.r2r.delete(keys, values)
             t1 = time.time()
             print(f"Time taken to delete: {t1-t0:.2f} seconds")
             print(response)
 
     def get_user_ids(self):
         if hasattr(self, "client"):
             t0 = time.time()
@@ -297,28 +400,44 @@
         else:
             t0 = time.time()
             response = self.r2r.get_user_ids()
             t1 = time.time()
             print(f"Time taken to get user IDs: {t1-t0:.2f} seconds")
             print(response)
 
-    def get_user_document_data(self):
+    def get_user_documents_metadata(self):
         if hasattr(self, "client"):
             t0 = time.time()
-            response = self.client.get_user_document_data(self.user_id)
+            response = self.client.get_user_documents_metadata(self.user_id)
             t1 = time.time()
             print(f"Time taken to get user document data: {t1-t0:.2f} seconds")
             print(response)
         else:
             t0 = time.time()
-            response = self.r2r.get_user_document_data(self.user_id)
+            response = self.r2r.get_user_documents_metadata(self.user_id)
             t1 = time.time()
             print(f"Time taken to get user document data: {t1-t0:.2f} seconds")
             print(response)
 
+    def get_document_data(
+        self, document_id: str = "c9bdbac7-0ea3-5c9e-b590-018bd09b127b"
+    ):
+        if hasattr(self, "client"):
+            t0 = time.time()
+            response = self.client.get_document_data(document_id)
+            t1 = time.time()
+            print(f"Time taken to get document data: {t1-t0:.2f} seconds")
+            print(response)
+        else:
+            t0 = time.time()
+            response = self.r2r.get_document_data(document_id)
+            t1 = time.time()
+            print(f"Time taken to get document data: {t1-t0:.2f} seconds")
+            print(response)
+
     def get_logs(self, pipeline_type: Optional[str] = None):
         if hasattr(self, "client"):
             t0 = time.time()
             response = self.client.get_logs(pipeline_type)
             t1 = time.time()
             print(f"Time taken to get logs: {t1-t0:.2f} seconds")
             print(response)
```

### Comparing `r2r-0.2.3/r2r/examples/servers/configurable_pipeline.py` & `r2r-0.2.4/r2r/examples/servers/configurable_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/integrations/exa.py` & `r2r-0.2.4/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/integrations/ionic.py` & `r2r-0.2.4/r2r/integrations/ionic.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/integrations/serper.py` & `r2r-0.2.4/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/llms/litellm/base_litellm.py` & `r2r-0.2.4/r2r/llms/litellm/base_litellm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/llms/llama_cpp/base_llama_cpp.py` & `r2r-0.2.4/r2r/llms/llama_cpp/base_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/llms/openai/base_openai.py` & `r2r-0.2.4/r2r/llms/openai/base_openai.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/main/r2r_abstractions.py` & `r2r-0.2.4/r2r/main/r2r_abstractions.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/main/r2r_app.py` & `r2r-0.2.4/r2r/main/r2r_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import asyncio
 import json
 import logging
+import os
 import uuid
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from fastapi import Body, FastAPI, File, Form, HTTPException, UploadFile
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import StreamingResponse
+from pydantic import BaseModel
 
 from r2r.core import (
     Document,
     DocumentType,
     GenerationConfig,
-    PipeLoggingConnectionSingleton,
+    KVLoggingSingleton,
+    RunManager,
     generate_id_from_label,
     generate_run_id,
+    increment_version,
+    manage_run,
     to_async_generator,
 )
 from r2r.pipes import R2REvalPipe
 
 from .r2r_abstractions import R2RPipelines, R2RProviders
 from .r2r_config import R2RConfig
 
 MB_CONVERSION_FACTOR = 1024 * 1024
 
-from pydantic import BaseModel
-
 logger = logging.getLogger(__name__)
 
 
 def syncable(func):
     """Decorator to mark methods for synchronous wrapper creation."""
     func._syncable = True
     return func
@@ -73,18 +76,25 @@
                                     asyncio.set_event_loop(loop)
                                     result = loop.run_until_complete(
                                         async_method(self, *args, **kwargs)
                                     )
                                 except Exception as e:
                                     exception = e
                                 finally:
-                                    loop.run_until_complete(
-                                        loop.shutdown_asyncgens()
+                                    generation_config = kwargs.get(
+                                        "rag_generation_config", None
                                     )
-                                    loop.close()
+                                    if (
+                                        not generation_config
+                                        or not generation_config.stream
+                                    ):
+                                        loop.run_until_complete(
+                                            loop.shutdown_asyncgens()
+                                        )
+                                        loop.close()
 
                             thread = Thread(target=run)
                             thread.start()
                             thread.join()
                             if exception:
                                 raise exception
                             return result
@@ -122,125 +132,201 @@
     """
 
     def __init__(
         self,
         config: R2RConfig,
         providers: R2RProviders,
         pipelines: R2RPipelines,
+        run_manager: Optional[RunManager] = None,
         do_apply_cors: bool = True,
         *args,
         **kwargs,
     ):
         self.config = config
         self.providers = providers
-        self.logging_connection = PipeLoggingConnectionSingleton()
+        self.logging_connection = KVLoggingSingleton()
         self.ingestion_pipeline = pipelines.ingestion_pipeline
         self.search_pipeline = pipelines.search_pipeline
         self.rag_pipeline = pipelines.rag_pipeline
         self.streaming_rag_pipeline = pipelines.streaming_rag_pipeline
         self.eval_pipeline = pipelines.eval_pipeline
-
+        self.run_manager = run_manager or RunManager(self.logging_connection)
         self.app = FastAPI()
 
-        if do_apply_cors:
-            R2RApp._apply_cors(self.app)
-
         self._setup_routes()
+        if do_apply_cors:
+            self._apply_cors()
+        self._check_embedding_provider()
 
     def _setup_routes(self):
         self.app.add_api_route(
-            path="/ingest_documents/",
+            path="/ingest_documents",
             endpoint=self.ingest_documents_app,
             methods=["POST"],
         )
         self.app.add_api_route(
-            path="/ingest_files/",
+            path="/ingest_files",
             endpoint=self.ingest_files_app,
             methods=["POST"],
         )
         self.app.add_api_route(
-            path="/search/", endpoint=self.search_app, methods=["POST"]
+            path="/update_documents",
+            endpoint=self.update_documents_app,
+            methods=["POST"],
+        )
+        self.app.add_api_route(
+            path="/update_files",
+            endpoint=self.update_files_app,
+            methods=["POST"],
         )
         self.app.add_api_route(
-            path="/rag/", endpoint=self.rag_app, methods=["POST"]
+            path="/search", endpoint=self.search_app, methods=["POST"]
         )
         self.app.add_api_route(
-            path="/evaluate/",
+            path="/rag", endpoint=self.rag_app, methods=["POST"]
+        )
+        self.app.add_api_route(
+            path="/evaluate",
             endpoint=self.evaluate_app,
             methods=["POST"],
         )
         self.app.add_api_route(
-            path="/delete/", endpoint=self.delete_app, methods=["DELETE"]
+            path="/delete", endpoint=self.delete_app, methods=["DELETE"]
         )
         self.app.add_api_route(
-            path="/get_user_ids/",
+            path="/get_document_data",
+            endpoint=self.get_document_data_app,
+            methods=["GET"],
+        )
+        self.app.add_api_route(
+            path="/get_user_ids",
             endpoint=self.get_user_ids_app,
             methods=["GET"],
         )
         self.app.add_api_route(
-            path="/get_user_document_data/",
-            endpoint=self.get_user_document_data_app,
+            path="/get_user_documents_metadata",
+            endpoint=self.get_user_documents_metadata_app,
             methods=["POST"],
         )
         self.app.add_api_route(
-            path="/get_logs/",
+            path="/get_logs",
             endpoint=self.get_logs_app,
             methods=["POST"],
         )
 
         self.app.add_api_route(
-            path="/get_open_api_endpoint/",
+            path="/get_open_api_endpoint",
             endpoint=self.get_open_api_endpoint,
-            methods=["POST"],
+            methods=["GET"],
         )
-        # self.app.include_router(self.app.router)
 
     @syncable
-    async def aingest_documents(self, documents: list[Document]):
-        try:
-            # Process the documents through the pipeline
-            await self.ingestion_pipeline.run(
-                input=to_async_generator(documents)
-            )
-            return {"results": "Entries upserted successfully."}
-        except Exception as e:
-            logger.error(
-                f"ingest_documents(documents={documents}) - \n\n{str(e)})"
-            )
-            raise HTTPException(status_code=500, detail=str(e))
+    async def aingest_documents(
+        self,
+        documents: list[Document],
+        versions: Optional[list[str]] = None,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        # Process the documents through the pipeline
+        await self.ingestion_pipeline.run(
+            input=to_async_generator(documents),
+            versions=versions,
+            run_manager=self.run_manager,
+        )
+        return {"results": "Entries upserted successfully."}
 
     class IngestDocumentsRequest(BaseModel):
         documents: list[Document]
 
     async def ingest_documents_app(self, request: IngestDocumentsRequest):
-        try:
-            return await self.aingest_documents(request.documents)
-        except Exception as e:
-            run_id = self.ingestion_pipeline.run_id or generate_run_id()
-            await self.ingestion_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="pipeline_type",
-                value=self.ingestion_pipeline.pipeline_type,
-                is_pipeline_info=True,
+        async with manage_run(self.run_manager, "ingest_documents_app") as run_id:        
+            try:
+                return await self.aingest_documents(request.documents)
+            except Exception as e:
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.ingestion_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
+
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
+
+    @syncable
+    async def aupdate_documents(
+        self, documents: list[Document], *args: Any, **kwargs: Any
+    ):
+        if len(documents) == 0:
+            raise HTTPException(
+                status_code=400, detail="No documents provided for update."
             )
 
-            await self.ingestion_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="error",
-                value=str(e),
-                is_pipeline_info=False,
+        try:
+            old_versions = []
+            new_versions = []
+            for doc in documents:
+                document_data = await self.aget_document_data(doc.id)
+                current_version = document_data["results"][0]["version"]
+                old_versions.append(current_version)
+                new_versions.append(increment_version(current_version))
+
+            await self.aingest_documents(documents, versions=new_versions)
+
+            # Delete the old version
+            for doc, old_version in zip(documents, old_versions):
+                await self.adelete(
+                    ["document_id", "version"], [str(doc.id), old_version]
+                )
+
+            return {"results": f"Documents updated."}
+        except Exception as e:
+            logger.error(
+                f"update_documents(documents={documents}) - \n\n{str(e)})"
             )
             raise HTTPException(status_code=500, detail=str(e))
 
+    class UpdateDocumentsRequest(BaseModel):
+        documents: list[Document]
+
+    async def update_documents_app(self, request: UpdateDocumentsRequest):
+        async with manage_run(self.run_manager, "update_documents_app") as run_id:
+            try:
+                return await self.aupdate_documents(request.documents)
+            except Exception as e:
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.ingestion_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
+                
+
     @syncable
     async def aingest_files(
         self,
         files: list[UploadFile],
         metadatas: Optional[list[dict]] = None,
         ids: Optional[list[uuid.UUID]] = None,
+        versions: Optional[list[str]] = None,
+        *args: Any,
+        **kwargs: Any,
     ):
         if metadatas and len(metadatas) != len(files):
             raise HTTPException(
                 status_code=400,
                 detail="Number of metadata entries does not match number of files.",
             )
         if ids and len(ids) != len(files):
@@ -278,396 +364,544 @@
 
                 document_id = (
                     generate_id_from_label(file.filename)
                     if ids is None
                     else ids[iteration]
                 )
                 document_metadata = metadatas[iteration] if metadatas else {}
-
                 documents.append(
                     Document(
                         id=document_id,
                         type=DocumentType(file.filename.split(".")[-1]),
                         data=file_content,
                         metadata=document_metadata,
                     )
                 )
                 logger.info(f"Document created: {document_id}")
 
             # Run the pipeline asynchronously
-            logger.info("Running the ingestion pipeline...")
             await self.ingestion_pipeline.run(
                 input=to_async_generator(documents),
+                versions=versions,
+                run_manager=self.run_manager,
             )
-            logger.info("Ingestion pipeline completed.")
 
             return {
                 "results": [
                     f"File '{file.filename}' processed successfully."
                     for file in files
                 ]
             }
-        except Exception as e:
+        except ValueError as e:
             logger.error(
                 f"ingest_files(metadata={metadatas}, ids={ids}, files={files}) - \n\n{str(e)})"
-            )
+                )
+            raise HTTPException(status_code=401, detail=str(e))
+        except Exception as e:
+            logger.error(
+                f"ingest_files(metadata={metadatas}, ids={ids}, files={files}) - \n\n{str(e)}"
+                )
             raise HTTPException(status_code=500, detail=str(e))
         finally:
             # Ensure all file handles are closed
             for file in files:
                 file.file.close()
 
     async def ingest_files_app(
         self,
         files: list[UploadFile] = File(...),
         metadatas: Optional[str] = Form(None),
         ids: Optional[str] = Form(None),
     ):
         """Ingest files into the system."""
-        try:
-            if ids and ids != "null":
-                ids_list = json.loads(ids)
-                if len(ids_list) != 0:
-                    try:
-                        ids_list = [uuid.UUID(id) for id in ids_list]
-                    except ValueError:
-                        raise HTTPException(
-                            status_code=400, detail="Invalid UUID provided."
-                        )
-            else:
-                ids_list = None
-
-            # Parse metadatas if provided
-            metadatas = (
-                json.loads(metadatas)
-                if metadatas and metadatas != "null"
-                else None
-            )
-
-            # Call aingest_files with the correct order of arguments
-            return await self.aingest_files(
-                files=files, metadatas=metadatas, ids=ids_list
-            )
-        except Exception as e:
-            logger.error(f"ingest_files() - \n\n{str(e)})")
-            run_id = self.ingestion_pipeline.run_id or generate_run_id()
-            await self.ingestion_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="pipeline_type",
-                value=self.ingestion_pipeline.pipeline_type,
-                is_pipeline_info=True,
-            )
+        async with manage_run(self.run_manager, "ingest_files_app") as run_id:
+            try:
+                if ids and ids != "null":
+                    ids_list = json.loads(ids)
+                    if len(ids_list) != 0:
+                        try:
+                            ids_list = [uuid.UUID(id) for id in ids_list]
+                        except ValueError:
+                            raise HTTPException(
+                                status_code=400, detail="Invalid UUID provided."
+                            )
+                else:
+                    ids_list = None
+
+                # Parse metadatas if provided
+                metadatas = (
+                    json.loads(metadatas)
+                    if metadatas and metadatas != "null"
+                    else None
+                )
 
-            await self.ingestion_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="error",
-                value=str(e),
-                is_pipeline_info=False,
+                # Call aingest_files with the correct order of arguments
+                return await self.aingest_files(
+                    files=files, metadatas=metadatas, ids=ids_list
+                )
+            except Exception as e:
+                logger.error(f"ingest_files() - \n\n{str(e)})")
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.ingestion_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
+
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
+
+    @syncable
+    async def aupdate_files(
+        self,
+        files: list[UploadFile],
+        metadatas: Optional[list[dict]] = None,
+        ids: list[uuid.UUID] = None,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        if len(files) == 0:
+            raise HTTPException(
+                status_code=400, detail="No files provided for update."
             )
+
+        try:
+            # Parse ids if provided
+            if ids and len(ids) != len(files):
+                raise HTTPException(
+                    status_code=400,
+                    detail="Number of ids does not match number of files.",
+                )
+
+            # Ensure metadatas length matches files length
+            if metadatas and len(metadatas) != len(files):
+                raise HTTPException(
+                    status_code=400,
+                    detail="Number of metadata entries does not match number of files.",
+                )
+
+            # Get the current version
+            old_versions = []
+            new_versions = []
+            for id in ids:
+                document_data = await self.aget_document_data(id)
+                current_version = document_data["results"][0]["version"]
+                old_versions.append(current_version)
+                new_versions.append(increment_version(current_version))
+
+            # Update files with the new version
+            await self.aingest_files(
+                files, metadatas, ids, versions=new_versions
+            )
+
+            # Delete the old version
+            for id, old_version in zip(ids, old_versions):
+                await self.adelete(
+                    ["document_id", "version"], [str(id), old_version]
+                )
+
+            return {"results": f"Files updated."}
+        except Exception as e:
+            logger.error(f"update_files(files={files}) - \n\n{str(e)})")
             raise HTTPException(status_code=500, detail=str(e))
+        finally:
+            for file in files:
+                file.file.close()
+
+    class UpdateFilesRequest(BaseModel):
+        files: list[UploadFile] = File(...)
+        metadatas: Optional[str] = Form(None)
+        ids: str = Form("")
+
+    async def update_files_app(
+        self,
+        files: list[UploadFile] = File(...),
+        metadatas: Optional[str] = Form(None),
+        ids: Optional[str] = Form(None),
+    ):
+        async with manage_run(self.run_manager, "update_files_app") as run_id:
+            
+            try:
+                # Parse metadatas if provided
+                metadatas = (
+                    json.loads(metadatas)
+                    if metadatas and metadatas != "null"
+                    else None
+                )
+
+                # Parse ids if provided
+                ids_list = json.loads(ids)
+                if ids_list:
+                    ids_list = [uuid.UUID(id) for id in ids_list]
+                if len(ids_list) != len(files):
+                    raise HTTPException(
+                        status_code=400,
+                        detail="Number of ids does not match number of files.",
+                    )
+                if len(ids_list) != len(metadatas):
+                    raise HTTPException(
+                        status_code=400,
+                        detail="Number of metadata entries does not match number of files.",
+                    )
+                return await self.aupdate_files(
+                    files=files, metadatas=metadatas, ids=ids_list
+                )
+            except Exception as e:
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.ingestion_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
+
+                await self.ingestion_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )                
+                raise HTTPException(status_code=500, detail=str(e))
 
     @syncable
     async def asearch(
         self,
         query: str,
         search_filters: Optional[dict] = None,
         search_limit: int = 10,
+        *args: Any,
+        **kwargs: Any,
     ):
         """Search for documents based on the query."""
-        try:
-            search_filters = search_filters or {}
-            results = await self.search_pipeline.run(
-                input=to_async_generator([query]),
-                search_filters=search_filters,
-                search_limit=search_limit,
-            )
-            return {"results": [results.dict() for results in results]}
-        except Exception as e:
-            logger.error(f"search(query={query}) - \n\n{str(e)})")
-            raise HTTPException(status_code=500, detail=str(e))
+        search_filters = search_filters or {}
+        results = await self.search_pipeline.run(
+            input=to_async_generator([query]),
+            search_filters=search_filters,
+            search_limit=search_limit,
+            run_manager=self.run_manager,
+        )
+        return {"results": [results.dict() for results in results]}
 
     class SearchRequest(BaseModel):
         query: str
         search_filters: Optional[str] = None
         search_limit: int = 10
 
     async def search_app(self, request: SearchRequest):
-        try:
-            search_filters = (
-                {}
-                if request.search_filters is None
-                or request.search_filters == "null"
-                else json.loads(request.search_filters)
-            )
-            return await self.asearch(
-                request.query, search_filters, request.search_limit
-            )
-        except Exception as e:
-            # TODO - Make this more modular
-            run_id = self.search_pipeline.run_id or generate_run_id()
-            await self.search_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="pipeline_type",
-                value=self.search_pipeline.pipeline_type,
-                is_pipeline_info=True,
-            )
+        async with manage_run(self.run_manager, "search_app") as run_id:
+            try:
+                search_filters = (
+                    {}
+                    if request.search_filters is None
+                    or request.search_filters == "null"
+                    else json.loads(request.search_filters)
+                )
+                return await self.asearch(
+                    request.query, search_filters, request.search_limit
+                )
+            except Exception as e:
+                # TODO - Make this more modular
+                await self.search_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.search_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
 
-            await self.search_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="error",
-                value=str(e),
-                is_pipeline_info=False,
-            )
-            raise HTTPException(status_code=500, detail=str(e))
+                await self.search_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
 
     @syncable
     async def arag(
         self,
         message: str,
         rag_generation_config: GenerationConfig,
         search_filters: Optional[dict[str, str]] = None,
         search_limit: int = 10,
+        *args,
+        **kwargs,
     ):
-        try:
-            if rag_generation_config.stream:
-
-                async def stream_response():
+        if rag_generation_config.stream:
+            async def stream_response():
+                # We must re-enter the manage_run context for the streaming pipeline
+                async with manage_run(self.run_manager, "arag"):
                     async for chunk in await self.streaming_rag_pipeline.run(
                         input=to_async_generator([message]),
                         streaming=True,
                         search_filters=search_filters,
                         search_limit=search_limit,
                         rag_generation_config=rag_generation_config,
+                        run_manager=self.run_manager,
+                        *args,
+                        **kwargs,
                     ):
                         yield chunk
 
-                return stream_response()
+            return stream_response()
 
-            else:
-                results = await self.rag_pipeline.run(
-                    input=to_async_generator([message]),
-                    streaming=False,
-                    search_filters=search_filters,
-                    search_limit=search_limit,
-                    rag_generation_config=rag_generation_config,
-                )
-                return results
-        except Exception as e:
-            logger.error(f"rag(message={message}) - \n\n{str(e)})")
-            raise HTTPException(status_code=500, detail=str(e))
+        else:
+            results = await self.rag_pipeline.run(
+                input=to_async_generator([message]),
+                streaming=False,
+                search_filters=search_filters,
+                search_limit=search_limit,
+                rag_generation_config=rag_generation_config,
+                run_manager=self.run_manager,
+            )
+            return results
 
     class RAGRequest(BaseModel):
         message: str
         search_filters: Optional[str] = None
         search_limit: int = 10
         rag_generation_config: Optional[str] = None
         streaming: Optional[bool] = None
 
     async def rag_app(self, request: RAGRequest):
-        try:
-            search_filters = (
-                None
-                if request.search_filters is None
-                or request.search_filters == "null"
-                else json.loads(request.search_filters)
-            )
-            rag_generation_config = (
-                GenerationConfig(
-                    **json.loads(request.rag_generation_config),
-                    stream=request.streaming,
-                )
-                if request.rag_generation_config
-                and request.rag_generation_config != "null"
-                else GenerationConfig(
-                    model="gpt-3.5-turbo", stream=request.streaming
-                )
-            )
-            response = await self.arag(
-                request.message,
-                rag_generation_config,
-                search_filters,
-                request.search_limit,
-            )
-            if request.streaming:
-                return StreamingResponse(
-                    response, media_type="application/json"
+        async with manage_run(self.run_manager, "rag_app") as run_id:
+            try:
+                search_filters = (
+                    None
+                    if request.search_filters is None
+                    or request.search_filters == "null"
+                    else json.loads(request.search_filters)
                 )
-            else:
-                return {"results": response}
-
-        except Exception as e:
-            # TODO - Make this more modular
-            run_id = self.rag_pipeline.run_id or generate_run_id()
-            await self.rag_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="pipeline_type",
-                value=self.rag_pipeline.pipeline_type,
-                is_pipeline_info=True,
-            )
+                rag_generation_config = (
+                    GenerationConfig(
+                        **json.loads(request.rag_generation_config),
+                        stream=request.streaming,
+                    )
+                    if request.rag_generation_config
+                    and request.rag_generation_config != "null"
+                    else GenerationConfig(
+                        model="gpt-3.5-turbo", stream=request.streaming
+                    )
+                )
+                response = await self.arag(
+                    request.message,
+                    rag_generation_config,
+                    search_filters,
+                    request.search_limit,
+                )
+                if request.streaming:
+                    return StreamingResponse(
+                        response, media_type="application/json"
+                    )
+                else:
+                    return {"results": response}
 
-            await self.rag_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="error",
-                value=str(e),
-                is_pipeline_info=False,
-            )
-            raise HTTPException(status_code=500, detail=str(e))
+            except Exception as e:
+                # TODO - Modularize this, somehow
+                await self.rag_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.rag_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
+                await self.rag_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
 
     @syncable
     async def aevaluate(
         self,
         query: str,
         context: str,
         completion: str,
+        *args: Any,
+        **kwargs: Any,
     ):
-        try:
-            eval_payload = R2REvalPipe.EvalPayload(
-                query=query,
-                context=context,
-                completion=completion,
-            )
-            result = await self.eval_pipeline.run(
-                input=to_async_generator([eval_payload])
-            )
-            return {"results": result}
-        except Exception as e:
-            logger.error(f"evaluate(query={query}) - \n\n{str(e)})")
-            raise HTTPException(status_code=500, detail=str(e))
+        eval_payload = R2REvalPipe.EvalPayload(
+            query=query,
+            context=context,
+            completion=completion,
+        )
+        result = await self.eval_pipeline.run(
+            input=to_async_generator([eval_payload]),
+            run_manager=self.run_manager,
+        )
+        return {"results": result}
 
     class EvalRequest(BaseModel):
         query: str
         context: str
         completion: str
 
     async def evaluate_app(self, request: EvalRequest):
-        try:
-            return await self.aevaluate(
-                query=request.query,
-                context=request.context,
-                completion=request.completion,
-            )
-        except Exception as e:
-            run_id = self.eval_pipeline.run_id or generate_run_id()
-            await self.eval_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="pipeline_type",
-                value=self.eval_pipeline.pipeline_type,
-                is_pipeline_info=True,
-            )
+        async with manage_run(self.run_manager, "evaluate_app") as run_id:
+            try:
+                return await self.aevaluate(
+                    query=request.query,
+                    context=request.context,
+                    completion=request.completion,
+                )
+            except Exception as e:
+                await self.eval_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="pipeline_type",
+                    value=self.eval_pipeline.pipeline_type,
+                    is_info_log=True,
+                )
 
-            await self.eval_pipeline.pipe_logger.log(
-                pipe_run_id=run_id,
-                key="error",
-                value=str(e),
-                is_pipeline_info=False,
-            )
-            raise HTTPException(status_code=500, detail=str(e))
+                await self.eval_pipeline.pipe_logger.log(
+                    log_id=run_id,
+                    key="error",
+                    value=str(e),
+                    is_info_log=False,
+                )
+                raise HTTPException(status_code=500, detail=str(e))
 
     @syncable
-    async def adelete(self, key: str, value: Union[bool, int, str]):
+    async def adelete(
+        self,
+        keys: list[str],
+        values: list[Union[bool, int, str]],
+        *args: Any,
+        **kwargs: Any,
+    ):
+        self.providers.vector_db.delete_by_metadata(keys, values)
+        return {"results": "Entries deleted successfully."}
+
+    class DeleteRequest(BaseModel):
+        keys: list[str]
+        values: list[Union[bool, int, str]]
+
+    async def delete_app(self, request: DeleteRequest = Body(...)):
         try:
-            self.providers.vector_db.delete_by_metadata(key, value)
-            return {"results": "Entries deleted successfully."}
+            return await self.adelete(request.keys, request.values)
         except Exception as e:
             logger.error(
-                f":delete: [Error](key={key}, value={value}, error={str(e)})"
+                f":delete: [Error](key={request.keys}, value={request.values}, error={str(e)})"
             )
             raise HTTPException(status_code=500, detail=str(e))
 
-    class DeleteRequest(BaseModel):
-        key: str
-        value: Union[bool, int, str]
+    @syncable
+    async def aget_user_ids(self, *args: Any, **kwargs: Any):
+        user_ids = self.providers.vector_db.get_metadatas(
+            metadata_fields=["user_id"]
+        )
 
-    async def delete_app(self, request: DeleteRequest = Body(...)):
-        return await self.adelete(request.key, request.value)
+        return {"results": [ele["user_id"] for ele in user_ids]}
 
-    @syncable
-    async def aget_user_ids(self):
+    async def get_user_ids_app(self):
         try:
-            user_ids = self.providers.vector_db.get_metadatas(
-                metadata_fields=["user_id"]
-            )
-
-            return {"results": [ele["user_id"] for ele in user_ids]}
+            return await self.aget_user_ids()
         except Exception as e:
             logger.error(f"get_user_ids() - \n\n{str(e)})")
             raise HTTPException(status_code=500, detail=str(e))
 
-    async def get_user_ids_app(self):
-        return await self.aget_user_ids()
-
     @syncable
-    async def aget_user_document_data(self, user_id: str):
+    async def aget_user_documents_metadata(
+        self, user_id: str, *args: Any, **kwargs: Any
+    ):
+        if isinstance(user_id, uuid.UUID):
+            user_id = str(user_id)
+        document_ids = self.providers.vector_db.get_metadatas(
+            metadata_fields=["document_id", "title"],
+            filter_field="user_id",
+            filter_value=user_id,
+        )
+        return {"results": [ele for ele in document_ids]}
+
+    class UserDocumentRequest(BaseModel):
+        user_id: str
+
+    async def get_user_documents_metadata_app(
+        self, request: UserDocumentRequest
+    ):
         try:
-            if isinstance(user_id, uuid.UUID):
-                user_id = str(user_id)
-            document_ids = self.providers.vector_db.get_metadatas(
-                metadata_fields=["document_id", "title"],
-                filter_field="user_id",
-                filter_value=user_id,
-            )
-            return {"results": [ele for ele in document_ids]}
+            return await self.aget_user_documents_metadata(request.user_id)
         except Exception as e:
             logger.error(
-                f"get_user_document_data(user_id={user_id}) - \n\n{str(e)})"
+                f"get_user_documents_metadata(user_id={request.user_id}) - \n\n{str(e)})"
             )
             raise HTTPException(status_code=500, detail=str(e))
 
-    class UserDocumentRequest(BaseModel):
-        user_id: str
-
-    async def get_user_document_data_app(self, request: UserDocumentRequest):
-        return await self.aget_user_document_data(request.user_id)
-
     @syncable
-    async def aget_logs(self, pipeline_type: Optional[str] = None):
-        try:
-            logs_per_run = 10
-            if self.logging_connection is None:
-                raise HTTPException(
-                    status_code=404, detail="Logging provider not found."
-                )
-            run_info = await self.logging_connection.get_run_info(
-                pipeline_type=pipeline_type,
-                limit=self.config.app.get("max_logs", 100) // logs_per_run,
-            )
-            run_ids = [run.run_id for run in run_info]
-            if len(run_ids) == 0:
-                return {"results": []}
-            logs = await self.logging_connection.get_logs(run_ids)
-            # Aggregate logs by run_id and include run_type
-            aggregated_logs = []
-
-            for run in run_info:
-                run_logs = [
-                    log for log in logs if log["pipe_run_id"] == run.run_id
-                ]
-                entries = [
-                    {"key": log["key"], "value": log["value"]}
-                    for log in run_logs
-                ]
-                aggregated_logs.append(
-                    {
-                        "run_id": run.run_id,
-                        "run_type": run.pipeline_type,
-                        "entries": entries,
-                    }
-                )
+    async def aget_document_data(
+        self, document_id: str, *args: Any, **kwargs: Any
+    ):
+        if isinstance(document_id, uuid.UUID):
+            document_id = str(document_id)
+        document_ids = self.providers.vector_db.get_metadatas(
+            metadata_fields=["document_id", "title", "version"],
+            filter_field="document_id",
+            filter_value=document_id,
+        )
+        return {"results": [ele for ele in document_ids]}
 
-            return {"results": aggregated_logs}
+    class DocumentDataRequest(BaseModel):
+        document_id: str
 
+    async def get_document_data_app(self, request: DocumentDataRequest):
+        try:
+            return await self.aget_document_data_app(request.document_id)
         except Exception as e:
-            logger.error(f":logs: [Error](error={str(e)})")
+            logger.error(
+                f"get_document_data(document_id={request.document_id}) - \n\n{str(e)})"
+            )
             raise HTTPException(status_code=500, detail=str(e))
 
+    @syncable
+    async def aget_logs(
+        self, log_type_filter: Optional[str] = None, *args: Any, **kwargs: Any
+    ):
+        logs_per_run = 10
+        if self.logging_connection is None:
+            raise HTTPException(
+                status_code=404, detail="Logging provider not found."
+            )
+        run_info = await self.logging_connection.get_run_info(
+            limit=self.config.app.get("max_logs", 100) // logs_per_run,
+            log_type_filter=log_type_filter,
+        )
+        run_ids = [run.run_id for run in run_info]
+        if len(run_ids) == 0:
+            return {"results": []}
+        logs = await self.logging_connection.get_logs(run_ids)
+        # Aggregate logs by run_id and include run_type
+        aggregated_logs = []
+
+        for run in run_info:
+            run_logs = [log for log in logs if log["log_id"] == run.run_id]
+            entries = [
+                {"key": log["key"], "value": log["value"]} for log in run_logs
+            ]
+            aggregated_logs.append(
+                {
+                    "run_id": run.run_id,
+                    "run_type": run.log_type,
+                    "entries": entries,
+                }
+            )
+
+        return {"results": aggregated_logs}
+
     class LogsRequest(BaseModel):
-        pipeline_type: Optional[str] = None
+        log_type_filter: Optional[str] = None
 
     async def get_logs_app(self, request: LogsRequest):
-        return await self.aget_logs(request.pipeline_type)
+        try:
+            return await self.aget_logs(request.log_type_filter)
+        except Exception as e:
+            logger.error(f":logs: [Error](error={str(e)})")
+            raise HTTPException(status_code=500, detail=str(e))
 
     def get_open_api_endpoint(self):
         from fastapi.openapi.utils import get_openapi
 
         return {
             "results": get_openapi(
                 title="R2R Application API",
@@ -682,23 +916,27 @@
         except ImportError:
             raise ImportError(
                 "Please install uvicorn using 'pip install uvicorn'"
             )
 
         uvicorn.run(self.app, host=host, port=port)
 
-    @staticmethod
-    def _apply_cors(app):
+    def _apply_cors(self):
         # CORS setup
         origins = [
             "*",  # TODO - Change this to the actual frontend URL
             "http://localhost:3000",
             "http://localhost:8000",
         ]
 
-        app.add_middleware(
+        self.app.add_middleware(
             CORSMiddleware,
             allow_origins=origins,  # Allows specified origins
             allow_credentials=True,
             allow_methods=["*"],  # Allows all methods
             allow_headers=["*"],  # Allows all headers
         )
+
+    def _check_embedding_provider(self):
+        if self.config.embedding.provider == "openai" and not os.getenv("OPENAI_API_KEY"):
+            logger.warning("OpenAI API key not found. Embedding provider will not be used.")
+            raise ValueError("OpenAI API key not found. Please set the OPENAI_API_KEY environment variable.")
```

### Comparing `r2r-0.2.3/r2r/main/r2r_client.py` & `r2r-0.2.4/r2r/main/r2r_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,117 @@
 """Module for the R2RClient class."""
 
 import asyncio
 import json
+import uuid
 from typing import AsyncGenerator, Generator, Optional, Union
 
 import httpx
 import nest_asyncio
 import requests
 
+from r2r.core import DocumentType
+
 nest_asyncio.apply()
 
 
+def default_serializer(obj):
+    if isinstance(obj, uuid.UUID):
+        return str(obj)
+    if isinstance(obj, DocumentType):
+        return obj.value
+    if isinstance(obj, bytes):
+        # return base64.b64encode(obj).decode('utf-8')
+        raise TypeError("Bytes serialization is not yet supported.")
+    raise TypeError(f"Type {type(obj)} not serializable.")
+
+
 class R2RClient:
     def __init__(self, base_url: str):
         self.base_url = base_url
 
     def ingest_documents(self, documents: list[dict]) -> dict:
-        url = f"{self.base_url}/ingest_documents/"
+        url = f"{self.base_url}/ingest_documents"
         data = {"documents": documents}
-        response = requests.post(url, json=data)
+        serialized_data = json.dumps(data, default=default_serializer)
+        response = requests.post(
+            url,
+            data=serialized_data,
+            headers={"Content-Type": "application/json"},
+        )
+
         response.raise_for_status()
         return response.json()
 
     def ingest_files(
         self,
-        metadatas: list[dict],
+        metadatas: Optional[list[dict]],
         files: list[str],
         ids: Optional[list[str]] = None,
     ) -> dict:
-        url = f"{self.base_url}/ingest_files/"
+        url = f"{self.base_url}/ingest_files"
         files_to_upload = [
             ("files", (file, open(file, "rb"), "application/octet-stream"))
             for file in files
         ]
         data = {
-            "metadatas": None if not metadatas else json.dumps(metadatas),
-            "ids": None if not ids else json.dumps(ids),
+            "metadatas": None
+            if metadatas is None
+            else json.dumps(metadatas, default=default_serializer),
+            "ids": None
+            if ids is None
+            else json.dumps(ids, default=default_serializer),
+        }
+        response = requests.post(url, files=files_to_upload, data=data)
+        response.raise_for_status()
+        return response.json()
+
+    def update_documents(self, documents: list[dict]) -> dict:
+        url = f"{self.base_url}/update_documents"
+        data = {"documents": documents}
+        serialized_data = json.dumps(data, default=default_serializer)
+        response = requests.post(
+            url,
+            data=serialized_data,
+            headers={"Content-Type": "application/json"},
+        )
+        response.raise_for_status()
+        return response.json()
+
+    def update_files(
+        self,
+        metadatas: Optional[list[dict]],
+        files: list[str],
+        ids: list[str],
+    ) -> dict:
+        url = f"{self.base_url}/update_files"
+        files_to_upload = [
+            ("files", (file, open(file, "rb"), "application/octet-stream"))
+            for file in files
+        ]
+        data = {
+            "metadatas": None
+            if metadatas is None
+            else json.dumps(metadatas, default=default_serializer),
+            "ids": json.dumps(ids, default=default_serializer),
         }
         response = requests.post(url, files=files_to_upload, data=data)
         response.raise_for_status()
         return response.json()
 
     def search(
-        self, query: str, search_filters: dict = {}, search_limit: int = 10
+        self,
+        query: str,
+        search_filters: Optional[dict] = None,
+        search_limit: int = 10,
     ) -> dict:
-        url = f"{self.base_url}/search/"
+        url = f"{self.base_url}/search"
         data = {
             "query": query,
-            "search_filters": json.dumps(search_filters),
+            "search_filters": json.dumps(search_filters or {}),
             "search_limit": search_limit,
         }
         response = requests.post(url, json=data)
         response.raise_for_status()
         return response.json()
 
     def rag(
@@ -66,45 +126,49 @@
             return self._stream_rag_sync(
                 message=message,
                 search_filters=search_filters,
                 search_limit=search_limit,
                 rag_generation_config=rag_generation_config,
             )
         else:
-            url = f"{self.base_url}/rag/"
+            url = f"{self.base_url}/rag"
             data = {
                 "message": message,
-                "search_filters": json.dumps(search_filters or {}),
+                "search_filters": json.dumps(search_filters)
+                if search_filters
+                else None,
                 "search_limit": search_limit,
+                "rag_generation_config": json.dumps(rag_generation_config)
+                if rag_generation_config
+                else None,
                 "streaming": streaming,
             }
-            if rag_generation_config:
-                data["rag_generation_config"] = json.dumps(
-                    rag_generation_config
-                )
             response = requests.post(url, json=data)
             response.raise_for_status()
             return response.json()
 
     async def _stream_rag(
         self,
         message: str,
         search_filters: Optional[dict] = None,
         search_limit: int = 10,
         rag_generation_config: Optional[dict] = None,
-    ) -> Generator[str, None, None]:
-        url = f"{self.base_url}/rag/"
+    ) -> AsyncGenerator[str, None]:
+        url = f"{self.base_url}/rag"
         data = {
             "message": message,
-            "search_filters": json.dumps(search_filters or {}),
+            "search_filters": json.dumps(search_filters)
+            if search_filters
+            else None,
             "search_limit": search_limit,
+            "rag_generation_config": json.dumps(rag_generation_config)
+            if rag_generation_config
+            else None,
             "streaming": True,
         }
-        if rag_generation_config:
-            data["rag_generation_config"] = json.dumps(rag_generation_config)
         async with httpx.AsyncClient() as client:
             async with client.stream("POST", url, json=data) as response:
                 response.raise_for_status()
                 async for chunk in response.aiter_text():
                     yield chunk
 
     def _stream_rag_sync(
@@ -131,36 +195,42 @@
         self, async_gen: AsyncGenerator[str, None]
     ) -> list[str]:
         chunks = []
         async for chunk in async_gen:
             chunks.append(chunk)
         return chunks
 
-    def delete(self, key: str, value: str) -> dict:
-        url = f"{self.base_url}/delete/"
-        data = {"key": key, "value": value}
+    def delete(
+        self, keys: list[str], values: list[Union[bool, int, str]]
+    ) -> dict:
+        url = f"{self.base_url}/delete"
+        data = {"keys": keys, "values": values}
         response = requests.request("DELETE", url, json=data)
         response.raise_for_status()
         return response.json()
 
     def get_user_ids(self) -> dict:
-        url = f"{self.base_url}/get_user_ids/"
+        url = f"{self.base_url}/get_user_ids"
         response = requests.get(url)
         response.raise_for_status()
         return response.json()
 
-    def get_user_document_data(self, user_id: str) -> dict:
-        url = f"{self.base_url}/get_user_document_data/"
+    def get_user_documents_metadata(self, user_id: str) -> dict:
+        url = f"{self.base_url}/get_user_documents_metadata"
         data = {"user_id": user_id}
         response = requests.post(url, json=data)
         response.raise_for_status()
-        response_json = response.json()
-        return response_json
+        return response.json()
 
-    def get_logs(
-        self, pipeline_type: Optional[str] = None, filter: Optional[str] = None
-    ) -> dict:
-        url = f"{self.base_url}/get_logs/"
-        data = {"pipeline_type": pipeline_type, "filter": filter}
+    def get_document_data(self, document_id: str) -> dict:
+        url = f"{self.base_url}/get_document_data"
+        data = {"document_id": document_id}
+        response = requests.post(url, json=data)
+        response.raise_for_status()
+        return response.json()
+
+    def get_logs(self, log_type_filter: Optional[str] = None) -> dict:
+        url = f"{self.base_url}/get_logs"
+        data = {"log_type_filter": log_type_filter}
         response = requests.post(url, json=data)
         response.raise_for_status()
         return response.json()
```

### Comparing `r2r-0.2.3/r2r/main/r2r_config.py` & `r2r-0.2.4/r2r/main/r2r_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import json
 import logging
 import os
-from typing import Any
+from enum import Enum
+from typing import Any, Type
+
+from pydantic import BaseModel
 
 from ..core.abstractions.document import DocumentType
-from ..core.pipes.pipe_logging import LoggingConfig
+from ..core.logging.kv_logger import LoggingConfig
 from ..core.providers.embedding_provider import EmbeddingConfig
 from ..core.providers.eval_provider import EvalConfig
 from ..core.providers.llm_provider import LLMConfig
 from ..core.providers.prompt_provider import PromptConfig
-from ..core.providers.vector_db_provider import VectorDBConfig
+from ..core.providers.vector_db_provider import ProviderConfig, VectorDBConfig
 
 logger = logging.getLogger(__name__)
 
 
 class R2RConfig:
     REQUIRED_KEYS: dict[str, list] = {
-        "app": [
-            "max_file_size_in_mb",
-        ],
+        "app": ["max_file_size_in_mb"],
         "embedding": [
             "provider",
             "search_model",
             "search_dimension",
             "batch_size",
             "text_splitter",
         ],
-        "eval": [
-            "llm",
-        ],
+        "eval": ["llm"],
         "ingestion": ["selected_parsers"],
         "completions": ["provider"],
         "logging": ["provider", "log_table"],
         "prompt": ["provider"],
         "vector_database": ["provider", "collection_name"],
     }
     app: dict[str, Any]
@@ -93,32 +92,54 @@
 
         # Load configuration from JSON file
         with open(config_path) as f:
             config_data = json.load(f)
 
         return cls(config_data)
 
-    # TODO - How to type 'redis.Redis' without introducing dependency on 'redis' package?
     def save_to_redis(self, redis_client: Any, key: str):
         config_data = {
-            section: getattr(self, section)
+            section: self._serialize_config(getattr(self, section))
             for section in R2RConfig.REQUIRED_KEYS.keys()
         }
         redis_client.set(f"R2RConfig:{key}", json.dumps(config_data))
 
     @classmethod
     def load_from_redis(cls, redis_client: Any, key: str) -> "R2RConfig":
         config_data = redis_client.get(f"R2RConfig:{key}")
         if config_data is None:
             raise ValueError(
                 f"Configuration not found in Redis with key '{key}'"
             )
-        return cls(json.loads(config_data))
+        config_data = json.loads(config_data)
+        # config_data["ingestion"]["selected_parsers"] = {
+        #     DocumentType(k): v
+        #     for k, v in config_data["ingestion"]["selected_parsers"].items()
+        # }
+        return cls(config_data)
 
     @classmethod
     def load_default_config(cls) -> dict:
         # Get the root directory of the project
         file_dir = os.path.dirname(os.path.abspath(__file__))
         default_config_path = os.path.join(file_dir, "..", "..", "config.json")
         # Load default configuration from JSON file
         with open(default_config_path) as f:
             return json.load(f)
+
+    @staticmethod
+    def _serialize_config(config_section: Any) -> dict:
+        # TODO - Make this approach cleaner
+        if isinstance(config_section, ProviderConfig):
+            config_section = config_section.dict()
+        filtered_result = {}
+        for k, v in config_section.items():
+            if isinstance(k, Enum):
+                k = k.value
+            if isinstance(v, dict):
+                formatted_v = {
+                    k2.value if isinstance(k2, Enum) else k2: v2
+                    for k2, v2 in v.items()
+                }
+                v = formatted_v
+            filtered_result[k] = v
+        return filtered_result
```

### Comparing `r2r-0.2.3/r2r/main/r2r_factory.py` & `r2r-0.2.4/r2r/main/r2r_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 from r2r.core import (
     EmbeddingConfig,
     EmbeddingProvider,
     EvalPipeline,
     EvalProvider,
     IngestionPipeline,
+    KVLoggingSingleton,
     LLMConfig,
     LLMProvider,
-    PipeLoggingConnectionSingleton,
+    LoggableAsyncPipe,
     PromptProvider,
     RAGPipeline,
     SearchPipeline,
     VectorDBConfig,
     VectorDBProvider,
 )
 
@@ -144,56 +145,99 @@
             prompt_provider = R2RPromptProvider()
         else:
             raise ValueError(
                 f"Prompt provider {prompt_config.provider} not supported"
             )
         return prompt_provider
 
-    def create_providers(self) -> R2RProviders:
-        llm_provider = self.create_llm_provider(self.config.completions)
-        prompt_provider = self.create_prompt_provider(self.config.prompt)
+    def create_providers(
+        self,
+        vector_db_provider_override: Optional[VectorDBProvider] = None,
+        embedding_provider_override: Optional[EmbeddingProvider] = None,
+        eval_provider_override: Optional[EvalProvider] = None,
+        llm_provider_override: Optional[LLMProvider] = None,
+        prompt_provider_override: Optional[PromptProvider] = None,
+        *args,
+        **kwargs,
+    ) -> R2RProviders:
+        prompt_provider = (
+            prompt_provider_override
+            or self.create_prompt_provider(self.config.prompt, *args, **kwargs)
+        )
         return R2RProviders(
-            vector_db=self.create_vector_db_provider(
-                self.config.vector_database
+            vector_db=vector_db_provider_override
+            or self.create_vector_db_provider(
+                self.config.vector_database, *args, **kwargs
             ),
-            embedding=self.create_embedding_provider(self.config.embedding),
-            eval=self.create_eval_provider(
-                self.config.eval, prompt_provider=prompt_provider
+            embedding=embedding_provider_override
+            or self.create_embedding_provider(
+                self.config.embedding, *args, **kwargs
+            ),
+            eval=eval_provider_override
+            or self.create_eval_provider(
+                self.config.eval,
+                prompt_provider=prompt_provider,
+                *args,
+                **kwargs,
+            ),
+            llm=llm_provider_override
+            or self.create_llm_provider(
+                self.config.completions, *args, **kwargs
+            ),
+            prompt=prompt_provider_override
+            or self.create_prompt_provider(
+                self.config.prompt, *args, **kwargs
             ),
-            llm=llm_provider,
-            prompt=prompt_provider,
         )
 
 
 class R2RPipeFactory:
     def __init__(self, config: R2RConfig, providers: R2RProviders):
         self.config = config
         self.providers = providers
 
-    def create_pipes(self) -> R2RPipes:
+    def create_pipes(
+        self,
+        parsing_pipe_override: Optional[LoggableAsyncPipe] = None,
+        embedding_pipe_override: Optional[LoggableAsyncPipe] = None,
+        vector_storage_pipe_override: Optional[LoggableAsyncPipe] = None,
+        search_pipe_override: Optional[LoggableAsyncPipe] = None,
+        rag_pipe_override: Optional[LoggableAsyncPipe] = None,
+        streaming_rag_pipe_override: Optional[LoggableAsyncPipe] = None,
+        eval_pipe_override: Optional[LoggableAsyncPipe] = None,
+        *args: Any,
+        **kwargs: Any,
+    ) -> R2RPipes:
         return R2RPipes(
-            parsing_pipe=self.create_parsing_pipe(
-                self.config.ingestion.get("selected_parsers")
+            parsing_pipe=parsing_pipe_override
+            or self.create_parsing_pipe(
+                self.config.ingestion.get("selected_parsers"), *args, **kwargs
             ),
-            embedding_pipe=self.create_embedding_pipe(),
-            vector_storage_pipe=self.create_vector_storage_pipe(),
-            search_pipe=self.create_search_pipe(),
-            rag_pipe=self.create_rag_pipe(),
-            streaming_rag_pipe=self.create_rag_pipe(streaming=True),
-            eval_pipe=self.create_eval_pipe(),
+            embedding_pipe=embedding_pipe_override
+            or self.create_embedding_pipe(*args, **kwargs),
+            vector_storage_pipe=vector_storage_pipe_override
+            or self.create_vector_storage_pipe(*args, **kwargs),
+            search_pipe=search_pipe_override
+            or self.create_search_pipe(*args, **kwargs),
+            rag_pipe=rag_pipe_override
+            or self.create_rag_pipe(*args, **kwargs),
+            streaming_rag_pipe=streaming_rag_pipe_override
+            or self.create_rag_pipe(streaming=True),
+            eval_pipe=eval_pipe_override
+            or self.create_eval_pipe(*args, **kwargs),
         )
 
     def create_parsing_pipe(
-        self, selected_parsers: Optional[dict] = None
+        self, selected_parsers: Optional[dict] = None, *args, **kwargs
     ) -> Any:
         from r2r.pipes import R2RDocumentParsingPipe
 
         return R2RDocumentParsingPipe(selected_parsers=selected_parsers or {})
 
-    def create_embedding_pipe(self) -> Any:
+    def create_embedding_pipe(self, *args, **kwargs) -> Any:
         from r2r.core import RecursiveCharacterTextSplitter
         from r2r.pipes import R2REmbeddingPipe
 
         text_splitter_config = self.config.embedding.extra_fields.get(
             "text_splitter"
         )
         if not text_splitter_config:
@@ -210,30 +254,30 @@
         return R2REmbeddingPipe(
             embedding_provider=self.providers.embedding,
             vector_db_provider=self.providers.vector_db,
             text_splitter=text_splitter,
             embedding_batch_size=self.config.embedding.batch_size,
         )
 
-    def create_vector_storage_pipe(self) -> Any:
+    def create_vector_storage_pipe(self, *args, **kwargs) -> Any:
         from r2r.pipes import R2RVectorStoragePipe
 
         return R2RVectorStoragePipe(
             vector_db_provider=self.providers.vector_db
         )
 
-    def create_search_pipe(self) -> Any:
+    def create_search_pipe(self, *args, **kwargs) -> Any:
         from r2r.pipes import R2RVectorSearchPipe
 
         return R2RVectorSearchPipe(
             vector_db_provider=self.providers.vector_db,
             embedding_provider=self.providers.embedding,
         )
 
-    def create_rag_pipe(self, streaming: bool = False) -> Any:
+    def create_rag_pipe(self, streaming: bool = False, *args, **kwargs) -> Any:
         if streaming:
             from r2r.pipes import R2RStreamingRAGPipe
 
             return R2RStreamingRAGPipe(
                 llm_provider=self.providers.llm,
                 prompt_provider=self.providers.prompt,
             )
@@ -241,38 +285,40 @@
             from r2r.pipes import R2RRAGPipe
 
             return R2RRAGPipe(
                 llm_provider=self.providers.llm,
                 prompt_provider=self.providers.prompt,
             )
 
-    def create_eval_pipe(self) -> Any:
+    def create_eval_pipe(self, *args, **kwargs) -> Any:
         from r2r.pipes import R2REvalPipe
 
         return R2REvalPipe(eval_provider=self.providers.eval)
 
 
 class R2RPipelineFactory:
     def __init__(self, config: R2RConfig, pipes: R2RPipes):
         self.config = config
         self.pipes = pipes
 
-    def create_ingestion_pipeline(self) -> IngestionPipeline:
+    def create_ingestion_pipeline(self, *args, **kwargs) -> IngestionPipeline:
         ingestion_pipeline = IngestionPipeline()
         ingestion_pipeline.add_pipe(self.pipes.parsing_pipe)
         ingestion_pipeline.add_pipe(self.pipes.embedding_pipe)
         ingestion_pipeline.add_pipe(self.pipes.vector_storage_pipe)
         return ingestion_pipeline
 
-    def create_search_pipeline(self) -> SearchPipeline:
+    def create_search_pipeline(self, *args, **kwargs) -> SearchPipeline:
         search_pipeline = SearchPipeline()
         search_pipeline.add_pipe(self.pipes.search_pipe)
         return search_pipeline
 
-    def create_rag_pipeline(self, streaming: bool = False) -> RAGPipeline:
+    def create_rag_pipeline(
+        self, streaming: bool = False, *args, **kwargs
+    ) -> RAGPipeline:
         search_pipe = self.pipes.search_pipe
         rag_pipe = (
             self.pipes.streaming_rag_pipe if streaming else self.pipes.rag_pipe
         )
 
         rag_pipeline = RAGPipeline()
         rag_pipeline.add_pipe(search_pipe)
@@ -289,38 +335,42 @@
                     "prev_output_field": "search_queries",
                     "input_field": "query",
                 },
             ],
         )
         return rag_pipeline
 
-    def create_eval_pipeline(self) -> EvalPipeline:
+    def create_eval_pipeline(self, *args, **kwargs) -> EvalPipeline:
         eval_pipeline = EvalPipeline()
         eval_pipeline.add_pipe(self.pipes.eval_pipe)
         return eval_pipeline
 
     def create_pipelines(
         self,
         ingestion_pipeline: Optional[IngestionPipeline] = None,
         search_pipeline: Optional[SearchPipeline] = None,
         rag_pipeline: Optional[RAGPipeline] = None,
         streaming_rag_pipeline: Optional[RAGPipeline] = None,
         eval_pipeline: Optional[EvalPipeline] = None,
+        *args,
+        **kwargs,
     ) -> R2RPipelines:
         try:
             self.configure_logging()
         except Exception as e:
             logger.warn(f"Error configuring logging: {e}")
 
         return R2RPipelines(
             ingestion_pipeline=ingestion_pipeline
-            or self.create_ingestion_pipeline(),
-            search_pipeline=search_pipeline or self.create_search_pipeline(),
+            or self.create_ingestion_pipeline(*args, **kwargs),
+            search_pipeline=search_pipeline
+            or self.create_search_pipeline(*args, **kwargs),
             rag_pipeline=rag_pipeline
-            or self.create_rag_pipeline(streaming=False),
+            or self.create_rag_pipeline(streaming=False, *args, **kwargs),
             streaming_rag_pipeline=streaming_rag_pipeline
-            or self.create_rag_pipeline(streaming=True),
-            eval_pipeline=eval_pipeline or self.create_eval_pipeline(),
+            or self.create_rag_pipeline(streaming=True, *args, **kwargs),
+            eval_pipeline=eval_pipeline
+            or self.create_eval_pipeline(*args, **kwargs),
         )
 
     def configure_logging(self):
-        PipeLoggingConnectionSingleton.configure(self.config.logging)
+        KVLoggingSingleton.configure(self.config.logging)
```

### Comparing `r2r-0.2.3/r2r/pipes/__init__.py` & `r2r-0.2.4/r2r/pipes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from .abstractions.search_pipe import SearchPipe
 from .embedding_pipe import R2REmbeddingPipe
 from .eval_pipe import R2REvalPipe
 from .parsing_pipe import R2RDocumentParsingPipe
 from .query_transform_pipe import R2RQueryTransformPipe
 from .rag_pipe import R2RRAGPipe
 from .streaming_rag_pipe import R2RStreamingRAGPipe
 from .vector_search_pipe import R2RVectorSearchPipe
 from .vector_storage_pipe import R2RVectorStoragePipe
+from .web_search_pipe import R2RWebSearchPipe
 
 __all__ = [
+    "SearchPipe",
     "R2REmbeddingPipe",
     "R2REvalPipe",
     "R2RDocumentParsingPipe",
     "R2RQueryTransformPipe",
     "R2RRAGPipe",
     "R2RStreamingRAGPipe",
     "R2RVectorSearchPipe",
     "R2RVectorStoragePipe",
+    "R2RWebSearchPipe",
 ]
```

### Comparing `r2r-0.2.3/r2r/pipes/abstractions/generator_pipe.py` & `r2r-0.2.4/r2r/pipes/abstractions/generator_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import uuid
 from abc import abstractmethod
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncState,
     GenerationConfig,
     LLMProvider,
@@ -36,14 +37,15 @@
         self.prompt_provider = prompt_provider
 
     @abstractmethod
     async def _run_logic(
         self,
         input: LoggableAsyncPipe.Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         rag_generation_config: GenerationConfig,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[Any, None]:
         pass
 
     @abstractmethod
```

### Comparing `r2r-0.2.3/r2r/pipes/abstractions/search_pipe.py` & `r2r-0.2.4/r2r/pipes/abstractions/search_pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
+import uuid
 from abc import abstractmethod
 from typing import Any, AsyncGenerator, Optional, Union
 
 from r2r.core import (
     AsyncPipe,
     AsyncState,
+    KVLoggingSingleton,
     LoggableAsyncPipe,
-    PipeLoggingConnectionSingleton,
     PipeType,
     SearchResult,
     VectorDBProvider,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -22,29 +23,27 @@
         search_limit: int = 10
 
     class Input(AsyncPipe.Input):
         message: Union[AsyncGenerator[str, None], str]
 
     def __init__(
         self,
-        vector_db_provider: VectorDBProvider,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.SEARCH,
         config: Optional[AsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         super().__init__(
             pipe_logger=pipe_logger,
             type=type,
             config=config,
             *args,
             **kwargs,
         )
-        self.vector_db_provider = vector_db_provider
 
     @abstractmethod
     async def search(
         self,
         query: str,
         filters: dict[str, Any] = {},
         limit: int = 10,
@@ -54,11 +53,12 @@
         pass
 
     @abstractmethod
     async def _run_logic(
         self,
         input: Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs,
     ) -> AsyncGenerator[SearchResult, None]:
         pass
```

### Comparing `r2r-0.2.3/r2r/pipes/embedding_pipe.py` & `r2r-0.2.4/r2r/pipes/embedding_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
 import copy
 import json
 import logging
+import uuid
 from abc import abstractmethod
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncState,
     EmbeddingProvider,
     Extraction,
     Fragment,
     FragmentType,
+    KVLoggingSingleton,
     LoggableAsyncPipe,
-    PipeLoggingConnectionSingleton,
     PipeType,
     TextSplitter,
     Vector,
     VectorEntry,
     generate_id_from_label,
 )
 
@@ -26,15 +27,15 @@
 class EmbeddingPipe(LoggableAsyncPipe):
     class Input(LoggableAsyncPipe.Input):
         message: AsyncGenerator[Extraction, None]
 
     def __init__(
         self,
         embedding_provider: EmbeddingProvider,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.INGESTOR,
         config: Optional[LoggableAsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         super().__init__(
             pipe_logger=pipe_logger,
@@ -62,14 +63,15 @@
         pass
 
     @abstractmethod
     async def _run_logic(
         self,
         input: AsyncGenerator[Extraction, None],
         state: AsyncState,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[VectorEntry, None]:
         pass
 
 
 class R2REmbeddingPipe(EmbeddingPipe):
@@ -79,15 +81,15 @@
 
     def __init__(
         self,
         embedding_provider: EmbeddingProvider,
         text_splitter: TextSplitter,
         embedding_batch_size: int = 1,
         id_prefix: str = "demo",
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.INGESTOR,
         config: Optional[LoggableAsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         """
         Initializes the embedding pipe with necessary components and configurations.
@@ -101,15 +103,15 @@
         )
         self.text_splitter = text_splitter
         self.embedding_batch_size = embedding_batch_size
         self.id_prefix = id_prefix
         self.pipe_run_info = None
 
     async def fragment(
-        self, extraction: Extraction
+        self, extraction: Extraction, run_id: uuid.UUID
     ) -> AsyncGenerator[Fragment, None]:
         """
         Splits text into manageable chunks for embedding.
         """
         if not isinstance(extraction, Extraction):
             raise ValueError(
                 f"Expected an Extraction, but received {type(extraction)}."
@@ -130,15 +132,15 @@
                 metadata=copy.deepcopy(extraction.metadata),
                 extraction_id=extraction.id,
                 document_id=extraction.document_id,
             )
             yield fragment
             fragment_dict = fragment.dict()
             await self.enqueue_log(
-                pipe_run_id=self.run_info.run_id,
+                run_id=run_id,
                 key="fragment",
                 value=json.dumps(
                     {
                         "data": fragment_dict["data"],
                         "document_id": str(fragment_dict["document_id"]),
                         "extraction_id": str(fragment_dict["extraction_id"]),
                         "fragment_id": str(fragment_dict["id"]),
@@ -186,25 +188,26 @@
             for raw_vector, fragment in zip(vectors, fragment_batch)
         ]
 
     async def _run_logic(
         self,
         input: EmbeddingPipe.Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[VectorEntry, None]:
         """
         Executes the embedding pipe: chunking, transforming, embedding, and storing documents.
         """
         batch_tasks = []
         fragment_batch = []
 
         async for extraction in input.message:
-            async for fragment in self.fragment(extraction):
+            async for fragment in self.fragment(extraction, run_id):
                 fragment_batch.append(fragment)
                 if len(fragment_batch) >= self.embedding_batch_size:
                     # Here, ensure `_process_batch` is scheduled as a coroutine, not called directly
                     batch_tasks.append(
                         self._process_batch(fragment_batch.copy())
                     )  # pass a copy if necessary
                     fragment_batch.clear()  # Clear the batch for new fragments
```

### Comparing `r2r-0.2.3/r2r/pipes/eval_pipe.py` & `r2r-0.2.4/r2r/pipes/eval_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import random
+import uuid
 from typing import Any, AsyncGenerator, Optional
 
 from pydantic import BaseModel
 
 from r2r import (
     AsyncState,
     EvalProvider,
@@ -38,13 +39,18 @@
             config=config
             or LoggableAsyncPipe.PipeConfig(name="default_eval_pipe"),
             *args,
             **kwargs,
         )
 
     async def _run_logic(
-        self, input: Input, state: AsyncState, *args: Any, **kwargs: Any
+        self,
+        input: Input,
+        run_id: uuid.UUID,
+        state: AsyncState,
+        *args: Any,
+        **kwargs: Any,
     ) -> AsyncGenerator[LLMChatCompletion, None]:
         async for item in input.message:
             yield self.eval_provider.evaluate(
                 item.query, item.context, item.completion
             )
```

### Comparing `r2r-0.2.3/r2r/pipes/parsing_pipe.py` & `r2r-0.2.4/r2r/pipes/parsing_pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module contains the `DocumentParsingPipe` class, which is responsible for parsing incoming documents into plaintext.
 """
 
 import asyncio
 import json
 import logging
 import time
+import uuid
 from abc import abstractmethod
 from typing import AsyncGenerator, Iterator, Optional
 
 from r2r.core import (
     AsyncParser,
     AsyncState,
     AudioParser,
@@ -18,19 +19,19 @@
     DocumentType,
     DOCXParser,
     Extraction,
     ExtractionType,
     HTMLParser,
     ImageParser,
     JSONParser,
+    KVLoggingSingleton,
     LoggableAsyncPipe,
     MarkdownParser,
     MovieParser,
     PDFParser,
-    PipeLoggingConnectionSingleton,
     PipeType,
     PPTParser,
     TextParser,
     XLSXParser,
     generate_id_from_label,
 )
 
@@ -38,15 +39,15 @@
 
 
 class DocumentParsingPipe(LoggableAsyncPipe):
     def __init__(
         self,
         selected_parsers: Optional[dict[DocumentType, AsyncParser]] = None,
         override_parsers: Optional[dict[DocumentType, AsyncParser]] = None,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.INGESTOR,
         config: Optional[LoggableAsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         super().__init__(
             pipe_logger=pipe_logger,
@@ -111,15 +112,15 @@
         DocumentType.SVG,
     }
 
     def __init__(
         self,
         selected_parsers: dict[DocumentType, AsyncParser],
         override_parsers: Optional[dict[DocumentType, AsyncParser]] = None,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.INGESTOR,
         config: Optional[LoggableAsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         logger.info(
             "Initializing a `R2RDocumentParsingPipe` to parse incoming documents."
@@ -154,14 +155,15 @@
 
                 logger.error(error_message)
                 raise ValueError(error_message)
 
     async def _parse(
         self,
         document: Document,
+        run_id: uuid.UUID,
     ) -> AsyncGenerator[Extraction, None]:
         if document.type not in self.parsers:
             logger.error(
                 f"Parser for {document.type} not found in `R2RDocumentParsingPipe`."
             )
             return
         parser = self.parsers[document.type]
@@ -194,15 +196,15 @@
                 metadata=document.metadata,
                 document_id=document.id,
                 type=extraction_type,
             )
             yield extraction
             extraction_dict = extraction.dict()
             await self.enqueue_log(
-                pipe_run_id=self.run_info.run_id,
+                run_id=run_id,
                 key="extraction",
                 value=json.dumps(
                     {
                         "data": extraction_dict["data"],
                         "document_id": str(extraction_dict["document_id"]),
                         "extraction_id": str(extraction_dict["id"]),
                     }
@@ -210,26 +212,38 @@
             )
             iteration += 1
         logger.info(
             f"Parsed document with metadata={document.metadata} and id={document.id} in t={time.time()-t0:.2f} seconds."
         )
 
     async def _run_logic(
-        self, input: Input, state: AsyncState, *args, **kwargs
+        self,
+        input: Input,
+        state: AsyncState,
+        run_id: uuid.UUID,
+        versions: Optional[list[str]] = None,
+        *args,
+        **kwargs,
     ) -> AsyncGenerator[Extraction, None]:
         parse_tasks = []
 
+        iteration = 0
         async for document in input.message:
-            parse_tasks.append(self._handle_parse_task(document))
+            version = versions[iteration] if versions else "v0"
+            iteration += 1
+            parse_tasks.append(
+                self._handle_parse_task(document, version, run_id)
+            )
 
         # Await all tasks and yield results concurrently
         for parse_task in asyncio.as_completed(parse_tasks):
             for extraction in await parse_task:
                 yield extraction
 
     async def _handle_parse_task(
-        self, document: Document
+        self, document: Document, version: str, run_id: uuid.UUID
     ) -> AsyncGenerator[Extraction, None]:
         extractions = []
-        async for extraction in self._parse(document):
+        async for extraction in self._parse(document, run_id):
+            extraction.metadata["version"] = version
             extractions.append(extraction)
         return extractions
```

### Comparing `r2r-0.2.3/r2r/pipes/query_transform_pipe.py` & `r2r-0.2.4/r2r/pipes/query_transform_pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import uuid
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncPipe,
     AsyncState,
     GenerationConfig,
     LLMProvider,
@@ -43,15 +44,16 @@
             **kwargs,
         )
 
     async def _run_logic(
         self,
         input: AsyncPipe.Input,
         state: AsyncState,
-        query_transform_config: GenerationConfig,
+        run_id: uuid.UUID,
+        query_transform_generation_config: GenerationConfig,
         num_query_xf_outputs: int = 3,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[str, None]:
         async for query in input.message:
             logger.info(
                 f"Transforming query: {query} into {num_query_xf_outputs} outputs with {self.config.task_prompt}."
@@ -59,15 +61,15 @@
 
             query_transform_request = self._get_message_payload(
                 query, num_outputs=num_query_xf_outputs
             )
 
             response = self.llm_provider.get_completion(
                 messages=query_transform_request,
-                generation_config=query_transform_config,
+                generation_config=query_transform_generation_config,
             )
             content = self.llm_provider.extract_content(response)
             outputs = content.split("\n")
             outputs = [
                 output.strip() for output in outputs if output.strip() != ""
             ]
             await state.update(
```

### Comparing `r2r-0.2.3/r2r/pipes/rag_pipe.py` & `r2r-0.2.4/r2r/pipes/rag_pipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import uuid
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncPipe,
     AsyncState,
     GenerationConfig,
     LLMChatCompletion,
@@ -45,28 +46,29 @@
             **kwargs,
         )
 
     async def _run_logic(
         self,
         input: Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         rag_generation_config: GenerationConfig,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[LLMChatCompletion, None]:
         context = await self._collect_context(input)
         messages = self._get_message_payload("\n".join(input.query), context)
 
         response = self.llm_provider.get_completion(
             messages=messages, generation_config=rag_generation_config
         )
         yield response
 
         await self.enqueue_log(
-            pipe_run_id=self.run_info.run_id,
+            run_id=run_id,
             key="llm_response",
             value=response.choices[0].message.content,
         )
 
     def _get_message_payload(self, query: str, context: str) -> dict:
         return [
             {
```

### Comparing `r2r-0.2.3/r2r/pipes/streaming_rag_pipe.py` & `r2r-0.2.4/r2r/pipes/streaming_rag_pipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import uuid
 from typing import Any, AsyncGenerator, Generator, Optional
 
 from r2r.core import (
     AsyncState,
     GenerationConfig,
     LLMChatCompletionChunk,
     LLMProvider,
@@ -42,14 +43,15 @@
             **kwargs,
         )
 
     async def _run_logic(
         self,
         input: R2RRAGPipe.Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         rag_generation_config: GenerationConfig,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[str, None]:
         iteration = 0
         context = ""
         # dump the search results and construct the context
@@ -71,15 +73,15 @@
             chunk = R2RStreamingRAGPipe._process_chunk(chunk)
             response += chunk
             yield chunk
 
         yield f"</{self.COMPLETION_STREAM_MARKER}>"
 
         await self.enqueue_log(
-            pipe_run_id=self.run_info.run_id,
+            run_id=run_id,
             key="llm_response",
             value=response,
         )
 
     async def _yield_chunks(
         self,
         start_marker: str,
```

### Comparing `r2r-0.2.3/r2r/pipes/vector_search_pipe.py` & `r2r-0.2.4/r2r/pipes/vector_search_pipe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import uuid
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncPipe,
     AsyncState,
     EmbeddingProvider,
     PipeType,
@@ -23,64 +24,65 @@
         embedding_provider: EmbeddingProvider,
         type: PipeType = PipeType.SEARCH,
         config: Optional[SearchPipe.SearchConfig] = None,
         *args,
         **kwargs,
     ):
         super().__init__(
-            vector_db_provider=vector_db_provider,
             type=type,
             config=config or SearchPipe.SearchConfig(),
             *args,
             **kwargs,
         )
         self.embedding_provider = embedding_provider
+        self.vector_db_provider = vector_db_provider
 
     async def search(
         self,
         message: str,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[SearchResult, None]:
         search_filters_override = kwargs.get("search_filters", None)
         search_limit_override = kwargs.get("search_limit", None)
         await self.enqueue_log(
-            pipe_run_id=self.run_info.run_id, key="search_query", value=message
+            run_id=run_id, key="search_query", value=message
         )
         results = []
         for result in self.vector_db_provider.search(
             query_vector=self.embedding_provider.get_embedding(
                 message,
             ),
             filters=search_filters_override or self.config.search_filters,
             limit=search_limit_override or self.config.search_limit,
         ):
             result.metadata["associatedQuery"] = message
             results.append(result)
             yield result
-
         await self.enqueue_log(
-            pipe_run_id=self.run_info.run_id,
+            run_id=run_id,
             key="search_results",
             value=json.dumps([ele.json() for ele in results]),
         )
 
     async def _run_logic(
         self,
         input: AsyncPipe.Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[SearchResult, None]:
         search_queries = []
         search_results = []
         async for search_request in input.message:
             search_queries.append(search_request)
             async for result in self.search(
-                message=search_request, *args, **kwargs
+                message=search_request, run_id=run_id, *args, **kwargs
             ):
                 search_results.append(result)
                 yield result
 
         await state.update(
             self.config.name, {"output": {"search_results": search_results}}
         )
```

### Comparing `r2r-0.2.3/r2r/pipes/vector_storage_pipe.py` & `r2r-0.2.4/r2r/pipes/vector_storage_pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import logging
+import uuid
 from typing import Any, AsyncGenerator, Optional
 
 from r2r.core import (
     AsyncState,
+    KVLoggingSingleton,
     LoggableAsyncPipe,
-    PipeLoggingConnectionSingleton,
     PipeType,
     VectorDBProvider,
     VectorEntry,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -19,15 +20,15 @@
         message: AsyncGenerator[VectorEntry, None]
         do_upsert: bool = True
 
     def __init__(
         self,
         vector_db_provider: VectorDBProvider,
         storage_batch_size: int = 128,
-        pipe_logger: Optional[PipeLoggingConnectionSingleton] = None,
+        pipe_logger: Optional[KVLoggingSingleton] = None,
         type: PipeType = PipeType.INGESTOR,
         config: Optional[LoggableAsyncPipe.PipeConfig] = None,
         *args,
         **kwargs,
     ):
         """
         Initializes the async vector storage pipe with necessary components and configurations.
@@ -66,14 +67,15 @@
             logger.error(error_message)
             raise ValueError(error_message)
 
     async def _run_logic(
         self,
         input: Input,
         state: AsyncState,
+        run_id: uuid.UUID,
         *args: Any,
         **kwargs: Any,
     ) -> AsyncGenerator[None, None]:
         """
         Executes the async vector storage pipe: storing embeddings in the vector database.
         """
         batch_tasks = []
```

### Comparing `r2r-0.2.3/r2r/prompts/local/defaults.jsonl` & `r2r-0.2.4/r2r/prompts/local/defaults.jsonl`

 * *Files 2% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 {"name": "default_system", "template": "You are a helpful assistant.", "input_types": {}}
 {"name": "default_rag", "template": "## Task:\n\nAnswer the query given immediately below given the context which follows later. Use line item references to like [1], [2], ... refer to specifically numbered items in the provided context. Pay close attention to the title of each given source to ensure it is consistent with the query.\n\n### Query:\n{query}\n\n### Context:\n{context}\n\n### Query:\n{query}\n\nREMINDER - Use line item references to like [1], [2], ... refer to specifically numbered items in the provided context.\n## Response:\n", "input_types": {"query": "str", "context": "str"}}
-{"name": "hyde", "template": "### Instruction:\n\nGiven the following query that follows to write a double newline separated list of up to {num_outputs} single paragraph attempted answers. \nDO NOT generate any single answer which is likely to require information from multiple distinct documents, \nEACH single answer will be used to carry out a cosine similarity semantic search over distinct indexed documents, such as varied medical documents. \nFOR EXAMPLE if asked `how do the key themes of Great Gatsby compare with 1984`, the two attempted answers would be \n`The key themes of Great Gatsby are ... ANSWER_CONTINUED` and `The key themes of 1984 are ... ANSWER_CONTINUED`, where `ANSWER_CONTINUED` IS TO BE COMPLETED BY YOU in your response. \nHere is the original user query to be transformed into answers:\n\n### Query:\n{message}\n\n### Response:\n", "input_types": {"num_outputs": "int", "message": "str"}}
+{"name": "hyde", "template": "### Instruction:\n\nGiven the query that follows write a double newline separated list of {num_outputs} single paragraph distinct attempted answers to the given query. \nDO NOT generate any single answer which is likely to require information from multiple distinct documents, \nEACH single answer will be used to carry out a cosine similarity semantic search over distinct indexed documents, such as varied medical documents. \nFOR EXAMPLE if asked `how do the key themes of Great Gatsby compare with 1984`, the two attempted answers would be \n`The key themes of Great Gatsby are ... ANSWER_CONTINUED` and `The key themes of 1984 are ... ANSWER_CONTINUED`, where `ANSWER_CONTINUED` IS TO BE COMPLETED BY YOU in your response. \nHere is the original user query to be transformed into answers:\n\n### Query:\n{message}\n\n### Response:\n", "input_types": {"num_outputs": "int", "message": "str"}}
 {"name": "rag_fusion_prompt", "template": "### Instruction:\n\nGiven the following query that follows to write a double newline separated list of up to {num_outputs} queries meant to help answer the original query. \nDO NOT generate any single query which is likely to require information from multiple distinct documents, \nEACH single query will be used to carry out a cosine similarity semantic search over distinct indexed documents, such as varied medical documents. \nFOR EXAMPLE if asked `how do the key themes of Great Gatsby compare with 1984`, the two queries would be \n`What are the key themes of Great Gatsby?` and `What are the key themes of 1984?`.\nHere is the original user query to be transformed into answers:\n\n### Query:\n{message}\n\n### Response:\n", "input_types": {"num_outputs": "int", "message": "str"}}
 {"name": "rag_answer_eval", "template": "### Instruction:\n\nYou are given a `query`, related `context` and an associated `answer`. Your task is to sequentially score each sentence in the given answer as either 1 or 0, based on whether or not the given sentence is relevant to the given query and supported in full by the given context.\n### Example:\n#### Input:\n\nQuery:\nWhy does Alice prefer spending her mornings in the garden?\n\nContext:\nAlice loves to read books in her garden. She has a large collection of mystery novels. Every morning, she spends an hour reading while drinking her favorite tea. Her garden is filled with various flowers, and she especially loves the roses. On weekends, Alice's friend, Bob, often joins her for tea and they discuss the books they've read.\n\nAnswer:\nAlice enjoys her mornings in the garden because she loves to read there. She often listens to music while reading.\n####### Response:\n\n([1,0], '1/2')### Input:\nQuery:\n{query}\n\nContext:\n{context}\n\nAnswer:\n{answer}\n\nResponse:\n\n",  "input_types": {"query": "str", "context": "str", "answer": "str"}}
 {"name": "rag_context_eval", "template": "### Instruction:\n\nYou are given a `query` and an associated `context`. Your task is to sequentially score each sentence in the context as either 1 or 0, based on the relevancy to the given query. For instance, if the query is \"What is the capital of France?\" then the sentence \"The capital of France is Paris\" would receive a +1 value, whereas \"The french enjoy wine\" would receive a 0. Return your response as a tuple containing a list of 1s and 0s, where each value corresponds to the respective sentence in the context, and then the rational fraction of 1's to the total number of sentences (e.g. '1/4'). NOTE - do not include ANY extra text other than the requested tuple.\n\nQuery:\n{query}\n\nContext:\n{context}\n\n###Response\n\n", "input_types": {"query": "str", "context": "str"}}
```

### Comparing `r2r-0.2.3/r2r/prompts/local/r2r_prompt_provider.py` & `r2r-0.2.4/r2r/prompts/local/r2r_prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/__init__.py` & `r2r-0.2.4/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/adapter/base.py` & `r2r-0.2.4/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/adapter/markdown.py` & `r2r-0.2.4/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/adapter/noop.py` & `r2r-0.2.4/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/adapter/text.py` & `r2r-0.2.4/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/client.py` & `r2r-0.2.4/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vecs/collection.py` & `r2r-0.2.4/r2r/vecs/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -948,121 +948,104 @@
                     )
 
         return None
 
 
 def build_filters(json_col: Column, filters: Dict):
     """
-    PRIVATE
-
     Builds filters for SQL query based on provided dictionary.
 
     Args:
         json_col (Column): The column in the database table.
         filters (Dict): The dictionary specifying filter conditions.
 
     Raises:
         FilterError: If filter conditions are not correctly formatted.
 
     Returns:
         The filter clause for the SQL query.
     """
-
     if not isinstance(filters, dict):
         raise FilterError("filters must be a dict")
 
-    if len(filters) > 1:
-        raise FilterError("max 1 entry per filter")
+    filter_clauses = []
 
     for key, value in filters.items():
         if not isinstance(key, str):
             raise FilterError("*filters* keys must be strings")
 
-        if key in ("$and", "$or"):
-            if not isinstance(value, list):
-                raise FilterError(
-                    "$and/$or filters must have associated list of conditions"
-                )
-
-            if key == "$and":
-                return and_(
-                    *[build_filters(json_col, subcond) for subcond in value]
-                )
-
-            if key == "$or":
-                return or_(
-                    *[build_filters(json_col, subcond) for subcond in value]
-                )
-
-            raise Unreachable()
-
         if isinstance(value, dict):
             if len(value) > 1:
-                raise FilterError("only one operator permitted")
+                raise FilterError("only one operator permitted per key")
             for operator, clause in value.items():
                 if operator not in (
                     "$eq",
                     "$ne",
                     "$lt",
                     "$lte",
                     "$gt",
                     "$gte",
                     "$in",
                 ):
                     raise FilterError("unknown operator")
 
-                # equality of singular values can take advantage of the metadata index
-                # using containment operator. Containment can not be used to test equality
-                # of lists or dicts so we restrict to single values with a __len__ check.
                 if operator == "$eq" and not hasattr(clause, "__len__"):
                     contains_value = cast({key: clause}, postgresql.JSONB)
-                    return json_col.op("@>")(contains_value)
-
-                if operator == "$in":
+                    filter_clauses.append(json_col.op("@>")(contains_value))
+                elif operator == "$in":
                     if not isinstance(clause, list):
                         raise FilterError(
                             "argument to $in filter must be a list"
                         )
-
                     for elem in clause:
                         if not isinstance(elem, (int, str, float)):
                             raise FilterError(
-                                "argument to $in filter must be a list or scalars"
+                                "argument to $in filter must be a list of scalars"
                             )
-
-                    # cast the array of scalars to a postgres array of jsonb so we can
-                    # directly compare json types in the query
                     contains_value = [
                         cast(elem, postgresql.JSONB) for elem in clause
                     ]
-                    return json_col.op("->")(key).in_(contains_value)
-
-                matches_value = cast(clause, postgresql.JSONB)
-
-                # handles non-singular values
-                if operator == "$eq":
-                    return json_col.op("->")(key) == matches_value
-
-                elif operator == "$ne":
-                    return json_col.op("->")(key) != matches_value
-
-                elif operator == "$lt":
-                    return json_col.op("->")(key) < matches_value
-
-                elif operator == "$lte":
-                    return json_col.op("->")(key) <= matches_value
-
-                elif operator == "$gt":
-                    return json_col.op("->")(key) > matches_value
-
-                elif operator == "$gte":
-                    return json_col.op("->")(key) >= matches_value
-
+                    filter_clauses.append(
+                        json_col.op("->")(key).in_(contains_value)
+                    )
                 else:
-                    raise Unreachable()
+                    matches_value = cast(clause, postgresql.JSONB)
+                    if operator == "$eq":
+                        filter_clauses.append(
+                            json_col.op("->")(key) == matches_value
+                        )
+                    elif operator == "$ne":
+                        filter_clauses.append(
+                            json_col.op("->")(key) != matches_value
+                        )
+                    elif operator == "$lt":
+                        filter_clauses.append(
+                            json_col.op("->")(key) < matches_value
+                        )
+                    elif operator == "$lte":
+                        filter_clauses.append(
+                            json_col.op("->")(key) <= matches_value
+                        )
+                    elif operator == "$gt":
+                        filter_clauses.append(
+                            json_col.op("->")(key) > matches_value
+                        )
+                    elif operator == "$gte":
+                        filter_clauses.append(
+                            json_col.op("->")(key) >= matches_value
+                        )
+                    else:
+                        raise Unreachable()
+        else:
+            raise FilterError("Filter value must be a dict with an operator")
+
+    if len(filter_clauses) == 1:
+        return filter_clauses[0]
+    else:
+        return and_(*filter_clauses)
 
 
 def build_table(name: str, meta: MetaData, dimension: int) -> Table:
     """
     PRIVATE
 
     Builds a SQLAlchemy model underpinning a `vecs.Collection`.
```

### Comparing `r2r-0.2.3/r2r/vecs/exc.py` & `r2r-0.2.4/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.2.3/r2r/vector_dbs/local/r2r_local_vector_db.py` & `r2r-0.2.4/r2r/vector_dbs/local/r2r_local_vector_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -134,27 +134,37 @@
                     SearchResult(id=id, score=score, metadata=json_metadata)
                 )
         results.sort(key=lambda x: x.score, reverse=True)
         conn.close()
         return results[:limit]
 
     def delete_by_metadata(
-        self, metadata_field: str, metadata_value: Union[bool, int, str]
+        self,
+        metadata_fields: list[str],
+        metadata_values: list[Union[bool, int, str]],
     ) -> None:
+        super().delete_by_metadata(metadata_fields, metadata_values)
         if self.config.collection_name is None:
             raise ValueError(
                 "Collection name is not set. Please call `initialize_collection` first."
             )
 
         conn = self._get_conn()
         cursor = self._get_cursor(conn)
         cursor.execute(f'SELECT * FROM "{self.config.collection_name}"')
-        for id, vector, metadata in cursor.fetchall():
+        for id, _, metadata in cursor.fetchall():
             metadata_json = json.loads(metadata)
-            if metadata_json.get(metadata_field) == metadata_value:
+            is_valid = True
+            for metadata_field, metadata_value in zip(
+                metadata_fields, metadata_values
+            ):
+                if metadata_json.get(metadata_field) != metadata_value:
+                    is_valid = False
+                    break
+            if is_valid:
                 cursor.execute(
                     f'DELETE FROM "{self.config.collection_name}" WHERE id = ?',
                     (id,),
                 )
         conn.commit()
         conn.close()
```

### Comparing `r2r-0.2.3/r2r/vector_dbs/pgvector/pgvector_db.py` & `r2r-0.2.4/r2r/vector_dbs/pgvector/pgvector_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,22 +150,25 @@
             )
         ]
 
     def create_index(self, index_type, column_name, index_options):
         pass
 
     def delete_by_metadata(
-        self, metadata_field: str, metadata_value: Union[bool, int, str]
+        self, metadata_fields: str, metadata_values: Union[bool, int, str]
     ) -> None:
+        super().delete_by_metadata(metadata_fields, metadata_values)
         if self.collection is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `delete_by_metadata`."
             )
         self.collection.delete(
-            filters={metadata_field: {"$eq": metadata_value}}
+            filters={
+                k: {"$eq": v} for k, v in zip(metadata_fields, metadata_values)
+            }
         )
 
     def get_metadatas(
         self,
         metadata_fields: list[str],
         filter_field: Optional[str] = None,
         filter_value: Optional[Union[bool, int, str]] = None,
```

### Comparing `r2r-0.2.3/r2r/vector_dbs/qdrant/qdrant_db.py` & `r2r-0.2.4/r2r/vector_dbs/qdrant/qdrant_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,30 +140,36 @@
             for result in results
         ]
 
     def create_index(self, index_type, column_name, index_options):
         pass
 
     def delete_by_metadata(
-        self, metadata_field: str, metadata_value: Union[bool, int, str]
+        self,
+        metadata_fields: list[str],
+        metadata_values: list[Union[bool, int, str]],
     ) -> None:
+        super().delete_by_metadata(metadata_fields, metadata_values)
         if self.config.collection_name is None:
             raise ValueError(
                 "Please call `initialize_collection` before attempting to run `delete_by_metadata`."
             )
 
         self.client.delete(
             collection_name=self.config.collection_name,
             points_selector=self.models.FilterSelector(
                 filter=self.models.Filter(
                     must=[
                         self.models.FieldCondition(
-                            key=metadata_field,
-                            match=self.models.MatchValue(value=metadata_value),
-                        ),
+                            key=field,
+                            match=self.models.MatchValue(value=value),
+                        )
+                        for field, value in zip(
+                            metadata_fields, metadata_values
+                        )
                     ],
                 )
             ),
         )
         return
 
     def get_metadatas(
```

### Comparing `r2r-0.2.3/PKG-INFO` & `r2r-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.2.3
+Version: 0.2.4
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: exa
 Provides-Extra: ionic
+Provides-Extra: local-embedding
 Provides-Extra: local-llm
-Provides-Extra: sentence-transformers-only
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
@@ -35,15 +35,15 @@
 Requires-Dist: pypdf (>=4.2.0,<5.0.0)
 Requires-Dist: python-docx (>=1.1.0,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: python-pptx (>=0.6.23,<0.7.0)
 Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ; extra == "all"
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: sentence-transformers (>=2.7.0,<3.0.0) ; extra == "all" or extra == "local-llm" or extra == "sentence-transformers-only"
+Requires-Dist: sentence-transformers (>=2.7.0,<3.0.0) ; extra == "all" or extra == "local-embedding"
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "all"
 Requires-Dist: types-requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0)
 Requires-Dist: vecs (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 <p align="left">
@@ -57,15 +57,15 @@
 <img src="./docs/pages/r2r.png" alt="Sciphi Framework">
 <h3 align="center">
 Build, deploy, observe, and optimize your RAG system.
 </h3>
 
 # About
 
-R2R, short for RAG to Riches, provides the fastest and most efficient way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is built around customizable pipelines and a feature-rich FastAPI implementation.
+R2R, short for RAG to Riches, provides the fastest and most efficient way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users. The framework is built around customizable pipelines and ships with a feature-rich REST API.
 
 ## Why?
 
 R2R was conceived to bridge the gap between local LLM experimentation and scalable production solutions. It is built with observability and customization in mind, ensuring that users can seamlessly transition from development to deployment.
 
 ## Key Features
 - **🔧 Build**: Use the framework to build arbitrary asynchronous pipelines.
@@ -97,16 +97,14 @@
 
 [Join the Discord server](https://discord.gg/p6KqD2kjtB)
 
 [R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
 
 [SciPhi Cloud Docs](https://docs.sciphi.ai/)
 
-[Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/local_rag)
-
 # R2R Demo
 
 The R2R demo offers a step-by-step guide on running the default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests a list of provided provided documents and demonstrates search, RAG, and advanced functionality. The script at `r2r/examples/demo.py`, which powers the demo, can be configured and extended with sufficient developer familiarity.
 
 ## Ingest Demo Files
 
 To comprehensively demonstrate the RAG functionalities of the R2R framework, we must start by ingesting a realistic set of documents. Running the command below will parse, chunk, embed, and store a preset list of files. The included file types cover HTML, PDF, PNG, and TXT examples:
@@ -127,15 +125,15 @@
 ```
 
 ### Confirm User Data
 
 To verify the successful ingestion of the demo documents, you can fetch the metadata for the uploaded documents associated with the default demo user ID:
 
 ```bash
-python -m r2r.examples.demo get_user_document_data --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
+python -m r2r.examples.demo get_user_documents_metadata --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
 ```
 
 **Demo Output:**
 
 ```plaintext
 ...
 Time taken to get user document data: 0.21 seconds
@@ -251,29 +249,37 @@
 <search>["{\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... </search>
 <completion>Lyft reported a net loss of $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit in 2020.</completion>                                                      
 Time taken to stream RAG response: 2.79 seconds
 ```
 
 ## Document Management Demo
 
+### Update Document 
+
+To update document(s) we may use the `update_as_files` or `update_as_documents` endpoints. Running the demo with `update_as_files` overwrites the data associated with 'aristotle.txt' with new data corresponding to 'aristotle_v2.txt' and increments the file version.
+
+```bash
+poetry run python -m r2r.examples.demo update_as_files
+```
+
 ### Document Deletion
 
-To delete a document by its ID, or any other metadata field, use the delete command. For example, to delete all chunks corresponding to the uploaded file `aristotle.txt`, we can call delete on the associated document ID with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
+To delete a document by its ID, or any other metadata field, use the delete command. For example, to delete all chunks corresponding to the uploaded file `aristotle.txt`, we can call delete on the metadata field `document_id` with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
 
 ```bash
-python -m r2r.examples.demo delete --key=document_id --value=15255e98-e245-5b58-a57f-6c51babf72dd
+poetry run python -m r2r.examples.demo delete --keys="['document_id']" --values="['c9bdbac7-0ea3-5c9e-b590-018bd09b127b']"
 ```
 
 ### User Deletion
 
 To delete all documents associated with a given user, run the delete command on the `user_id`:
 
 ```bash
 run the following command with care, as it will erase all ingested user data
-python -m r2r.examples.demo delete --key=user_id --value=063edaf8-3e63-4cb9-a4d6-a855f36376c3
+python -m r2r.examples.demo delete --keys="['user_id']" --values="['063edaf8-3e63-4cb9-a4d6-a855f36376c3']"
 ```
 
 ## R2R Server-Client Demo
 
 This section extends the previous demo by showing how to set up and use the R2R framework with a server-client architecture. The R2R server can be stood up to handle requests, while the client can communicate with the server to perform various operations.
 
 ### Launch the Server
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.2.3 Summary: SciPhi R2R License: MIT
+Metadata-Version: 2.1 Name: r2r Version: 0.2.4 Summary: SciPhi R2R License: MIT
 Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: exa Provides-Extra: ionic
-Provides-Extra: local-llm Provides-Extra: sentence-transformers-only Requires-
-Dist: aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
+Provides-Extra: local-embedding Provides-Extra: local-llm Requires-Dist:
+aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3) Requires-Dist: exa-py (>=1.0.9,<2.0.0) ;
 extra == "exa" Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fire
 (>=0.5.0,<0.6.0) Requires-Dist: gunicorn (>=21.2.0,<22.0.0) Requires-Dist:
 ionic-api-sdk (==0.9.3) ; extra == "ionic" Requires-Dist: litellm
 (>=1.35.18,<2.0.0) Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra ==
 "all" or extra == "local-llm" Requires-Dist: markdown (>=3.6,<4.0) Requires-
 Dist: nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0) Requires-Dist: pydantic
 (>=2.6.3,<3.0.0) Requires-Dist: pypdf (>=4.2.0,<5.0.0) Requires-Dist: python-
 docx (>=1.1.0,<2.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: python-pptx (>=0.6.23,<0.7.0) Requires-Dist: qdrant_client
 (>=1.7.0,<2.0.0) ; extra == "all" Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: sentence-transformers
-(>=2.7.0,<3.0.0) ; extra == "all" or extra == "local-llm" or extra ==
-"sentence-transformers-only" Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra
-== "all" Requires-Dist: types-requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn
-(>=0.27.0.post1,<0.28.0) Requires-Dist: vecs (>=0.4.0,<0.5.0) Description-
-Content-Type: text/markdown
+(>=2.7.0,<3.0.0) ; extra == "all" or extra == "local-embedding" Requires-Dist:
+tiktoken (>=0.5.2,<0.6.0) ; extra == "all" Requires-Dist: types-requests
+(>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.27.0.post1,<0.28.0) Requires-
+Dist: vecs (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown
 _[_D_o_c_s_]_[_D_i_s_c_o_r_d_]_[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
 [Sciphi Framework]
         ******** BBuuiilldd,, ddeeppllooyy,, oobbsseerrvvee,, aanndd ooppttiimmiizzee yyoouurr RRAAGG ssyysstteemm.. ********
 # About R2R, short for RAG to Riches, provides the fastest and most efficient
 way to deliver high-quality Retrieval-Augmented Generation (RAG) to end users.
-The framework is built around customizable pipelines and a feature-rich FastAPI
-implementation. ## Why? R2R was conceived to bridge the gap between local LLM
+The framework is built around customizable pipelines and ships with a feature-
+rich REST API. ## Why? R2R was conceived to bridge the gap between local LLM
 experimentation and scalable production solutions. It is built with
 observability and customization in mind, ensuring that users can seamlessly
 transition from development to deployment. ## Key Features - **ð§ Build**:
 Use the framework to build arbitrary asynchronous pipelines. - **ð Deploy**:
 Instantly launch production-ready asynchronous RAG pipelines with streaming
 capabilities. - **ð§© Customize**: Tailor your multimodal pipeline with
 intuitive configuration files. - **ð Extend**: Enhance your pipeline with
@@ -44,53 +43,52 @@
 Contents 1. [Quick Install](#quick-install) 2. [Links](#links) 3. [R2R Demo]
 (#r2r-demo) 4. [R2R Server-Client Demo](#r2r-server-client-demo) 5. [Core
 Abstractions](#core-abstractions) 6. [Summary](#summary) # Quick Install:
 ```bash # use the `'r2r[all]'` to download all required deps pip install r2r #
 setup env export OPENAI_API_KEY=sk-... ``` ## Links [Join the Discord server]
 (https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart](https://r2r-
 docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud Docs](https://
-docs.sciphi.ai/) [Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/
-local_rag) # R2R Demo The R2R demo offers a step-by-step guide on running the
-default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests a
-list of provided provided documents and demonstrates search, RAG, and advanced
-functionality. The script at `r2r/examples/demo.py`, which powers the demo, can
-be configured and extended with sufficient developer familiarity. ## Ingest
-Demo Files To comprehensively demonstrate the RAG functionalities of the R2R
-framework, we must start by ingesting a realistic set of documents. Running the
-command below will parse, chunk, embed, and store a preset list of files. The
-included file types cover HTML, PDF, PNG, and TXT examples: ```bash python -
-m r2r.examples.demo ingest_as_files ``` **Demo Output:** ```plaintext ...
+docs.sciphi.ai/) # R2R Demo The R2R demo offers a step-by-step guide on running
+the default R2R Retrieval-Augmented Generation (RAG) pipeline. The demo ingests
+a list of provided provided documents and demonstrates search, RAG, and
+advanced functionality. The script at `r2r/examples/demo.py`, which powers the
+demo, can be configured and extended with sufficient developer familiarity. ##
+Ingest Demo Files To comprehensively demonstrate the RAG functionalities of the
+R2R framework, we must start by ingesting a realistic set of documents. Running
+the command below will parse, chunk, embed, and store a preset list of files.
+The included file types cover HTML, PDF, PNG, and TXT examples: ```bash python
+-m r2r.examples.demo ingest_as_files ``` **Demo Output:** ```plaintext ...
 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'pg_essay_1.html', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3'} and
 id=4a4fb848-fc03-5487-a7e5-33c9fdfb73cc in t=0.00 seconds. - 2024-05-21 08:39:
 59,003 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'lyft_2021.pdf', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3'} and
 id=c5abc0b7-b9e5-54d9-b3d3-fdb14af4d065 in t=3.47 seconds. - 2024-05-21 08:40:
 02,477 r2r.pipes.parsing_pipe - INFO - Parsed document with metadata={'title':
 'screen_shot.png', 'user_id': '063edaf8-3e63-4cb9-a4d6-a855f36376c3',
 'image_type': 'png'} and id=74f1506a-9a37-59d7-b288-5ef3683dca8f in t=18.37
 seconds. - 2024-05-21 08:40:32,310 ... Time taken to ingest files: 28.49
 seconds ``` ### Confirm User Data To verify the successful ingestion of the
 demo documents, you can fetch the metadata for the uploaded documents
 associated with the default demo user ID: ```bash python -m r2r.examples.demo
-get_user_document_data --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3" ```
-**Demo Output:** ```plaintext ... Time taken to get user document data: 0.21
-seconds {'results': [ { 'document_id': '327f6110-edd1-5fe3-b6b3-49b55f1cbc28',
-'title': 'pg_essay_3.html' }, { 'document_id': '946859f0-da5c-5db7-9b5c-
-c586be76d709', 'title': 'pg_essay_5.html' }, { 'document_id': '64c1c913-be06-
-548f-acbc-3618b00d3616', 'title': 'lyft_2021.pdf' }, ... ] } ``` ## Search Demo
-Documents Documents are stored by default in a local vector database. The
-vector database provider and settings can be specified via an input
-`config.json`. To perform a search query on the ingested user documents, use
-the following command: ```bash python -m r2r.examples.demo search --query="Who
-was Aristotle?" ``` **Demo Output:** ```plaintext ... Time taken to search:
-0.39 seconds { 'id': UUID('93c44e73-8e95-50c2-84af-6a42f070b552'), 'score':
-0.7739712385010018, 'metadata': { 'document_id': '15255e98-e245-5b58-a57f-
-6c51babf72dd', 'extraction_id': '5c61f9b9-b468-5fd7-8eb1-5d797a15c484', 'text':
-'Aristotle[A] (Greek: á¼ÏÎ¹ÏÏÎ¿ÏÎ­Î»Î·Ï AristotÃ©lÄs, pronounced
+get_user_documents_metadata --user_id="063edaf8-3e63-4cb9-a4d6-a855f36376c3"
+``` **Demo Output:** ```plaintext ... Time taken to get user document data:
+0.21 seconds {'results': [ { 'document_id': '327f6110-edd1-5fe3-b6b3-
+49b55f1cbc28', 'title': 'pg_essay_3.html' }, { 'document_id': '946859f0-da5c-
+5db7-9b5c-c586be76d709', 'title': 'pg_essay_5.html' }, { 'document_id':
+'64c1c913-be06-548f-acbc-3618b00d3616', 'title': 'lyft_2021.pdf' }, ... ] } ```
+## Search Demo Documents Documents are stored by default in a local vector
+database. The vector database provider and settings can be specified via an
+input `config.json`. To perform a search query on the ingested user documents,
+use the following command: ```bash python -m r2r.examples.demo search --
+query="Who was Aristotle?" ``` **Demo Output:** ```plaintext ... Time taken to
+search: 0.39 seconds { 'id': UUID('93c44e73-8e95-50c2-84af-6a42f070b552'),
+'score': 0.7739712385010018, 'metadata': { 'document_id': '15255e98-e245-5b58-
+a57f-6c51babf72dd', 'extraction_id': '5c61f9b9-b468-5fd7-8eb1-5d797a15c484',
+'text': 'Aristotle[A] (Greek: á¼ÏÎ¹ÏÏÎ¿ÏÎ­Î»Î·Ï AristotÃ©lÄs, pronounced
 [aristotÃ©lÉËs]; 384â322 BC) was an Ancient Greek philosopher and polymath.
 His writings cover a broad range of subjects spanning the natural sciences,
 philosophy, linguistics, economics, politics, psychology, and the arts. As the
 founder of the Peripatetic school of philosophy in the Lyceum in Athens, he
 began the wider Aristotelian tradition that followed, which set the groundwork
 for the development of modern science.', 'title': 'aristotle.txt', 'user_id':
 '063edaf8-3e63-4cb9-a4d6-a855f36376c3', 'query': 'Who was Aristotle?' } } ...
@@ -108,48 +106,53 @@
 streaming results from a RAG query, use the following command: ```bash python -
 m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
 streaming=true ``` **Demo Output:** ```plaintext r2r.main.r2r_config - INFO -
 Loading configuration from /config.json - 2024-05-20 22:27:31,890 ... ["
 {\"id\":\"808c47c5-ebef-504a-a230-aa9ddcfbd87 .... Lyft reported a net loss of
 $1,752,857,000 in 2020 according to [2]. Therefore, Lyft did not make a profit
 in 2020. Time taken to stream RAG response: 2.79 seconds ``` ## Document
-Management Demo ### Document Deletion To delete a document by its ID, or any
-other metadata field, use the delete command. For example, to delete all chunks
-corresponding to the uploaded file `aristotle.txt`, we can call delete on the
-associated document ID with the value `15255e98-e245-5b58-a57f-6c51babf72dd`:
-```bash python -m r2r.examples.demo delete --key=document_id --value=15255e98-
-e245-5b58-a57f-6c51babf72dd ``` ### User Deletion To delete all documents
-associated with a given user, run the delete command on the `user_id`: ```bash
-run the following command with care, as it will erase all ingested user data
-python -m r2r.examples.demo delete --key=user_id --value=063edaf8-3e63-4cb9-
-a4d6-a855f36376c3 ``` ## R2R Server-Client Demo This section extends the
-previous demo by showing how to set up and use the R2R framework with a server-
-client architecture. The R2R server can be stood up to handle requests, while
-the client can communicate with the server to perform various operations. ###
-Launch the Server Use the following command to start the server: ```bash python
--m r2r.examples.demo serve ``` This command starts the R2R server on the
-default host `0.0.0.0` and port `8000`. ### Example Commands 1. **Ingest
-Documents as Files**: ```bash python -m r2r.examples.demo ingest_as_files --
-base_url=http://localhost:8000 ``` This command will send the ingestion request
-to the server running at `http://localhost:8000`. 2. **Perform a Search**:
-```bash python -m r2r.examples.demo search --query="Who was Aristotle?" --
-base_url=http://localhost:8000 ``` This command sends the search query to the
-server and retrieves the results. 3. **Run a RAG Completion**: ```bash python -
-m r2r.examples.demo rag --query="What was Uber's profit in 2020?" --
-base_url=http://localhost:8000 ``` This command sends the RAG query to the
-server and retrieves the generated response. 4. **Run a RAG Stream**: ```bash
-python -m r2r.examples.demo rag --query="What was Lyft's profit in 2020?" --
-streaming=true --base_url=http://localhost:8000 ``` This command streams the
-RAG query results from the server. ### Server-Client Summary By using the
-server-client model, you can extend the basic R2R demo to support more scalable
-and modular deployments. The server handles requests and performs heavy
-computations, while clients can communicate with the server to perform
-ingestion, search, RAG, and other operations, as shown in the examples above.
-For detailed setup and basic functionality, refer back to the [R2R Demo](#r2r-
-demo). # Core Abstractions The framework revolves around three core
+Management Demo ### Update Document To update document(s) we may use the
+`update_as_files` or `update_as_documents` endpoints. Running the demo with
+`update_as_files` overwrites the data associated with 'aristotle.txt' with new
+data corresponding to 'aristotle_v2.txt' and increments the file version.
+```bash poetry run python -m r2r.examples.demo update_as_files ``` ### Document
+Deletion To delete a document by its ID, or any other metadata field, use the
+delete command. For example, to delete all chunks corresponding to the uploaded
+file `aristotle.txt`, we can call delete on the metadata field `document_id`
+with the value `15255e98-e245-5b58-a57f-6c51babf72dd`: ```bash poetry run
+python -m r2r.examples.demo delete --keys="['document_id']" --values="
+['c9bdbac7-0ea3-5c9e-b590-018bd09b127b']" ``` ### User Deletion To delete all
+documents associated with a given user, run the delete command on the
+`user_id`: ```bash run the following command with care, as it will erase all
+ingested user data python -m r2r.examples.demo delete --keys="['user_id']" --
+values="['063edaf8-3e63-4cb9-a4d6-a855f36376c3']" ``` ## R2R Server-Client Demo
+This section extends the previous demo by showing how to set up and use the R2R
+framework with a server-client architecture. The R2R server can be stood up to
+handle requests, while the client can communicate with the server to perform
+various operations. ### Launch the Server Use the following command to start
+the server: ```bash python -m r2r.examples.demo serve ``` This command starts
+the R2R server on the default host `0.0.0.0` and port `8000`. ### Example
+Commands 1. **Ingest Documents as Files**: ```bash python -m r2r.examples.demo
+ingest_as_files --base_url=http://localhost:8000 ``` This command will send the
+ingestion request to the server running at `http://localhost:8000`. 2.
+**Perform a Search**: ```bash python -m r2r.examples.demo search --query="Who
+was Aristotle?" --base_url=http://localhost:8000 ``` This command sends the
+search query to the server and retrieves the results. 3. **Run a RAG
+Completion**: ```bash python -m r2r.examples.demo rag --query="What was Uber's
+profit in 2020?" --base_url=http://localhost:8000 ``` This command sends the
+RAG query to the server and retrieves the generated response. 4. **Run a RAG
+Stream**: ```bash python -m r2r.examples.demo rag --query="What was Lyft's
+profit in 2020?" --streaming=true --base_url=http://localhost:8000 ``` This
+command streams the RAG query results from the server. ### Server-Client
+Summary By using the server-client model, you can extend the basic R2R demo to
+support more scalable and modular deployments. The server handles requests and
+performs heavy computations, while clients can communicate with the server to
+perform ingestion, search, RAG, and other operations, as shown in the examples
+above. For detailed setup and basic functionality, refer back to the [R2R Demo]
+(#r2r-demo). # Core Abstractions The framework revolves around three core
 abstractions: Providers, Pipes, and Pipelines. ## Providers Providers supply
 the necessary resources and capabilities to the pipes and pipelines. Key
 provider types include: - **Vector Database Provider**: Manages the storage and
 retrieval of vector embeddings. Examples include Qdrant, PGVector, and
 LocalVectorDB. - **Embedding Provider**: Converts text into vector embeddings.
 Supported providers include OpenAI, SentenceTransformers, and
 DummyEmbeddingProvider. - **LLM Provider**: Interfaces with large language
```

