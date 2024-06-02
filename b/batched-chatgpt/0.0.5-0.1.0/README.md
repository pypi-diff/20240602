# Comparing `tmp/batched_chatgpt-0.0.5.tar.gz` & `tmp/batched_chatgpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batched_chatgpt-0.0.5.tar", last modified: Sun Mar 24 11:29:37 2024, max compression
+gzip compressed data, was "batched_chatgpt-0.1.0.tar", last modified: Sun Jun  2 11:12:55 2024, max compression
```

## Comparing `batched_chatgpt-0.0.5.tar` & `batched_chatgpt-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 11:29:37.787624 batched_chatgpt-0.0.5/
--rw-rw-rw-   0        0        0      178 2024-03-24 11:29:37.786627 batched_chatgpt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2217 2024-03-24 11:14:54.000000 batched_chatgpt-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 11:29:37.762720 batched_chatgpt-0.0.5/batched_chatgpt/
--rw-rw-rw-   0        0        0       63 2024-03-24 11:14:54.000000 batched_chatgpt-0.0.5/batched_chatgpt/__init__.py
--rw-rw-rw-   0        0        0     5292 2024-03-24 11:27:31.000000 batched_chatgpt-0.0.5/batched_chatgpt/chatgpt_utils.py
--rw-rw-rw-   0        0        0     1444 2024-03-13 13:41:23.000000 batched_chatgpt-0.0.5/batched_chatgpt/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-24 11:29:37.785629 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/
--rw-rw-rw-   0        0        0      178 2024-03-24 11:29:37.000000 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-03-24 11:29:37.000000 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 11:29:37.000000 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-24 11:29:37.000000 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-24 11:29:37.000000 batched_chatgpt-0.0.5/batched_chatgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 11:29:37.788621 batched_chatgpt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-03-24 11:14:54.000000 batched_chatgpt-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:12:55.186064 batched_chatgpt-0.1.0/
+-rw-rw-rw-   0        0        0      178 2024-06-02 11:12:55.185094 batched_chatgpt-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2217 2024-03-24 11:54:33.000000 batched_chatgpt-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-02 11:12:55.159868 batched_chatgpt-0.1.0/batched_chatgpt/
+-rw-rw-rw-   0        0        0       63 2024-06-02 11:09:04.000000 batched_chatgpt-0.1.0/batched_chatgpt/__init__.py
+-rw-rw-rw-   0        0        0     5458 2024-06-02 11:09:04.000000 batched_chatgpt-0.1.0/batched_chatgpt/chatgpt_utils.py
+-rw-rw-rw-   0        0        0     1444 2024-03-13 13:41:23.000000 batched_chatgpt-0.1.0/batched_chatgpt/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-02 11:12:55.183101 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/
+-rw-rw-rw-   0        0        0      178 2024-06-02 11:12:54.000000 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-06-02 11:12:55.000000 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 11:12:54.000000 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-06-02 11:12:54.000000 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-06-02 11:12:54.000000 batched_chatgpt-0.1.0/batched_chatgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-02 11:12:55.186064 batched_chatgpt-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-06-02 11:09:04.000000 batched_chatgpt-0.1.0/setup.py
```

### Comparing `batched_chatgpt-0.0.5/README.md` & `batched_chatgpt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `batched_chatgpt-0.0.5/batched_chatgpt/chatgpt_utils.py` & `batched_chatgpt-0.1.0/batched_chatgpt/chatgpt_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,21 @@
 
     timeout-ed output be None"""
     pkl_path = get_saving_filename_safely(pkl_path) if pkl_path else None  # if pkl_path, result saved.
 
     outputs = [None] * len(items)
     c = count()
     while not all(outputs):
+        retry_count = next(c)
+        if retry_count > 0:
+            logger.info("There exists failed API call. Retrying...")
+        # display a warning message if the global retry count exceeds 5.
+        if retry_count >= 5:
+            logger.warning("Retry count has exceeds 5. The process may be stuck due to an unresponsive item.")
+
         # printing remained queries if the number of remained queries is small
         num_of_remains = outputs.count(None)
         print(f"num of remains: {num_of_remains}") if verbose else ...
         if verbose and num_of_remains <= chunk_size:
             pprint(f"printing remains...:\n{[items[i][1].content for i, o in enumerate(outputs) if o is None]}")
 
         remain_inputs = [(i, item) for i, item in enumerate(items) if outputs[i] is None]  # store failed item indices
@@ -82,21 +89,17 @@
         for i, chunk in enumerate(tqdm(chunks, "Batches")):  # tqdm num is the num of chunks
             results = process_chunk(chunk, model_name, temperature, timeout_each)
             results = list(map(lambda x: x.content if x else None, results))
             for j, result in enumerate(results):
                 outputs[remain_indices[i * chunk_size + j]] = result
 
             # save the outputs which may be incomplete
-            pickle_bobj(outputs, pkl_path) if pkl_path else None
+            pickle_bobj({'prompts': items, 'completions': outputs}, pkl_path) if pkl_path else None
 
             time.sleep(sleep_between_chunk) if not all(outputs) else ...
-
-        # display a warning message if the global retry count exceeds 5.
-        if next(c) >= 5:
-            logger.warning("Retry count has exceeds 5. The process may be stuck due to an unresponsive item.")
     return outputs
 
 
 def call_chatgpt(
         human_message: List[str],
         system_message: Union[str, List[str]] = "You're a helpful assistant",
         model_name: str = "gpt-3.5-turbo",
```

### Comparing `batched_chatgpt-0.0.5/batched_chatgpt/utils.py` & `batched_chatgpt-0.1.0/batched_chatgpt/utils.py`

 * *Files identical despite different names*

