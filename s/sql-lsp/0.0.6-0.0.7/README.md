# Comparing `tmp/sql_lsp-0.0.6.tar.gz` & `tmp/sql_lsp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_lsp-0.0.6.tar", max compression
+gzip compressed data, was "sql_lsp-0.0.7.tar", max compression
```

## Comparing `sql_lsp-0.0.6.tar` & `sql_lsp-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1624 2024-05-06 02:35:19.504764 sql_lsp-0.0.6/README.md
--rw-r--r--   0        0        0      546 2024-05-27 02:18:47.971287 sql_lsp-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 03:55:22.443530 sql_lsp-0.0.6/sql_lsp/__init__.py
--rw-r--r--   0        0        0       71 2024-05-05 03:55:22.443530 sql_lsp-0.0.6/sql_lsp/__main__.py
--rw-r--r--   0        0        0     6169 2024-05-24 04:20:41.975414 sql_lsp-0.0.6/sql_lsp/completion.py
--rw-r--r--   0        0        0      329 2024-05-24 05:19:48.464502 sql_lsp-0.0.6/sql_lsp/config.py
--rw-r--r--   0        0        0     2369 2024-05-05 03:55:22.443530 sql_lsp-0.0.6/sql_lsp/database.py
--rw-r--r--   0        0        0     7991 2024-05-24 05:15:54.405504 sql_lsp-0.0.6/sql_lsp/mysql_connector.py
--rw-r--r--   0        0        0    10831 2024-05-27 02:19:10.210444 sql_lsp-0.0.6/sql_lsp/server.py
--rw-r--r--   0        0        0     4677 2024-05-24 05:26:46.789314 sql_lsp-0.0.6/sql_lsp/utils.py
--rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 sql_lsp-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1752 2024-06-02 01:41:40.453431 sql_lsp-0.0.7/README.md
+-rw-r--r--   0        0        0      558 2024-06-02 03:00:21.276676 sql_lsp-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 03:55:22.443530 sql_lsp-0.0.7/sql_lsp/__init__.py
+-rw-r--r--   0        0        0     1470 2024-06-02 02:49:51.034704 sql_lsp-0.0.7/sql_lsp/cli.py
+-rw-r--r--   0        0        0     6169 2024-05-24 04:20:41.975414 sql_lsp-0.0.7/sql_lsp/completion.py
+-rw-r--r--   0        0        0      329 2024-05-24 05:19:48.464502 sql_lsp-0.0.7/sql_lsp/config.py
+-rw-r--r--   0        0        0     2369 2024-05-05 03:55:22.443530 sql_lsp-0.0.7/sql_lsp/database.py
+-rw-r--r--   0        0        0     7991 2024-05-24 05:15:54.405504 sql_lsp-0.0.7/sql_lsp/mysql_connector.py
+-rw-r--r--   0        0        0    10831 2024-06-02 02:50:56.815901 sql_lsp-0.0.7/sql_lsp/server.py
+-rw-r--r--   0        0        0     4677 2024-05-24 05:26:46.789314 sql_lsp-0.0.7/sql_lsp/utils.py
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 sql_lsp-0.0.7/PKG-INFO
```

### Comparing `sql_lsp-0.0.6/README.md` & `sql_lsp-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -57,7 +57,9 @@
 
 ``` emacs-lisp
 (add-to-list 'eglot-server-programs
                '((sql-mode)
                  . ("sql-ls" "--stdio")))
 ```
 
+To enable all abilities for the language server, apply the patch provided in the
+repository in the file `eglot.patch` to eglot.
```

### Comparing `sql_lsp-0.0.6/pyproject.toml` & `sql_lsp-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-sql-ls = "sql_lsp.__main__:main"
+sql-ls = "sql_lsp.cli:main"
 
 [tool.poetry]
 name = "sql-lsp"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Chahak Mehta <chahakmehta013@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pygls = "^1.1.1"
 mysql-connector-python = "^8.2.0"
 sqlfluff = "^2.3.5"
 tabulate = "^0.9.0"
+click = "^8.1.7"
 
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.10.1"
 
 [tool.basedpyright]
```

### Comparing `sql_lsp-0.0.6/sql_lsp/completion.py` & `sql_lsp-0.0.7/sql_lsp/completion.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.6/sql_lsp/database.py` & `sql_lsp-0.0.7/sql_lsp/database.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.6/sql_lsp/mysql_connector.py` & `sql_lsp-0.0.7/sql_lsp/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.6/sql_lsp/server.py` & `sql_lsp-0.0.7/sql_lsp/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             self.available_connections = server_config["connections"]
             self.dbconn = DBConnection(
                 config=list(self.available_connections.values())[0]
             )
         return super().lsp_initialize(params)
 
 
-sql_server = LanguageServer("sql-ls", "v0.0.6", protocol_cls=SqlLanguageServerProtocol)
+sql_server = LanguageServer("sql-ls", "v0.0.7", protocol_cls=SqlLanguageServerProtocol)
 
 
 def _publish_diagnostics(ls: LanguageServer, uri: str):
     """Publish diagnostics to LSP server."""
     document = ls.workspace.get_text_document(uri)
     lint_diagnostics = sqlfluff.lint(
         document.source, dialect="mysql", config=fluff_config
```

### Comparing `sql_lsp-0.0.6/sql_lsp/utils.py` & `sql_lsp-0.0.7/sql_lsp/utils.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.6/PKG-INFO` & `sql_lsp-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: sql-lsp
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Chahak Mehta
 Author-email: chahakmehta013@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: mysql-connector-python (>=8.2.0,<9.0.0)
 Requires-Dist: pygls (>=1.1.1,<2.0.0)
 Requires-Dist: sqlfluff (>=2.3.5,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # sql-lsp
@@ -72,8 +73,10 @@
 
 ``` emacs-lisp
 (add-to-list 'eglot-server-programs
                '((sql-mode)
                  . ("sql-ls" "--stdio")))
 ```
 
+To enable all abilities for the language server, apply the patch provided in the
+repository in the file `eglot.patch` to eglot.
```

