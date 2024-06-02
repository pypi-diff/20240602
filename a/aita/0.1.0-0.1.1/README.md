# Comparing `tmp/aita-0.1.0.tar.gz` & `tmp/aita-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aita-0.1.0.tar", max compression
+gzip compressed data, was "aita-0.1.1.tar", max compression
```

## Comparing `aita-0.1.0.tar` & `aita-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,56 @@
--rw-r--r--   0        0        0    10881 2024-02-17 04:08:39.254098 aita-0.1.0/LICENSE
--rw-r--r--   0        0        0     3161 2024-04-18 20:59:07.369891 aita-0.1.0/README.md
--rw-r--r--   0        0        0      424 2024-02-17 04:08:39.201550 aita-0.1.0/aita/.editorconfig
--rw-r--r--   0        0        0    10539 2024-02-19 18:25:51.912426 aita-0.1.0/aita/.gitignore
--rw-r--r--   0        0        0        7 2024-03-02 07:37:26.675147 aita-0.1.0/aita/README.md
--rw-r--r--   0        0        0      313 2024-02-17 05:19:49.350060 aita-0.1.0/aita/__init__.py
--rw-r--r--   0        0        0     1438 2024-02-17 05:18:38.689934 aita-0.1.0/aita/__main__.py
--rw-r--r--   0        0        0        0 2024-04-17 21:53:19.777436 aita-0.1.0/aita/agent/__init__.py
--rw-r--r--   0        0        0     2736 2024-04-27 23:42:05.210640 aita-0.1.0/aita/agent/base.py
--rw-r--r--   0        0        0      710 2024-04-27 23:35:08.066009 aita-0.1.0/aita/agent/ipython.py
--rw-r--r--   0        0        0      931 2024-04-27 23:28:52.823321 aita-0.1.0/aita/agent/pandas.py
--rw-r--r--   0        0        0      848 2024-04-17 22:03:05.225302 aita-0.1.0/aita/agent/pyspark.py
--rw-r--r--   0        0        0      806 2024-04-27 23:06:24.256924 aita-0.1.0/aita/agent/sql.py
--rw-r--r--   0        0        0        0 2024-02-18 05:49:28.323810 aita-0.1.0/aita/datasource/__init__.py
--rw-r--r--   0        0        0     1583 2024-04-17 22:06:08.795991 aita-0.1.0/aita/datasource/base.py
--rw-r--r--   0        0        0      373 2024-02-27 01:34:57.816357 aita-0.1.0/aita/datasource/bigquery.py
--rw-r--r--   0        0        0      803 2024-02-27 01:34:57.821756 aita-0.1.0/aita/datasource/factory.py
--rw-r--r--   0        0        0      498 2024-04-17 22:05:46.752703 aita-0.1.0/aita/datasource/mysql.py
--rw-r--r--   0        0        0      388 2024-02-27 01:34:57.819825 aita-0.1.0/aita/datasource/postgresql.py
--rw-r--r--   0        0        0     2887 2024-04-05 23:17:35.543027 aita-0.1.0/aita/datasource/snowflake.py
--rw-r--r--   0        0        0      313 2024-02-19 18:28:09.775021 aita-0.1.0/aita/example.py
--rw-r--r--   0        0        0     1057 2024-02-23 04:57:54.714776 aita-0.1.0/aita/state_store.py
--rw-r--r--   0        0        0        0 2024-04-17 21:53:12.009385 aita-0.1.0/aita/tool/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-17 21:57:04.494325 aita-0.1.0/aita/tool/ipython.py
--rw-r--r--   0        0        0      363 2024-04-17 21:57:04.487808 aita-0.1.0/aita/tool/pandas.py
--rw-r--r--   0        0        0      357 2024-04-17 21:57:04.482914 aita-0.1.0/aita/tool/spark.py
--rw-r--r--   0        0        0     1653 2024-04-17 21:57:04.516195 aita-0.1.0/aita/tool/sql.py
--rw-r--r--   0        0        0      629 2024-04-10 05:41:52.925969 aita-0.1.0/aita/utils.py
--rw-r--r--   0        0        0     4311 2024-04-26 23:00:48.235401 aita-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 aita-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10881 2024-02-17 04:08:39.254098 aita-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4686 2024-05-28 00:16:08.861163 aita-0.1.1/README.md
+-rw-r--r--   0        0        0      424 2024-02-17 04:08:39.201550 aita-0.1.1/aita/.editorconfig
+-rw-r--r--   0        0        0    10539 2024-02-19 18:25:51.912426 aita-0.1.1/aita/.gitignore
+-rw-r--r--   0        0        0      176 2024-06-01 17:40:19.504383 aita-0.1.1/aita/.idea/.gitignore
+-rw-r--r--   0        0        0      665 2024-06-01 17:42:50.277521 aita-0.1.1/aita/.idea/aita.iml
+-rw-r--r--   0        0        0      833 2024-06-01 17:42:50.254698 aita-0.1.1/aita/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2024-06-01 17:42:50.286004 aita-0.1.1/aita/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      188 2024-06-01 17:42:50.283804 aita-0.1.1/aita/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2024-06-01 17:42:50.280016 aita-0.1.1/aita/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2024-06-01 17:42:50.288845 aita-0.1.1/aita/.idea/vcs.xml
+-rw-r--r--   0        0        0      733 2024-06-01 18:07:50.507180 aita-0.1.1/aita/README.md
+-rw-r--r--   0        0        0      313 2024-02-17 05:19:49.350060 aita-0.1.1/aita/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:53:19.777436 aita-0.1.1/aita/agent/__init__.py
+-rw-r--r--   0        0        0     9763 2024-06-01 05:50:54.950099 aita-0.1.1/aita/agent/base.py
+-rw-r--r--   0        0        0      813 2024-05-27 16:25:54.998653 aita-0.1.1/aita/agent/factory.py
+-rw-r--r--   0        0        0      725 2024-06-01 08:01:43.973531 aita-0.1.1/aita/agent/pandas.py
+-rw-r--r--   0        0        0      687 2024-06-01 23:53:15.154068 aita-0.1.1/aita/agent/pyarrow.py
+-rw-r--r--   0        0        0     1534 2024-06-01 17:59:32.448350 aita-0.1.1/aita/agent/pyspark.py
+-rw-r--r--   0        0        0      492 2024-05-29 16:45:32.531175 aita-0.1.1/aita/agent/python.py
+-rw-r--r--   0        0        0      498 2024-06-01 06:16:11.085942 aita-0.1.1/aita/agent/sql.py
+-rw-r--r--   0        0        0        0 2024-02-18 05:49:28.323810 aita-0.1.1/aita/datasource/__init__.py
+-rw-r--r--   0        0        0      312 2024-06-01 07:28:12.513640 aita-0.1.1/aita/datasource/base.py
+-rw-r--r--   0        0        0      500 2024-05-15 06:16:36.561011 aita-0.1.1/aita/datasource/bigquery.py
+-rw-r--r--   0        0        0     1732 2024-06-01 08:08:43.620052 aita-0.1.1/aita/datasource/catalog.py
+-rw-r--r--   0        0        0     1135 2024-05-23 22:33:38.010910 aita-0.1.1/aita/datasource/factory.py
+-rw-r--r--   0        0        0     1787 2024-06-01 17:29:17.174107 aita-0.1.1/aita/datasource/file.py
+-rw-r--r--   0        0        0     1435 2024-05-21 21:43:49.085475 aita-0.1.1/aita/datasource/mysql.py
+-rw-r--r--   0        0        0      490 2024-05-20 05:03:33.662370 aita-0.1.1/aita/datasource/nosql.py
+-rw-r--r--   0        0        0     1537 2024-05-23 05:56:13.927255 aita-0.1.1/aita/datasource/postgresql.py
+-rw-r--r--   0        0        0     1294 2024-05-25 22:28:54.836728 aita-0.1.1/aita/datasource/snowflake.py
+-rw-r--r--   0        0        0     1513 2024-06-01 06:22:45.409600 aita-0.1.1/aita/datasource/sql.py
+-rw-r--r--   0        0        0     1001 2024-05-25 22:40:17.342137 aita-0.1.1/aita/datasource/sqlite.py
+-rw-r--r--   0        0        0     2068 2024-05-17 05:56:58.575503 aita-0.1.1/aita/prompt/ExampleFormatTemplate.py
+-rw-r--r--   0        0        0     9973 2024-05-17 06:45:47.748310 aita-0.1.1/aita/prompt/ExampleSelectorTemplate.py
+-rw-r--r--   0        0        0     4042 2024-05-17 06:45:47.737257 aita-0.1.1/aita/prompt/PromptICLTemplate.py
+-rw-r--r--   0        0        0    19493 2024-05-17 06:45:47.755591 aita-0.1.1/aita/prompt/PromptReprTemplate.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:49:31.582964 aita-0.1.1/aita/prompt/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-31 22:28:37.719539 aita-0.1.1/aita/prompt/base.py
+-rw-r--r--   0        0        0     1509 2024-05-23 21:04:05.999426 aita-0.1.1/aita/prompt/enums.py
+-rw-r--r--   0        0        0     4913 2024-05-29 04:14:56.935922 aita-0.1.1/aita/prompt/prompt_builder.py
+-rw-r--r--   0        0        0    15528 2024-05-17 23:57:05.466692 aita-0.1.1/aita/prompt/templates/dataset1.json
+-rw-r--r--   0        0        0    13192 2024-05-17 23:50:07.171654 aita-0.1.1/aita/prompt/templates/dataset2.json
+-rw-r--r--   0        0        0     4575 2024-05-23 21:33:23.144991 aita-0.1.1/aita/prompt/templates/formatted_data.json
+-rw-r--r--   0        0        0      722 2024-05-23 21:33:23.115841 aita-0.1.1/aita/prompt/templates/templates_parser.py
+-rw-r--r--   0        0        0    13124 2024-05-17 06:45:16.754527 aita-0.1.1/aita/prompt/utils.py
+-rw-r--r--   0        0        0      519 2024-06-01 18:07:50.499579 aita-0.1.1/aita/states.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:53:12.009385 aita-0.1.1/aita/tool/__init__.py
+-rw-r--r--   0        0        0      712 2024-06-01 17:39:16.411886 aita-0.1.1/aita/tool/factory.py
+-rw-r--r--   0        0        0      567 2024-06-01 06:16:11.098039 aita-0.1.1/aita/tool/pandas.py
+-rw-r--r--   0        0        0      609 2024-06-01 06:16:11.101298 aita-0.1.1/aita/tool/pyarrow.py
+-rw-r--r--   0        0        0      912 2024-05-29 16:45:32.510747 aita-0.1.1/aita/tool/pyspark.py
+-rw-r--r--   0        0        0     1493 2024-05-29 16:45:32.526106 aita-0.1.1/aita/tool/python.py
+-rw-r--r--   0        0        0     3469 2024-06-01 08:01:43.979331 aita-0.1.1/aita/tool/sql.py
+-rw-r--r--   0        0        0     4514 2024-06-02 03:43:26.055725 aita-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 aita-0.1.1/PKG-INFO
```

### Comparing `aita-0.1.0/LICENSE` & `aita-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aita-0.1.0/aita/.gitignore` & `aita-0.1.1/aita/.gitignore`

 * *Files identical despite different names*

### Comparing `aita-0.1.0/aita/agent/pandas.py` & `aita-0.1.1/aita/agent/pandas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from typing import List, Dict
-import pandas as pd
-from aita.agent.base import AitaAgent
+from typing import Dict
+
+from aita.agent.base import ToolAgent
+from aita.tool.sql import ConvertToPandasTool
 from aita.tool.pandas import PandasTool
