# Comparing `tmp/langfun-0.0.2.dev20240531.tar.gz` & `tmp/langfun-0.0.2.dev20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240531.tar", last modified: Fri May 31 08:04:22 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240601.tar", last modified: Sat Jun  1 08:03:48 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240531.tar` & `langfun-0.0.2.dev20240601.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.482950 langfun-0.0.2.dev20240531/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.486950 langfun-0.0.2.dev20240531/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.486950 langfun-0.0.2.dev20240531/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.490950 langfun-0.0.2.dev20240531/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.490950 langfun-0.0.2.dev20240531/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.494950 langfun-0.0.2.dev20240531/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/audio_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office.py
--rw-r--r--   0 runner    (1001) docker     (127)    85434 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/pdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.498950 langfun-0.0.2.dev20240531/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 08:04:22.000000 langfun-0.0.2.dev20240531/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:04:22.502950 langfun-0.0.2.dev20240531/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-31 08:03:41.000000 langfun-0.0.2.dev20240531/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.966538 langfun-0.0.2.dev20240601/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-01 08:03:48.966538 langfun-0.0.2.dev20240601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.946538 langfun-0.0.2.dev20240601/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.950538 langfun-0.0.2.dev20240601/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.950538 langfun-0.0.2.dev20240601/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.954538 langfun-0.0.2.dev20240601/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.954538 langfun-0.0.2.dev20240601/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.958538 langfun-0.0.2.dev20240601/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.958538 langfun-0.0.2.dev20240601/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.958538 langfun-0.0.2.dev20240601/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.958538 langfun-0.0.2.dev20240601/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/audio_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/ms_office.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87866 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/ms_office_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/pdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.962538 langfun-0.0.2.dev20240601/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27664 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.966538 langfun-0.0.2.dev20240601/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:03:48.966538 langfun-0.0.2.dev20240601/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-06-01 08:03:48.000000 langfun-0.0.2.dev20240601/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-06-01 08:03:48.000000 langfun-0.0.2.dev20240601/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:03:48.000000 langfun-0.0.2.dev20240601/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-01 08:03:48.000000 langfun-0.0.2.dev20240601/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-01 08:03:48.000000 langfun-0.0.2.dev20240601/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 08:03:48.966538 langfun-0.0.2.dev20240601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-06-01 08:03:07.000000 langfun-0.0.2.dev20240601/setup.py
```

### Comparing `langfun-0.0.2.dev20240531/LICENSE` & `langfun-0.0.2.dev20240601/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/PKG-INFO` & `langfun-0.0.2.dev20240601/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240531
+Version: 0.0.2.dev20240601
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -21,21 +21,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-aiplatform>=1.5.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
+Requires-Dist: openpyxl>=3.1.0
+Requires-Dist: pandas>=2.1.4
 Requires-Dist: pyglove>=0.4.5.dev20240423
+Requires-Dist: python-docx>=0.8.11
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: python-docx>=0.8.11
-Requires-Dist: pandas>=2.1.4
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/google/langfun/main/docs/_static/logo.svg" width="520px" alt="logo"></img>
 </div>
 
 # Langfun
```

### Comparing `langfun-0.0.2.dev20240531/README.md` & `langfun-0.0.2.dev20240601/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/__init__.py` & `langfun-0.0.2.dev20240601/langfun/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,16 @@
 from langfun.core import llms
 lm_cache = llms.cache.lm_cache
 
 from langfun.core import memories
 
 from langfun.core import modalities
 
+Mime = modalities.Mime
+MimeType = Mime  # For backwards compatibility.
 Image = modalities.Image
 Video = modalities.Video
 PDF = modalities.PDF
 
 # Error types.
 MappingError = structured.MappingError
 SchemaError = structured.SchemaError
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 from langfun.core.message import AIMessage
 from langfun.core.message import SystemMessage
 from langfun.core.message import MemoryRecord
 
 # Interface for modality.
 from langfun.core.modality import Modality
 from langfun.core.modality import ModalityRef
+from langfun.core.modality import ModalityError
 
 # Interfaces for languge models.
 from langfun.core.language_model import LanguageModel
 from langfun.core.language_model import LMSample
 from langfun.core.language_model import LMSamplingOptions
 from langfun.core.language_model import LMSamplingUsage
 from langfun.core.language_model import LMSamplingResult
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240601/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/component.py` & `langfun-0.0.2.dev20240601/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/component_test.py` & `langfun-0.0.2.dev20240601/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240601/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240601/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/console.py` & `langfun-0.0.2.dev20240601/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/console_test.py` & `langfun-0.0.2.dev20240601/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240601/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240601/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240601/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/language_model.py` & `langfun-0.0.2.dev20240601/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240601/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/google_genai.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,17 +45,18 @@
       (
           'API key. If None, the key will be read from environment variable '
           "'GOOGLE_API_KEY'. "
           'Get an API key at https://ai.google.dev/tutorials/setup'
       ),
   ] = None
 
