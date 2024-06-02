# Comparing `tmp/eidolon_ai_sdk-0.1.61.tar.gz` & `tmp/eidolon_ai_sdk-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.61.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.62.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.61.tar` & `eidolon_ai_sdk-0.1.62.tar`

### file list

```diff
@@ -1,147 +1,147 @@
--rw-r--r--   0        0        0      701 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/README.md
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2424 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3850 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2865 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0     1059 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4642 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1399 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0      812 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/document_retriever.py
--rw-r--r--   0        0        0     1428 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2323 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0      781 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/result_summarizer.py
--rw-r--r--   0        0        0     3179 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     4751 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    13376 2024-05-30 15:41:52.307256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1809 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9545 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9508 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1822 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6517 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     3008 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     9128 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     6039 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/apu.py
--rw-r--r--   0        0        0     3790 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14187 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4841 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9490 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3597 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     3099 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4491 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0     5205 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/tool_call_unit.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0     1000 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-30 15:41:52.311256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    23004 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4911 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     7664 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/logging.conf
--rw-r--r--   0        0        0     2214 2024-05-30 15:41:52.315256 eidolon_ai_sdk-0.1.61/pyproject.toml
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.61/PKG-INFO
+-rw-r--r--   0        0        0      701 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2424 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3850 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2865 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0     1059 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4642 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1399 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0      812 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/document_retriever.py
+-rw-r--r--   0        0        0     1428 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2323 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0      781 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/result_summarizer.py
+-rw-r--r--   0        0        0     3179 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     4751 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    13376 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1809 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9545 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9508 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1822 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6517 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     3008 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9377 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     6039 2024-06-02 14:42:49.463829 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/apu.py
+-rw-r--r--   0        0        0     3790 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14187 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4841 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9490 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3597 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     3099 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4664 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0     5205 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/tool_call_unit.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0     1000 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    23004 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     7664 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     7002 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-06-02 14:42:49.467830 eidolon_ai_sdk-0.1.62/logging.conf
+-rw-r--r--   0        0        0     2214 2024-06-02 14:42:49.471830 eidolon_ai_sdk-0.1.62/pyproject.toml
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.62/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.61/README.md` & `eidolon_ai_sdk-0.1.62/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/document_retriever.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/document_retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/result_summarizer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/result_summarizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     async def _get_schema(self, machine: str) -> dict:
         if machine not in self._machine_schemas:
             self._machine_schemas[machine] = await Machine(machine=machine).get_schema()
         return copy.deepcopy(self._machine_schemas[machine])
 
     async def build_action_tool(
-        self, machine: str, agent: str, action: str, allowed_pids: Set[str], call_context: CallContext
+            self, machine: str, agent: str, action: str, allowed_pids: Set[str], call_context: CallContext
     ):
         agent_client = Agent.get(agent)
         path = f"/processes/{{process_id}}/agent/{agent}/actions/{action}"
         machine_schema = await self._get_schema(machine)
         endpoint_schema = machine_schema["paths"][path]["post"]
         try:
             name = self._name(agent, action=action)
@@ -81,14 +81,16 @@
                 action,
                 name,
                 body_schema,
                 description,
                 self._process_tool(agent_client, action, allowed_pids, call_context),
             )
             return tool
+        except _InvalidSchema:
+            logger.warning(f"unable to build tool {path}")
         except ValueError:
             logger.warning(f"unable to build tool {path}", exc_info=True)
 
     async def build_program_tools(self, call_context: CallContext):
         tools = []
         for agent in self.spec.agents:
             agent_client = Agent.get(agent)
@@ -104,14 +106,16 @@
                         action,
                         name,
                         self._body_schema(schema, name),
                         description,
                         self._program_tool(agent_client, action, call_context),
                     )
                     tools.append(tool)
+                except _InvalidSchema:
+                    logger.warning(f"unable to build tool {path}")
                 except ValueError:
                     logger.warning(f"unable to build tool {path}", exc_info=True)
         return tools
 
     def _build_tool_def(self, agent, operation, name, schema, description, tool_call):
         model = schema_to_model(schema, "InputModel")
         return FnHandler(
@@ -135,15 +139,15 @@
             return dict(type="object", properties=dict(body=json_schema))
         elif "application/json" in body["content"]:
             json_schema = body["content"]["application/json"]["schema"]
             return dict(type="object", properties=dict(body=json_schema))
         elif "text/plain" in body["content"]:
             return dict(type="object", properties=dict(body=dict(type="string")))
         else:
-            raise ValueError(f"Agent action at {name} does not support text/plain or application/json")
+            raise _InvalidSchema(f"Agent action at {name} does not support text/plain or application/json")
 
     @staticmethod
     def _description(endpoint_schema, name):
         description = endpoint_schema.get("description", "")
         if not description:
             logger.warning(f"Agent program at {name} does not have a description. LLM may not use it properly")
         return description
@@ -209,7 +213,11 @@
             remote_process_id=self.process_id,
             state=self.state,
             available_actions=self.available_actions,
         )
         await call_data.upsert()
 
         return await super().iteration_complete()
+
+
+class _InvalidSchema(ValueError):
+    pass
```

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/apu.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
+import copy
 import logging
 import typing
 from abc import ABC
 from dataclasses import dataclass
