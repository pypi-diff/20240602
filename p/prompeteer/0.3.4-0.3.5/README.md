# Comparing `tmp/prompeteer-0.3.4.tar.gz` & `tmp/prompeteer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompeteer-0.3.4.tar", last modified: Mon May 20 12:30:11 2024, max compression
+gzip compressed data, was "prompeteer-0.3.5.tar", last modified: Sun Jun  2 11:54:35 2024, max compression
```

## Comparing `prompeteer-0.3.4.tar` & `prompeteer-0.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.919345 prompeteer-0.3.4/
--rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.4/MANIFEST.in
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-20 12:30:11.918977 prompeteer-0.3.4/PKG-INFO
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.910513 prompeteer-0.3.4/prompeteer/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     4142 2024-05-19 11:15:13.000000 prompeteer-0.3.4/prompeteer/prompeteer.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.913238 prompeteer-0.3.4/prompeteer/prompt/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/prompt/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)      673 2024-05-19 12:43:18.000000 prompeteer-0.3.4/prompeteer/prompt/prompt.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3171 2024-05-19 13:02:38.000000 prompeteer-0.3.4/prompeteer/prompt/prompt_config.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.914117 prompeteer-0.3.4/prompeteer/providers/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/providers/__init__.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.915198 prompeteer-0.3.4/prompeteer/providers/aws_bedrock/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/providers/aws_bedrock/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2186 2024-05-20 12:29:31.000000 prompeteer-0.3.4/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1866 2024-05-19 12:41:47.000000 prompeteer-0.3.4/prompeteer/providers/aws_bedrock/aws_llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.916374 prompeteer-0.3.4/prompeteer/providers/azure_openai/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/providers/azure_openai/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     2070 2024-05-19 12:41:18.000000 prompeteer-0.3.4/prompeteer/providers/azure_openai/azure_llm_request.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3074 2024-05-19 13:17:36.000000 prompeteer-0.3.4/prompeteer/providers/azure_openai/azure_openai_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1445 2024-05-19 11:15:13.000000 prompeteer-0.3.4/prompeteer/providers/llm_client.py
--rw-r--r--   0 yoaz       (502) staff       (20)     3790 2024-05-19 13:43:20.000000 prompeteer-0.3.4/prompeteer/providers/llm_request.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.917103 prompeteer-0.3.4/prompeteer/utils/
--rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.4/prompeteer/utils/__init__.py
--rw-r--r--   0 yoaz       (502) staff       (20)     1012 2024-05-19 12:43:51.000000 prompeteer-0.3.4/prompeteer/utils/utils.py
-drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-05-20 12:30:11.918438 prompeteer-0.3.4/prompeteer.egg-info/
--rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-05-20 12:30:11.000000 prompeteer-0.3.4/prompeteer.egg-info/PKG-INFO
--rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-05-20 12:30:11.000000 prompeteer-0.3.4/prompeteer.egg-info/SOURCES.txt
--rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-05-20 12:30:11.000000 prompeteer-0.3.4/prompeteer.egg-info/dependency_links.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-05-20 12:30:11.000000 prompeteer-0.3.4/prompeteer.egg-info/requires.txt
--rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-05-20 12:30:11.000000 prompeteer-0.3.4/prompeteer.egg-info/top_level.txt
--rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.4/public_README.md
--rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-05-20 12:30:11.919399 prompeteer-0.3.4/setup.cfg
--rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-05-20 12:30:11.000000 prompeteer-0.3.4/setup.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.946705 prompeteer-0.3.5/
+-rw-r--r--   0 yoaz       (502) staff       (20)       42 2024-05-15 15:30:47.000000 prompeteer-0.3.5/MANIFEST.in
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-06-02 11:54:35.946385 prompeteer-0.3.5/PKG-INFO
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.937559 prompeteer-0.3.5/prompeteer/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     4142 2024-05-23 10:04:38.000000 prompeteer-0.3.5/prompeteer/prompeteer.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.940394 prompeteer-0.3.5/prompeteer/prompt/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/prompt/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)      673 2024-05-19 12:43:18.000000 prompeteer-0.3.5/prompeteer/prompt/prompt.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3171 2024-05-19 13:02:38.000000 prompeteer-0.3.5/prompeteer/prompt/prompt_config.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.941508 prompeteer-0.3.5/prompeteer/providers/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/providers/__init__.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.942400 prompeteer-0.3.5/prompeteer/providers/aws_bedrock/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/providers/aws_bedrock/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2186 2024-05-30 11:52:32.000000 prompeteer-0.3.5/prompeteer/providers/aws_bedrock/aws_bedrock_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1866 2024-05-19 12:41:47.000000 prompeteer-0.3.5/prompeteer/providers/aws_bedrock/aws_llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.943824 prompeteer-0.3.5/prompeteer/providers/azure_openai/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/providers/azure_openai/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     2070 2024-05-19 12:41:18.000000 prompeteer-0.3.5/prompeteer/providers/azure_openai/azure_llm_request.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3074 2024-05-19 13:17:36.000000 prompeteer-0.3.5/prompeteer/providers/azure_openai/azure_openai_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1445 2024-05-19 11:15:13.000000 prompeteer-0.3.5/prompeteer/providers/llm_client.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     3798 2024-06-02 11:51:52.000000 prompeteer-0.3.5/prompeteer/providers/llm_request.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.945299 prompeteer-0.3.5/prompeteer/utils/
+-rw-r--r--   0 yoaz       (502) staff       (20)        0 2024-05-15 12:42:33.000000 prompeteer-0.3.5/prompeteer/utils/__init__.py
+-rw-r--r--   0 yoaz       (502) staff       (20)     1012 2024-05-19 12:43:51.000000 prompeteer-0.3.5/prompeteer/utils/utils.py
+drwxr-xr-x   0 yoaz       (502) staff       (20)        0 2024-06-02 11:54:35.945897 prompeteer-0.3.5/prompeteer.egg-info/
+-rw-r--r--   0 yoaz       (502) staff       (20)     3883 2024-06-02 11:54:35.000000 prompeteer-0.3.5/prompeteer.egg-info/PKG-INFO
+-rw-r--r--   0 yoaz       (502) staff       (20)      816 2024-06-02 11:54:35.000000 prompeteer-0.3.5/prompeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)        1 2024-06-02 11:54:35.000000 prompeteer-0.3.5/prompeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       52 2024-06-02 11:54:35.000000 prompeteer-0.3.5/prompeteer.egg-info/requires.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)       11 2024-06-02 11:54:35.000000 prompeteer-0.3.5/prompeteer.egg-info/top_level.txt
+-rw-r--r--   0 yoaz       (502) staff       (20)     3414 2024-05-15 13:59:10.000000 prompeteer-0.3.5/public_README.md
+-rw-r--r--   0 yoaz       (502) staff       (20)       38 2024-06-02 11:54:35.946765 prompeteer-0.3.5/setup.cfg
+-rw-r--r--   0 yoaz       (502) staff       (20)      877 2024-06-02 11:54:35.000000 prompeteer-0.3.5/setup.py
```

### Comparing `prompeteer-0.3.4/PKG-INFO` & `prompeteer-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.4
+Version: 0.3.5
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.4/prompeteer/prompeteer.py` & `prompeteer-0.3.5/prompeteer/prompeteer.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/prompt/prompt.py` & `prompeteer-0.3.5/prompeteer/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/prompt/prompt_config.py` & `prompeteer-0.3.5/prompeteer/prompt/prompt_config.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/aws_bedrock/aws_bedrock_client.py` & `prompeteer-0.3.5/prompeteer/providers/aws_bedrock/aws_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/aws_bedrock/aws_llm_request.py` & `prompeteer-0.3.5/prompeteer/providers/aws_bedrock/aws_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/azure_openai/azure_llm_request.py` & `prompeteer-0.3.5/prompeteer/providers/azure_openai/azure_llm_request.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/azure_openai/azure_openai_client.py` & `prompeteer-0.3.5/prompeteer/providers/azure_openai/azure_openai_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/llm_client.py` & `prompeteer-0.3.5/prompeteer/providers/llm_client.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer/providers/llm_request.py` & `prompeteer-0.3.5/prompeteer/providers/llm_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def get_texts_to_inject(self) -> List[str]:
         """
         Returns a list of all text parts of the prompt that are candidates for variable substitution
         """
         raise NotImplementedError
 
     def validate_variables_to_inject(self, variables_to_inject: List[Variable]):