-  multimodal: Annotated[bool, 'Whether this model has multimodal support.'] = (
-      False
-  )
+  supported_modalities: Annotated[
+      list[str],
+      'A list of MIME types for supported modalities'
+  ] = []
 
   # Set the default max concurrency to 8 workers.
   max_concurrency = 8
 
   def _on_bound(self):
     super()._on_bound()
     self.__dict__.pop('_api_initialized', None)
@@ -114,22 +115,35 @@
     """Gets Evergreen formatted content from langfun message."""
     formatted = lf.UserMessage(prompt.text)
     formatted.source = prompt
 
     chunks = []
     for lf_chunk in formatted.chunk():
       if isinstance(lf_chunk, str):
-        chunk = lf_chunk
-      elif self.multimodal and isinstance(lf_chunk, lf_modalities.MimeType):
-        chunk = genai.types.BlobDict(
-            data=lf_chunk.to_bytes(), mime_type=lf_chunk.mime_type
-        )
+        chunks.append(lf_chunk)
+      elif isinstance(lf_chunk, lf_modalities.Mime):
+        try:
+          modalities = lf_chunk.make_compatible(
+              self.supported_modalities + ['text/plain']
+          )
+          if isinstance(modalities, lf_modalities.Mime):
+            modalities = [modalities]
+          for modality in modalities:
+            if modality.is_text:
+              chunk = modality.to_text()
+            else:
+              chunk = genai.types.BlobDict(
+                  data=modality.to_bytes(),
+                  mime_type=modality.mime_type
+              )
+            chunks.append(chunk)
+        except lf.ModalityError as e:
+          raise lf.ModalityError(f'Unsupported modality: {lf_chunk!r}') from e
       else:
-        raise ValueError(f'Unsupported modality: {lf_chunk!r}')
-      chunks.append(chunk)
+        raise lf.ModalityError(f'Unsupported modality: {lf_chunk!r}')
     return chunks
 
   def _response_to_result(
       self, response: genai.types.GenerateContentResponse | pg.Dict
   ) -> lf.LMSamplingResult:
     """Parses generative response into message."""
     samples = []
@@ -260,39 +274,78 @@
 
 
 #
 # Public Gemini models.
 #
 
 
+_IMAGE_TYPES = [
+    'image/png',
+    'image/jpeg',
+    'image/webp',
+    'image/heic',
+    'image/heif',
+]
+
+_AUDIO_TYPES = [
+    'audio/aac',
+    'audio/flac',
+    'audio/mp3',
+    'audio/m4a',
+    'audio/mpeg',
+    'audio/mpga',
+    'audio/mp4',
+    'audio/opus',
+    'audio/pcm',
+    'audio/wav',
+    'audio/webm'
+]
+
+_VIDEO_TYPES = [
+    'video/mov',
+    'video/mpeg',
+    'video/mpegps',
+    'video/mpg',
+    'video/mp4',
+    'video/webm',
+    'video/wmv',
+    'video/x-flv',
+    'video/3gpp',
+]
+
+_PDF = [
+    'application/pdf',
+]
+
+
 class GeminiPro1_5(GenAI):  # pylint: disable=invalid-name
   """Gemini Pro latest model."""
 
   model = 'gemini-1.5-pro-latest'
-  multimodal = True
+  supported_modalities = _PDF + _IMAGE_TYPES + _AUDIO_TYPES + _VIDEO_TYPES
 
 
 class GeminiFlash1_5(GenAI):  # pylint: disable=invalid-name
   """Gemini Flash latest model."""
 
   model = 'gemini-1.5-flash-latest'
-  multimodal = True
+  supported_modalities = _PDF + _IMAGE_TYPES + _AUDIO_TYPES + _VIDEO_TYPES
 
 
 class GeminiPro(GenAI):
   """Gemini Pro model."""
 
   model = 'gemini-pro'
 
 
 class GeminiProVision(GenAI):
   """Gemini Pro vision model."""
 
   model = 'gemini-pro-vision'
-  multimodal = True
+  supported_modalities = _IMAGE_TYPES + _VIDEO_TYPES
 
 
 class Palm2(GenAI):
   """PaLM2 model."""
 
   model = 'text-bison-001'
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/google_genai_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
   def test_content_from_message_mm(self):
     message = lf.UserMessage(
         'This is an <<[[image]]>>, what is it?',
         image=lf_modalities.Image.from_bytes(example_image),
     )
 
     # Non-multimodal model.