+from pandas import DataFrame
+
+from aita.tool.python import PythonTool
+
 
+class PandasAgent(ToolAgent):
 
-class PandasAgent(AitaAgent):
-    dataframes: List[pd.DataFrame]
+    def __init__(
+        self, model: str, model_parameters: Dict = None
+    ):
+        super().__init__([
+            PandasTool(),
+            ConvertToPandasTool(),
+        ], model, model_parameters)
 
-    prompt_context = """
-    Meta data of all available data source as pandas dataframe:
-    {dataframe_metadata}
-    """
-
-    def __init__(self,
-                 dataframes: Dict[str, pd.DataFrame],
-                 model_id: str,
-                 model_parameters: Dict = None):
-        tool = PandasTool(script_context=dataframes)
-        dataframe_metadata = []
-        for name, df in dataframes.items():
-            dataframe_metadata.append({
-                "name": name,
-                "columns": df.columns.tolist()
-            })
-        self.prompt_context = self.prompt_context.format(dataframe_metadata=dataframe_metadata)
-        super().__init__(model_id, model_parameters, [tool], prompt_context=self.prompt_context)
+    def add_dataframe(self, dataframe: DataFrame):
+        self._fill_prompt_context(dataframe.info)
+        for tool in self.tools:
+            if isinstance(tool, PythonTool):
+                tool.update_script_context(script_context=dataframe)
+        return self
```

### Comparing `aita-0.1.0/pyproject.toml` & `aita-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,122 @@
-# Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aita"
-version = "0.1.0"
+version = "0.1.1"
 description = "AI Powered Data Platform"
 readme = "README.md"
 authors = ["aita <contact@project-aita.com>"]
 license = "Apache Software License 2.0"
