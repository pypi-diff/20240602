# Comparing `tmp/whyhow-0.0.6.tar.gz` & `tmp/whyhow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyhow-0.0.6.tar", last modified: Fri May 24 04:58:46 2024, max compression
+gzip compressed data, was "whyhow-0.0.7.tar", last modified: Sun Jun  2 02:28:57 2024, max compression
```

## Comparing `whyhow-0.0.6.tar` & `whyhow-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.662514 whyhow-0.0.6/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     8677 2024-05-24 04:58:46.662273 whyhow-0.0.6/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)     7548 2024-05-24 04:57:29.000000 whyhow-0.0.6/README.md
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-05-07 03:43:17.000000 whyhow-0.0.6/pyproject.toml
--rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-05-24 04:58:46.662553 whyhow-0.0.6/setup.cfg
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.656150 whyhow-0.0.6/src/
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.657557 whyhow-0.0.6/src/whyhow/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-05-24 04:57:51.000000 whyhow-0.0.6/src/whyhow/__init__.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.659309 whyhow-0.0.6/src/whyhow/apis/
--rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/apis/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.6/src/whyhow/apis/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     9876 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/apis/graph.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     6707 2024-04-21 01:37:48.000000 whyhow-0.0.6/src/whyhow/client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/exceptions.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/py.typed
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.660312 whyhow-0.0.6/src/whyhow/schemas/
--rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/schemas/__init__.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.6/src/whyhow/schemas/base.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     5089 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/schemas/common.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)     2569 2024-05-24 02:12:35.000000 whyhow-0.0.6/src/whyhow/schemas/graph.py
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.661165 whyhow-0.0.6/src/whyhow.egg-info/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     8677 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/PKG-INFO
--rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/SOURCES.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/dependency_links.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.6/src/whyhow.egg-info/not-zip-safe
--rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/requires.txt
--rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-05-24 04:58:46.000000 whyhow-0.0.6/src/whyhow.egg-info/top_level.txt
-drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-05-24 04:58:46.660760 whyhow-0.0.6/tests/
--rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-05-07 03:43:17.000000 whyhow-0.0.6/tests/test_client.py
--rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.6/tests/test_dummy.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.430298 whyhow-0.0.7/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     9422 2024-06-02 02:28:57.430002 whyhow-0.0.7/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     8293 2024-06-02 02:21:34.000000 whyhow-0.0.7/README.md
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2061 2024-05-07 03:43:17.000000 whyhow-0.0.7/pyproject.toml
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       38 2024-06-02 02:28:57.430341 whyhow-0.0.7/setup.cfg
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.423033 whyhow-0.0.7/src/
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.424869 whyhow-0.0.7/src/whyhow/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      125 2024-06-02 02:28:09.000000 whyhow-0.0.7/src/whyhow/__init__.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.426686 whyhow-0.0.7/src/whyhow/apis/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       49 2024-03-30 23:23:35.000000 whyhow-0.0.7/src/whyhow/apis/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      501 2024-04-04 06:55:34.000000 whyhow-0.0.7/src/whyhow/apis/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     9876 2024-05-24 02:12:35.000000 whyhow-0.0.7/src/whyhow/apis/graph.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     9952 2024-06-02 01:43:32.000000 whyhow-0.0.7/src/whyhow/client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      166 2024-03-30 23:23:35.000000 whyhow-0.0.7/src/whyhow/exceptions.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        0 2024-03-30 23:23:35.000000 whyhow-0.0.7/src/whyhow/py.typed
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.428050 whyhow-0.0.7/src/whyhow/schemas/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      189 2024-03-30 23:23:35.000000 whyhow-0.0.7/src/whyhow/schemas/__init__.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      624 2024-03-30 23:23:35.000000 whyhow-0.0.7/src/whyhow/schemas/base.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     5089 2024-05-24 02:12:35.000000 whyhow-0.0.7/src/whyhow/schemas/common.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     2569 2024-05-24 02:12:35.000000 whyhow-0.0.7/src/whyhow/schemas/graph.py
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.428842 whyhow-0.0.7/src/whyhow.egg-info/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     9422 2024-06-02 02:28:57.000000 whyhow-0.0.7/src/whyhow.egg-info/PKG-INFO
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      548 2024-06-02 02:28:57.000000 whyhow-0.0.7/src/whyhow.egg-info/SOURCES.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-06-02 02:28:57.000000 whyhow-0.0.7/src/whyhow.egg-info/dependency_links.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        1 2024-03-31 17:56:30.000000 whyhow-0.0.7/src/whyhow.egg-info/not-zip-safe
+-rw-r--r--   0 tomsmoker   (501) staff       (20)      218 2024-06-02 02:28:57.000000 whyhow-0.0.7/src/whyhow.egg-info/requires.txt
+-rw-r--r--   0 tomsmoker   (501) staff       (20)        7 2024-06-02 02:28:57.000000 whyhow-0.0.7/src/whyhow.egg-info/top_level.txt
+drwxr-xr-x   0 tomsmoker   (501) staff       (20)        0 2024-06-02 02:28:57.428559 whyhow-0.0.7/tests/
+-rw-r--r--   0 tomsmoker   (501) staff       (20)     1431 2024-05-07 03:43:17.000000 whyhow-0.0.7/tests/test_client.py
+-rw-r--r--   0 tomsmoker   (501) staff       (20)       48 2024-03-30 23:23:35.000000 whyhow-0.0.7/tests/test_dummy.py
```

### Comparing `whyhow-0.0.6/PKG-INFO` & `whyhow-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.6
+Version: 0.0.7
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -30,15 +30,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pymdown-extensions; extra == "docs"
 
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/whyhow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs with your data.
 
 # Installation