-    with self.assertRaisesRegex(ValueError, 'Unsupported modality'):
+    with self.assertRaisesRegex(lf.ModalityError, 'Unsupported modality'):
       google_genai.GeminiPro()._content_from_message(message)
 
     model = google_genai.GeminiProVision()
     chunks = model._content_from_message(message)
     self.maxDiff = None
     self.assertEqual(
         chunks,
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/vertexai.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,17 +71,18 @@
       credentials_lib.Credentials | None,
       (
           'Credentials to use. If None, the default credentials to the '
           'environment will be used.'
       ),
   ] = None
 
-  multimodal: Annotated[bool, 'Whether this model has multimodal support.'] = (
-      False
-  )
+  supported_modalities: Annotated[
+      list[str],
+      'A list of MIME types for supported modalities'
+  ] = []
 
   def _on_bound(self):
     super()._on_bound()
     self.__dict__.pop('_api_initialized', None)
 
   @functools.cached_property
   def _api_initialized(self):
@@ -138,24 +139,37 @@
 
   def _content_from_message(
       self, prompt: lf.Message
   ) -> list[str | Any]:
     """Gets generation input from langfun message."""
     from vertexai import generative_models
     chunks = []
+
     for lf_chunk in prompt.chunk():
       if isinstance(lf_chunk, str):
-        chunk = lf_chunk
-      elif self.multimodal and isinstance(lf_chunk, lf_modalities.MimeType):
-        chunk = generative_models.Part.from_data(
-            lf_chunk.to_bytes(), lf_chunk.mime_type
-        )
+        chunks.append(lf_chunk)
+      elif isinstance(lf_chunk, lf_modalities.Mime):
+        try:
+          modalities = lf_chunk.make_compatible(
+              self.supported_modalities + ['text/plain']
+          )
+          if isinstance(modalities, lf_modalities.Mime):
+            modalities = [modalities]
+          for modality in modalities:
+            if modality.is_text:
+              chunk = modality.to_text()
+            else:
+              chunk = generative_models.Part.from_data(
+                  modality.to_bytes(), modality.mime_type
+              )
+            chunks.append(chunk)
+        except lf.ModalityError as e:
+          raise lf.ModalityError(f'Unsupported modality: {lf_chunk!r}') from e
       else:
-        raise ValueError(f'Unsupported modality: {lf_chunk!r}')
-      chunks.append(chunk)
+        raise lf.ModalityError(f'Unsupported modality: {lf_chunk!r}')
     return chunks
 
   def _generation_response_to_message(
       self,
       response: Any,  # generative_models.GenerationResponse
   ) -> lf.Message:
     """Parses generative response into message."""
@@ -261,46 +275,85 @@
       self._text_generation_model_cache[model_id] = model
     return model
 
 
 _VERTEXAI_MODEL_HUB = _ModelHub()
 
 