-repository = "https://github.com/aita/aita"
-homepage = "https://github.com/aita/aita"
+repository = "https://github.com/project-aita/aita"
+homepage = "https://www.project-aita.com"
 
-# Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = []  #! Update me
+keywords = ["Artificial Intelligence", "Data Analysis", "Code Generation"]
 
-# Pypi classifiers: https://pypi.org/classifiers/
-classifiers = [  #! Update me
-  "Development Status :: 3 - Alpha",
-  "Intended Audience :: Developers",
-  "Operating System :: OS Independent",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-  "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+]
+
+packages = [
+    { include = "aita" },
 ]
 
-[tool.poetry.scripts]
-# Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
-"aita" = "aita.__main__:app"
-"init-data" = "app.initial_data:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-typer = {extras = ["all"], version = "^0.4.0"}
-rich = "^10.14.0"
-fastapi = "^0.109.2"
-celery = "^5.3.6"
+#bcrypt = "^4.0.1"
+#docstring-parser = "^0.15"
+#email-validator = "^2.1.0.post1"
+#emails = "^0.6"
+#numpy = "^1.26.4"
+#passlib = "^1.7.4"
+#psycopg2-binary = "^2.9.9"
+#python-jose = "^3.3.0"
+#python-multipart = "^0.0.9"
+#raven = "^6.10.0"
+#tenacity = "^8.2.3"
+
+mock = "^5.1.0"
 openai = "^1.12.0"
-uvicorn = "^0.27.1"
-tenacity = "^8.2.3"
-raven = "^6.10.0"
-types-toml = "^0.10.8.7"
-types-setuptools = "^69.1.0.20240301"
-pydantic = "^2.6.1"
-pydantic-settings = "^2.2.0"
-sqlalchemy = "^1.4.0"
-passlib = "^1.7.4"
-python-jose = "^3.3.0"
-email-validator = "^2.1.0.post1"
-emails = "^0.6"
-python-multipart = "^0.0.9"
-psycopg2-binary = "^2.9.9"
-docstring-parser = "^0.15"
-numpy = "^1.26.4"
-langchain = "^0.1.9"
+pydantic = "^2.7.1"
+jupyter-ai-magics = "^2.14.0"
+pandas = "^2.2.2"
 langchain-openai = "^0.0.7"
-mock = "^5.1.0"
-alembic = "^1.13.1"
-bcrypt = "^4.0.1"
-pandas = "^2.2.1"
-snowflake-connector-python = {extras = ["pandas"], version = "^3.8.0"}
+langchain = "0.1.20"
+langgraph = "^0.0.48"
+adbc-driver-sqlite = "^1.0.0"
 ipython = "8.14"
-jupyter = "^1.0.0"
-pyspark = "^3.5.1"
-jupyter-ai-magics = "^2.14.0"
+pyarrow = "^16.1.0"
+typer = "^0.12.3"
+types-setuptools = "^70.0.0.20240524"
+
+[tool.poetry.group.aws]
+optional = true
+
+[tool.poetry.group.aws.dependencies]
+boto3 = "^1.34.117"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.postgresql]
+optional = true
+
+[tool.poetry.group.postgresql.dependencies]
+adbc-driver-postgresql = "^1.0.0"
+
+[tool.poetry.group.snowflake]
+optional = true
+
+[tool.poetry.group.snowflake.dependencies]
+adbc-driver-snowflake = "^1.0.0"
+
+[tool.poetry.group.pyspark]
+optional = true
+
+[tool.poetry.group.pyspark.dependencies]
+findspark = "^2.0.1"
+pyspark = "^3.2.0"
+
+[tool.poetry.group.aitalab]
+optional = true
+
+[tool.poetry.group.aitalab.dependencies]
+alembic = "^1.13.1"
+reflex = "^0.5.0"
+transformers = "^4.40.2"
+sql-metadata = "^2.11.0"
+
+[tool.poetry.group.dev.dependencies]
+jupyter = "^1.0.0"
 bandit = "^1.7.1"