+
+import jsonref
 from pydantic import BaseModel, TypeAdapter
 from typing import Dict, List, AsyncIterator, Coroutine
 
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.llm_unit import LLMCallFunction
 from eidolon_ai_sdk.cpu.processing_unit import ProcessingUnit
 from eidolon_ai_client.events import (
@@ -64,20 +67,24 @@
             for handler in await logic_unit.build_tools(call_context):
                 new_name = logic_unit.__class__.__name__ + "_" + handler.name
                 i = 0
                 while new_name in acc:
                     new_name = logic_unit.__class__.__name__ + "_" + handler.name + "_" + str(i)
                     i += 1
                 input_model = handler.input_model_fn(logic_unit, handler)
+                schema = copy.deepcopy(jsonref.replace_refs(
+                    input_model.model_json_schema(),
+                    jsonschema=True,
+                ))
                 acc[new_name] = LLMToolWrapper(
                     logic_unit=logic_unit,
                     llm_message=LLMCallFunction(
                         name=new_name,
                         description=handler.description(logic_unit, handler),
-                        parameters=input_model.model_json_schema(),
+                        parameters=schema,
                     ),
                     eidolon_handler=handler,
                     input_model=input_model,
                 )
         return acc
```

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/cpu/tool_call_unit.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/cpu/tool_call_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,24 +104,23 @@
                     field.default = None
                 return t, field
 
         try:
             field_type = property_schema.get("type")
             if field_type == "object":
                 # Recursive call for nested object
-                nested_model = schema_to_model(property_schema, f"{model_name}_{property_name.capitalize()}Model")
+                sub_model_name = property_schema.get("title", f"{model_name}_{property_name.capitalize()}Model")
+                nested_model = schema_to_model(property_schema, sub_model_name)
                 fields[property_name] = wrap_optional(nested_model, makeFieldOrDefaultValue())
             elif field_type == "array":
                 # Recursive call for arrays of objects
                 items_schema = property_schema.get("items", {})
                 if isinstance(items_schema, dict) and items_schema.get("type") == "object":
-                    nested_item_model = schema_to_model(
-                        items_schema,
-                        f"{model_name}_{property_name.capitalize()}ItemModel",
-                    )
+                    sub_model_name = property_schema.get("title", f"{model_name}_{property_name.capitalize()}Model")
+                    nested_item_model = schema_to_model(items_schema, sub_model_name)
                     fields[property_name] = wrap_optional(List[nested_item_model], makeFieldOrDefaultValue())
                 else:
                     python_type = get_python_type(property_name, items_schema, str)
                     fields[property_name] = wrap_optional(List[python_type], makeFieldOrDefaultValue())
             else:
                 fields[property_name] = wrap_optional(
                     get_python_type(property_name, property_schema), makeFieldOrDefaultValue()
```

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.62/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/logging.conf` & `eidolon_ai_sdk-0.1.62/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.61/pyproject.toml` & `eidolon_ai_sdk-0.1.62/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.61"
+version = "0.1.62"
 description = "An open source sgent service SDK"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "8985234d9585794364dfe285f0adb9c7ea975035"
+last-update-hash = "fa5ed8e19be7619ea5f19708bcf96307bcc84d3c"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
@@ -57,15 +57,15 @@
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 dill = "^0.3.8"
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
 eidolon-ai-mistralai = "^0.1.6a"
-eidolon-ai-client = "^0.1.22"
+eidolon-ai-client = "^0.1.23"
 eidolon-ai-usage-client = "^0.1.6"
 boto3 = "^1.34.74"
 azure-identity = "^1.16.0"
 playwright = "^1.43.0"
 
 [tool.pytest.ini_options]
 pythonpath = "project"
```

### Comparing `eidolon_ai_sdk-0.1.61/PKG-INFO` & `eidolon_ai_sdk-0.1.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.61
+Version: 0.1.62
 Summary: An open source sgent service SDK
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.74,<2.0.0)
 Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: eidolon-ai-client (>=0.1.22,<0.2.0)
+Requires-Dist: eidolon-ai-client (>=0.1.23,<0.2.0)
 Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.6,<0.2.0)
 Requires-Dist: esprima (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
```