-        placeholder_pattern = re.compile(r'\{([^}]+)\}')
+        placeholder_pattern = re.compile(r'\{\{([^}]+)\}\}')
         all_placeholders = set()
 
         # Collect all placeholders from the texts
         for text in self.get_texts_to_inject():
             if text:
                 all_placeholders.update(placeholder_pattern.findall(text))
 
@@ -73,15 +73,15 @@
             if not text:
                 return text
 
             def replacer(match):
                 var_name = match.group(1)
                 return variables_map.get(var_name, '') if var_name in variables_map else ''
 
-            return re.sub(r'\{([^}]+)\}', replacer, text)
+            return re.sub(r'\{\{([^}]+)\}\}', replacer, text)
 
         texts_to_inject = self.get_texts_to_inject()
         injected_texts = [replace_placeholders(text) for text in texts_to_inject]
 
         self._set_injected_texts(injected_texts)
 
     @abstractmethod
```

### Comparing `prompeteer-0.3.4/prompeteer/utils/utils.py` & `prompeteer-0.3.5/prompeteer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/prompeteer.egg-info/PKG-INFO` & `prompeteer-0.3.5/prompeteer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompeteer
-Version: 0.3.4
+Version: 0.3.5
 Summary: Prompt Development and Evaluation tool
 Author: Yoaz Menda
 Author-email: yoazmenda@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `prompeteer-0.3.4/prompeteer.egg-info/SOURCES.txt` & `prompeteer-0.3.5/prompeteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/public_README.md` & `prompeteer-0.3.5/public_README.md`

 * *Files identical despite different names*

### Comparing `prompeteer-0.3.4/setup.py` & `prompeteer-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("public_README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='prompeteer',
-    version='0.3.4',
+    version='0.3.5',
     author='Yoaz Menda',
     author_email='yoazmenda@gmail.com',
     description='Prompt Development and Evaluation tool',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests', 'tests.*', 'README.md']),  # Include all packages
     py_modules=['prompeteer'],
```