-black = {version = "^22.3.0", allow-prereleases = true}
+black = { version = "^22.3.0", allow-prereleases = true }
 darglint = "^1.8.1"
-isort = {extras = ["colors"], version = "^5.10.1"}
+isort = { extras = ["colors"], version = "^5.10.1" }
 mypy = "^1.0"
 mypy-extensions = "^0.4.3"
 pre-commit = "^2.15.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.11.1"
 pytest = "^6.2.5"
 pyupgrade = "^2.29.1"
 safety = "^1.10.3"
 coverage = "^6.1.2"
 coverage-badge = "^1.1.0"
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
 
+
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 100
 color = true
 
 exclude = '''
@@ -107,15 +133,15 @@
     | env
     | venv
 )/
 '''
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
-py_version = 38
+py_version = 39
 line_length = 100
 
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
 sections = ["FUTURE", "TYPING", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 include_trailing_comma = true
 profile = "black"
 multi_line_output = 3
@@ -148,23 +174,23 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 
 
 [tool.pytest.ini_options]
 # https://docs.pytest.org/en/6.2.x/customize.html#pyproject-toml
 # Directories that are not visited by pytest collector:
-norecursedirs =["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
+norecursedirs = ["hooks", "*.egg", ".eggs", "dist", "build", "docs", ".tox", ".git", "__pycache__"]
 doctest_optionflags = ["NUMBER", "NORMALIZE_WHITESPACE", "IGNORE_EXCEPTION_DETAIL"]
 
 # Extra options:
 addopts = [
-  "--strict-markers",
-  "--tb=short",
-  "--doctest-modules",
-  "--doctest-continue-on-failure",
+    "--strict-markers",
+    "--tb=short",
+    "--doctest-modules",
+    "--doctest-continue-on-failure",
 ]
 
 [tool.coverage.run]
 source = ["tests"]
 
 [coverage.paths]
 source = "aita"
```