+_IMAGE_TYPES = [
+    'image/png',
+    'image/jpeg',
+    'image/webp',
+    'image/heic',
+    'image/heif',
+]
+
+_AUDIO_TYPES = [
+    'audio/aac',
+    'audio/flac',
+    'audio/mp3',
+    'audio/m4a',
+    'audio/mpeg',
+    'audio/mpga',
+    'audio/mp4',
+    'audio/opus',
+    'audio/pcm',
+    'audio/wav',
+    'audio/webm'
+]
+
+_VIDEO_TYPES = [
+    'video/mov',
+    'video/mpeg',
+    'video/mpegps',
+    'video/mpg',
+    'video/mp4',
+    'video/webm',
+    'video/wmv',
+    'video/x-flv',
+    'video/3gpp',
+]
+
+_PDF = [
+    'application/pdf',
+]
+
+
 class VertexAIGeminiPro1_5(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Pro model."""
 
   model = 'gemini-1.5-pro-preview-0514'
-  multimodal = True
+  supported_modalities = _PDF + _IMAGE_TYPES + _AUDIO_TYPES + _VIDEO_TYPES
 
 
 class VertexAIGeminiPro1_5_0409(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Pro model."""
 
   model = 'gemini-1.5-pro-preview-0409'
-  multimodal = True
+  supported_modalities = _PDF + _IMAGE_TYPES + _AUDIO_TYPES + _VIDEO_TYPES
 
 
 class VertexAIGeminiFlash1_5(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Flash model."""
 
   model = 'gemini-1.5-flash-preview-0514'
-  multimodal = True
+  supported_modalities = _PDF + _IMAGE_TYPES + _AUDIO_TYPES + _VIDEO_TYPES
 
 
 class VertexAIGeminiPro1(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.0 Pro model."""
 
   model = 'gemini-1.0-pro'
 
 
 class VertexAIGeminiPro1Vision(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.0 Pro model."""
 
   model = 'gemini-1.0-pro-vision'
-  multimodal = True
+  supported_modalities = _IMAGE_TYPES + _VIDEO_TYPES
 
 
 class VertexAIPalm2(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI PaLM2 text generation model."""
 
   model = 'text-bison'
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240601/langfun/core/llms/vertexai_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
   def test_content_from_message_mm(self):
     message = lf.UserMessage(
         'This is an <<[[image]]>>, what is it?',
         image=lf_modalities.Image.from_bytes(example_image),
     )
 
     # Non-multimodal model.
-    with self.assertRaisesRegex(ValueError, 'Unsupported modality'):
+    with self.assertRaisesRegex(lf.ModalityError, 'Unsupported modality'):
       vertexai.VertexAIGeminiPro1()._content_from_message(message)
 
     model = vertexai.VertexAIGeminiPro1Vision()
     chunks = model._content_from_message(message)
     self.maxDiff = None
     self.assertEqual([chunks[0], chunks[2]], ['This is an', ', what is it?'])
     self.assertIsInstance(chunks[1], generative_models.Part)
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240601/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240601/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/memory.py` & `langfun-0.0.2.dev20240601/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/message.py` & `langfun-0.0.2.dev20240601/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/message_test.py` & `langfun-0.0.2.dev20240601/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Modalities for LLM."""
 
 # pylint: disable=g-importing-member
 # pylint: disable=g-bad-import-order
 # pylint: disable=g-import-not-at-top
 
 from langfun.core.modalities.audio import Audio
-from langfun.core.modalities.mime import MimeType
+from langfun.core.modalities.mime import Mime
 from langfun.core.modalities.mime import Custom
 from langfun.core.modalities.ms_office import Docx
 from langfun.core.modalities.ms_office import Pptx
 from langfun.core.modalities.ms_office import Xlsx
 from langfun.core.modalities.image import Image
 from langfun.core.modalities.pdf import PDF
 from langfun.core.modalities.video import Video
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/audio.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/video.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2024 The Langfun Authors
+# Copyright 2023 The Langfun Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Audio types."""
+"""Video modality."""
 
 import functools
 from langfun.core.modalities import mime
 
 
-class Audio(mime.MimeType):
-  """Audio."""
+class Video(mime.Mime):
+  """Video."""
 
-  MIME_PREFIX = 'audio'
+  MIME_PREFIX = 'video'
 
   @functools.cached_property
-  def audio_format(self) -> str:
+  def video_format(self) -> str:
     return self.mime_type.removeprefix(self.MIME_PREFIX + '/')
 
   def _html(self, uri: str) -> str:
-    return f'<audio controls> <source src="{uri}"> </audio>'
+    return f'<video controls> <source src="{uri}"> </video>'
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/audio_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/audio_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Image modality."""
 
 import functools
 from langfun.core.modalities import mime
 
 
-class Image(mime.MimeType):
+class Image(mime.Mime):
   """Image."""
 
   MIME_PREFIX = 'image'
 
   @functools.cached_property
   def image_format(self) -> str:
     return self.mime_type.removeprefix(self.MIME_PREFIX + '/')
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/image_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Image tests."""
 import unittest
 from unittest import mock
 
+import langfun.core as lf
 from langfun.core.modalities import image as image_lib
+from langfun.core.modalities import mime as mime_lib
 import pyglove as pg
 
 
 image_content = (
     b'\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR\x00\x00\x00\x18\x00\x00\x00\x18\x04'
     b'\x03\x00\x00\x00\x12Y \xcb\x00\x00\x00\x18PLTE\x00\x00'
     b'\x00fff_chaag_cg_ch^ci_ciC\xedb\x94\x00\x00\x00\x08tRNS'
@@ -32,34 +34,49 @@
 
 
 def mock_request(*args, **kwargs):
   del args, kwargs
   return pg.Dict(content=image_content)
 
 
-class ImageContentTest(unittest.TestCase):
+class ImageTest(unittest.TestCase):
 
-  def test_image_content(self):
+  def test_from_bytes(self):
     image = image_lib.Image.from_bytes(image_content)
     self.assertEqual(image.image_format, 'png')
     self.assertIn('data:image/png;base64,', image._repr_html_())
     self.assertEqual(image.to_bytes(), image_content)
+    with self.assertRaisesRegex(
+        lf.ModalityError, '.* cannot be converted to text'
+    ):
+      image.to_text()
 
-  def test_bad_image(self):
+  def test_from_bytes_invalid(self):
     image = image_lib.Image.from_bytes(b'bad')
     with self.assertRaisesRegex(ValueError, 'Expected MIME type'):
       _ = image.image_format
 
+  def test_from_bytes_base_cls(self):
+    self.assertIsInstance(
+        mime_lib.Mime.from_bytes(image_content), image_lib.Image
+    )
 
-class ImageFileTest(unittest.TestCase):
-
-  def test_image_file(self):
+  def test_from_uri(self):
     image = image_lib.Image.from_uri('http://mock/web/a.png')
     with mock.patch('requests.get') as mock_requests_get:
       mock_requests_get.side_effect = mock_request
       self.assertEqual(image.image_format, 'png')
       self.assertEqual(image._repr_html_(), '<img src="http://mock/web/a.png">')
       self.assertEqual(image.to_bytes(), image_content)
 
+  def test_from_uri_base_cls(self):
+    with mock.patch('requests.get') as mock_requests_get:
+      mock_requests_get.side_effect = mock_request
+      image = mime_lib.Mime.from_uri('http://mock/web/a.png')
+      self.assertIsInstance(image, image_lib.Image)
+      self.assertEqual(image.image_format, 'png')
+      self.assertEqual(image._repr_html_(), '<img src="http://mock/web/a.png">')
+      self.assertEqual(image.to_bytes(), image_content)
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/ms_office.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,96 +7,105 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""MIME type data."""
+"""Microsoft Office file types."""
 
 import base64
-import functools
-from typing import Annotated, Union
-import langfun.core as lf
-import magic
-import pyglove as pg
+import io
+import os
+from typing import Iterable
+from langfun.core.modalities import mime
+from langfun.core.modalities import pdf
 import requests
 
 
-class MimeType(lf.Modality):
-  """Base for MIME type data."""
+class Xlsx(mime.Mime):
+  """Xlsx file type."""
 
-  # The regular expression that describes the MIME type str.
-  # If None, the MIME type is dynamic. Subclass could override.
-  MIME_PREFIX = None
-
-  uri: Annotated[str | None, 'The URI for locating the MIME data. '] = None
-
-  content: Annotated[
-      Union[str, bytes, None], 'The raw content of the MIME type.'
-  ] = None
-
-  @functools.cached_property
-  def mime_type(self) -> str:
-    """Returns the MIME type."""
-    mime = magic.from_buffer((self.to_bytes()), mime=True)
-    if self.MIME_PREFIX and not mime.lower().startswith(self.MIME_PREFIX):
-      raise ValueError(
-          f'Expected MIME type: {self.MIME_PREFIX}, Encountered: {mime}'
-      )
-    return mime
-
-  def _on_bound(self):
-    super()._on_bound()
-    if self.uri is None and self.content is None:
-      raise ValueError('Either uri or content must be provided.')
-
-  def to_bytes(self) -> bytes:
-    if self.content is not None:
-      return self.content
-
-    assert self.uri is not None
-    if self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
-      content = requests.get(
-          self.uri,
-          headers={'User-Agent': 'Langfun'},
-      ).content
-    else:
-      content = pg.io.readfile(self.uri, mode='rb')
-    self.rebind(content=content, skip_notification=True)
-    return self.content
-
-  @property
-  def content_uri(self) -> str:
-    base64_content = base64.b64encode(self.to_bytes()).decode()
-    return f'data:{self.mime_type};base64,{base64_content}'
-
-  @classmethod
-  def from_uri(cls, uri: str, **kwargs) -> 'MimeType':
-    return cls(uri=uri, content=None, **kwargs)
-
-  @classmethod
-  def from_bytes(cls, content: bytes | str, **kwargs) -> 'MimeType':
-    return cls(content=content, **kwargs)
+  MIME_PREFIX = (
+      'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
+  )
+
+  def to_html(self) -> str:
+    import pandas as pd  # pylint: disable=g-import-not-at-top
+
+    df = pd.read_excel(io.BytesIO(self.to_bytes()))
+    return df.to_html()
+
+  def _repr_html_(self) -> str:
+    return self.to_html()
+
+  def _is_compatible(self, mime_types: Iterable[str]) -> bool:
+    return bool(set(mime_types).intersection([
+        'text/html',
+        'text/plain',
+    ]))
+
+  def _make_compatible(self, mime_types: Iterable[str]) -> mime.Mime:
+    """Returns the MimeType of the converted file."""
+    del mime_types
+    return mime.Mime(uri=self.uri, content=self.to_html())
+
+
+class Docx(mime.Mime):
+  """Docx file type."""
+
+  MIME_PREFIX = (
+      'application/vnd.openxmlformats-officedocument.wordprocessingml.document'
+  )
+
+  def to_xml(self) -> str:
+    import docx  # pylint: disable=g-import-not-at-top
+
+    doc = docx.Document(io.BytesIO(self.to_bytes()))
+    return str(doc.element.xml)
 
   def _repr_html_(self) -> str:
-    if self.uri and self.uri.lower().startswith(('http:', 'https:', 'ftp:')):
-      uri = self.uri
-    else:
-      uri = self.content_uri
-    return self._html(uri)
-
-  def _html(self, uri) -> str:
-    return f'<embed type="{self.mime_type}" src="{uri}"/>'
-
-
-@pg.use_init_args(['mime', 'content', 'uri'])
-class Custom(MimeType):
-  """Custom MIME data."""
-
-  mime: Annotated[
-      str, 'The MIME type of the data. E.g. text/plain, or image/png. '
-  ]
-
-  @property
-  def mime_type(self) -> str:
-    return self.mime
+    return self.to_xml()
+
+  def _is_compatible(self, mime_types: Iterable[str]) -> bool:
+    return bool(set(mime_types).intersection([
+        'application/xml',
+        'text/xml',
+        'text/plain',
+    ]))
+
+  def _make_compatible(self, mime_types: Iterable[str]) -> mime.Mime:
+    """Returns the MimeType of the converted file."""
+    del mime_types
+    return mime.Mime(uri=self.uri, content=self.to_xml())
+
+
+class Pptx(mime.Mime):
+  """Pptx file type."""
+
+  MIME_PREFIX = 'application/vnd.openxmlformats-officedocument.presentationml.presentation'
+  API_URL = 'https://v2.convertapi.com/convert/pptx/to/pdf'
+
+  def to_pdf(self, convert_api_key: str | None = None) -> pdf.PDF:
+    api_key = convert_api_key or os.environ.get('CONVERT_API_KEY')
+    url = f'{self.API_URL}?Secret={api_key}'
+
+    json = {
+        'Parameters': [{
+            'Name': 'File',
+            'FileValue': {
+                'Name': os.path.basename(self.uri) if self.uri else 'tmp.pptx',
+                'Data': base64.b64encode(self.to_bytes()).decode('utf-8'),
+            },
+        }]
+    }
+    response = requests.post(url, json=json).json()
+    base64_pdf = response['Files'][0]['FileData']
+    return pdf.PDF.from_bytes(base64.b64decode(base64_pdf))
+
+  def _is_compatible(self, mime_types: Iterable[str]) -> bool:
+    return 'application/pdf' in mime_types
+
+  def _make_compatible(self, mime_types: Iterable[str]) -> mime.Mime:
+    """Returns the MimeType of the converted file."""
+    del mime_types
+    return self.to_pdf()
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/mime_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """MIME tests."""
 import unittest
 from unittest import mock
 
+import langfun.core as lf
 from langfun.core.modalities import mime
 import pyglove as pg
 
 
 def mock_request(*args, **kwargs):
   del args, kwargs
   return pg.Dict(content='foo')
@@ -27,18 +28,32 @@
 def mock_readfile(*args, **kwargs):
   del args, kwargs
   return 'bar'
 
 
 class CustomMimeTest(unittest.TestCase):
 
-  def test_content(self):
-    content = mime.Custom('text/plain', 'foo')
-    self.assertEqual(content.to_bytes(), 'foo')
+  def test_from_byes(self):
+    content = mime.Mime.from_bytes(b'hello')
+    self.assertIs(content.__class__, mime.Mime)
+
+    content = mime.Custom('text/plain', b'foo')
+    self.assertEqual(content.to_bytes(), b'foo')
     self.assertEqual(content.mime_type, 'text/plain')
+    self.assertTrue(content.is_text)
+    self.assertFalse(content.is_binary)
+    self.assertEqual(content.to_text(), 'foo')
+    self.assertTrue(content.is_compatible('text/plain'))
+    self.assertFalse(content.is_compatible('text/xml'))
+    self.assertIs(content.make_compatible('text/plain'), content)
+
+    with self.assertRaisesRegex(
+        lf.ModalityError, '.* cannot be converted to supported types'
+    ):
+      content.make_compatible('application/pdf')
 
     with self.assertRaisesRegex(
         ValueError, 'Either uri or content must be provided.'
     ):
       mime.Custom('text/plain')
 
   def test_from_uri(self):
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/ms_office_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/ms_office_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Video tests."""
+import base64
 import io
 import unittest
 from unittest import mock
 
 from langfun.core.modalities import ms_office as ms_office_lib
+from langfun.core.modalities import pdf as pdf_lib
 import pyglove as pg
 
 
 def sample_docx_bytes():
   import docx  # pylint: disable=g-import-not-at-top
 
   # Create a new Document
@@ -239,74 +241,149 @@
 
 
 def pptx_mock_request(*args, **kwargs):
   del args, kwargs
   return pg.Dict(content=pptx_bytes)
 
 
+pdf_bytes = (
+    b'%PDF-1.1\n%\xc2\xa5\xc2\xb1\xc3\xab\n\n1 0 obj\n'
+    b'<< /Type /Catalog\n     /Pages 2 0 R\n  >>\nendobj\n\n2 0 obj\n '
+    b'<< /Type /Pages\n     /Kids [3 0 R]\n     '
+    b'/Count 1\n     /MediaBox [0 0 300 144]\n  '
+    b'>>\nendobj\n\n3 0 obj\n  '
+    b'<<  /Type /Page\n      /Parent 2 0 R\n      /Resources\n       '
+    b'<< /Font\n'
+    b'<< /F1\n'
+    b'<< /Type /Font\n'
+    b'/Subtype /Type1\n'
+    b'/BaseFont /Times-Roman\n'
+    b'>>\n>>\n>>\n      '
+    b'/Contents 4 0 R\n  >>\nendobj\n\n4 0 obj\n  '
+    b'<< /Length 55 >>\nstream\n  BT\n    /F1 18 Tf\n    0 0 Td\n    '
+    b'(Hello World) Tj\n  ET\nendstream\nendobj\n\nxref\n0 5\n0000000000 '
+    b'65535 f \n0000000018 00000 n \n0000000077 00000 n \n0000000178 00000 n '
+    b'\n0000000457 00000 n \ntrailer\n  <<  /Root 1 0 R\n      /Size 5\n  '
+    b'>>\nstartxref\n565\n%%EOF\n'
+)
+
+
+def convert_mock_request(*args, **kwargs):
+  del args, kwargs
+
+  class Result:
+    def json(self):
+      return {
+          'Files': [
+              {
+                  'FileData': base64.b64encode(pdf_bytes).decode()
+              }
+          ]
+      }
+  return Result()
+
+
 class DocxTest(unittest.TestCase):
 
-  def test_content(self):
+  def test_from_bytes(self):
     content = ms_office_lib.Docx.from_bytes(docx_bytes)
-    self.assertEqual(
+    self.assertIn(
         content.mime_type,
-        'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+        (
+            'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+            'application/octet-stream',
+        ),
     )
     self.assertEqual(content.to_bytes(), docx_bytes)
+    self.assertTrue(content.is_compatible('text/plain'))
+    self.assertFalse(content.is_compatible('application/pdf'))
+    self.assertEqual(
+        content.make_compatible(['image/png', 'text/plain']).mime_type,
+        'text/plain'
+    )
 
-  def test_file(self):
+  def test_from_uri(self):
     content = ms_office_lib.Docx.from_uri('http://mock/web/a.docx')
     with mock.patch('requests.get') as mock_requests_get:
       mock_requests_get.side_effect = docx_mock_request
-      self.assertEqual(
+      self.assertIn(
           content.mime_type,
-          'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+          (
+              'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
+              'application/octet-stream',
+          ),
       )
       self.assertEqual(content.to_bytes(), docx_bytes)
       self.assertEqual(content.to_xml(), expected_docx_xml)
 
 
 class XlsxTest(unittest.TestCase):
 
-  def test_content(self):
+  def test_from_bytes(self):
     content = ms_office_lib.Xlsx.from_bytes(xlsx_bytes)
-    self.assertEqual(
+    self.assertIn(
         content.mime_type,
-        'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
+        (
+            'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
+            'application/octet-stream',
+        ),
     )
     self.assertEqual(content.to_bytes(), xlsx_bytes)
+    self.assertTrue(content.is_compatible('text/plain'))
+    self.assertFalse(content.is_compatible('application/pdf'))
+    self.assertEqual(
+        content.make_compatible('text/plain').mime_type,
+        'text/html'
+    )
 
-  def test_file(self):
+  def test_from_uri(self):
     content = ms_office_lib.Xlsx.from_uri('http://mock/web/a.xlsx')
     with mock.patch('requests.get') as mock_requests_get:
       mock_requests_get.side_effect = xlsx_mock_request
-      self.assertEqual(
+      self.assertIn(
           content.mime_type,
-          'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
+          (
+              'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet',
+              'application/octet-stream',
+          ),
       )
       self.assertEqual(content.to_bytes(), xlsx_bytes)
       self.assertEqual(content.to_html(), expected_xlsx_html)
 
 
 class PptxTest(unittest.TestCase):
 
   def test_content(self):
     content = ms_office_lib.Pptx.from_bytes(pptx_bytes)
-    self.assertEqual(
+    self.assertIn(
         content.mime_type,
-        'application/vnd.openxmlformats-officedocument.presentationml.presentation',
+        (
+            'application/vnd.openxmlformats-officedocument.presentationml.presentation',
+            'application/octet-stream',
+        ),
     )
     self.assertEqual(content.to_bytes(), pptx_bytes)
 
   def test_file(self):
     content = ms_office_lib.Pptx.from_uri('http://mock/web/a.pptx')
+    self.assertFalse(content.is_compatible('text/plain'))
+    self.assertTrue(content.is_compatible('application/pdf'))
     with mock.patch('requests.get') as mock_requests_get:
       mock_requests_get.side_effect = pptx_mock_request
-      self.assertEqual(
+      self.assertIn(
           content.mime_type,
-          'application/vnd.openxmlformats-officedocument.presentationml.presentation',
+          (
+              'application/vnd.openxmlformats-officedocument.presentationml.presentation',
+              'application/octet-stream',
+          ),
       )
       self.assertEqual(content.to_bytes(), pptx_bytes)
 
+    with mock.patch('requests.post') as mock_requests_post:
+      mock_requests_post.side_effect = convert_mock_request
+      self.assertIsInstance(
+          content.make_compatible('application/pdf'), pdf_lib.PDF
+      )
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/pdf.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """PDF modality."""
 
 from langfun.core.modalities import mime
 
 
-class PDF(mime.MimeType):
+class PDF(mime.Mime):
   """PDF document."""
 
   MIME_PREFIX = 'application/pdf'
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/pdf_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/pdf_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/audio.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Copyright 2023 The Langfun Authors
+# Copyright 2024 The Langfun Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Video modality."""
+"""Audio types."""
 
 import functools
 from langfun.core.modalities import mime
 
 
-class Video(mime.MimeType):
-  """Video."""
+class Audio(mime.Mime):
+  """Audio."""
 
-  MIME_PREFIX = 'video'
+  MIME_PREFIX = 'audio'
 
   @functools.cached_property
-  def video_format(self) -> str:
+  def audio_format(self) -> str:
     return self.mime_type.removeprefix(self.MIME_PREFIX + '/')
 
   def _html(self, uri: str) -> str:
-    return f'<video controls> <source src="{uri}"> </video>'
+    return f'<audio controls> <source src="{uri}"> </audio>'
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modality.py` & `langfun-0.0.2.dev20240601/langfun/core/modality.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,7 +104,11 @@
 
     def _placehold(k, v, p):
       del p
       if isinstance(v, Modality):
         return ModalityRef(name=value.sym_path + k)
       return v
     return value.clone().rebind(_placehold, raise_on_no_change=False)
+
+
+class ModalityError(RuntimeError):  # pylint: disable=g-bad-exception-name
+  """Exception raised when modality is not supported."""
```

### Comparing `langfun-0.0.2.dev20240531/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240601/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240601/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240601/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/sampling.py` & `langfun-0.0.2.dev20240601/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240601/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240601/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/subscription.py` & `langfun-0.0.2.dev20240601/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240601/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/template.py` & `langfun-0.0.2.dev20240601/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/template_test.py` & `langfun-0.0.2.dev20240601/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240601/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240601/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240601/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240601/langfun.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240531
+Version: 0.0.2.dev20240601
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -21,21 +21,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: google-cloud-aiplatform>=1.5.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
+Requires-Dist: openpyxl>=3.1.0
+Requires-Dist: pandas>=2.1.4
 Requires-Dist: pyglove>=0.4.5.dev20240423
+Requires-Dist: python-docx>=0.8.11
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: python-docx>=0.8.11
-Requires-Dist: pandas>=2.1.4
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/google/langfun/main/docs/_static/logo.svg" width="520px" alt="logo"></img>
 </div>
 
 # Langfun
```

### Comparing `langfun-0.0.2.dev20240531/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240601/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240531/setup.py` & `langfun-0.0.2.dev20240601/setup.py`

 * *Files identical despite different names*