@@ -53,15 +53,22 @@
 ## Install from PyPI
 
 You can install the SDK directly from PyPI using pip:
 
 ```shell
 pip install whyhow
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 ## Install from Github
@@ -70,15 +77,22 @@
 
 ```shell
 
 git clone git@github.com:whyhow-ai/whyhow.git
 cd whyhow
 pip install .
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 # Examples
@@ -93,14 +107,30 @@
 
 ```shell
 from whyhow import WhyHow
 
 client = WhyHow(api_key=<your whyhow api key>)
 ```
 
+For Azure Open AI: 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, use_azure=True)
+```
+
+For an alternative model (for example, healthcare for text extraction): 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, model_type='health')
+```
+
 ## Add documents to namespace
 
 Your namespace is a logical grouping of the raw data you upload, the seed concepts you define, and the graphs you create. Namespaces are meant to be tightly scoped to your use case. You can create as many namespaces as you want.
 
 ```shell
 
 namespace = "harry-potter"
```

### Comparing `whyhow-0.0.6/README.md` & `whyhow-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/whyhow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs with your data.
 
 # Installation
@@ -21,15 +21,22 @@
 ## Install from PyPI
 
 You can install the SDK directly from PyPI using pip:
 
 ```shell
 pip install whyhow
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 ## Install from Github
@@ -38,15 +45,22 @@
 
 ```shell
 
 git clone git@github.com:whyhow-ai/whyhow.git
 cd whyhow
 pip install .
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 # Examples
@@ -61,14 +75,30 @@
 
 ```shell
 from whyhow import WhyHow
 
 client = WhyHow(api_key=<your whyhow api key>)
 ```
 
+For Azure Open AI: 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, use_azure=True)
+```
+
+For an alternative model (for example, healthcare for text extraction): 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, model_type='health')
+```
+
 ## Add documents to namespace
 
 Your namespace is a logical grouping of the raw data you upload, the seed concepts you define, and the graphs you create. Namespaces are meant to be tightly scoped to your use case. You can create as many namespaces as you want.
 
 ```shell
 
 namespace = "harry-potter"
```

### Comparing `whyhow-0.0.6/pyproject.toml` & `whyhow-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/src/whyhow/apis/graph.py` & `whyhow-0.0.7/src/whyhow/apis/graph.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/src/whyhow/schemas/base.py` & `whyhow-0.0.7/src/whyhow/schemas/base.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/src/whyhow/schemas/common.py` & `whyhow-0.0.7/src/whyhow/schemas/common.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/src/whyhow/schemas/graph.py` & `whyhow-0.0.7/src/whyhow/schemas/graph.py`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/src/whyhow.egg-info/PKG-INFO` & `whyhow-0.0.7/src/whyhow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whyhow
-Version: 0.0.6
+Version: 0.0.7
 Summary: Whyhow automated KG SDK
 Author-email: Tom Smoker <tom@whyhow.ai>, Chris Rec <chris@whyhow.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/whyhow-ai/whyhow
 Keywords: SDK,KG
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -30,15 +30,15 @@
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: pymdown-extensions; extra == "docs"
 
 # WhyHow Knowledge Graph Creation SDK
 
 [![Python Version](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)
-[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/why/)
+[![PyPI Version](https://img.shields.io/pypi/v/whyhow)](https://pypi.org/project/whyhow/)
 [![Code Style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)](https://mypy-lang.org/)
 [![Whyhow Discord](https://dcbadge.vercel.app/api/server/9bWqrsxgHr?compact=true&style=flat)](https://discord.gg/9bWqrsxgHr)
 
 The WhyHow Knowledge Graph Creation SDK enables you to quickly and easily build automated knowledge graphs tailored to your unique worldview. Instantly build, extend, and query well-scoped KGs with your data.
 
 # Installation
@@ -53,15 +53,22 @@
 ## Install from PyPI
 
 You can install the SDK directly from PyPI using pip:
 
 ```shell
 pip install whyhow
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 ## Install from Github
@@ -70,15 +77,22 @@
 
 ```shell
 
 git clone git@github.com:whyhow-ai/whyhow.git
 cd whyhow
 pip install .
 
+# For OpenAI
 export OPENAI_API_KEY=<your openai api key>
+
+# For Azure OpenAI 
+export AZURE_OPENAI_API_KEY=<your azure openai api key>
+export AZURE_OPENAI_API_VERSION=<your azure openai api version>
+export AZURE_OPENAI_ENDPOINT=<your azure openai api endpoint>
+
 export PINECONE_API_KEY=<your pinecone api key>
 export NEO4J_URL=<your neo4j url>
 export NEO4J_USERNAME=<your neo4j username>
 export NEO4J_PASSWORD=<your neo4j password>
 ```
 
 # Examples
@@ -93,14 +107,30 @@
 
 ```shell
 from whyhow import WhyHow
 
 client = WhyHow(api_key=<your whyhow api key>)
 ```
 
+For Azure Open AI: 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, use_azure=True)
+```
+
+For an alternative model (for example, healthcare for text extraction): 
+
+```shell
+from whyhow import WhyHow
+
+client = WhyHow(api_key=<your whyhow api key>, model_type='health')
+```
+
 ## Add documents to namespace
 
 Your namespace is a logical grouping of the raw data you upload, the seed concepts you define, and the graphs you create. Namespaces are meant to be tightly scoped to your use case. You can create as many namespaces as you want.
 
 ```shell
 
 namespace = "harry-potter"
```

### Comparing `whyhow-0.0.6/src/whyhow.egg-info/SOURCES.txt` & `whyhow-0.0.7/src/whyhow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whyhow-0.0.6/tests/test_client.py` & `whyhow-0.0.7/tests/test_client.py`

 * *Files identical despite different names*

