# Comparing `tmp/suparkanbun-1.5.2-py3-none-any.whl.zip` & `tmp/suparkanbun-1.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 957536 bytes, number of entries: 72
+Zip file size: 957535 bytes, number of entries: 72
 -rw-r--r--  2.0 unx       89 b- defN 21-Jun-19 01:01 suparkanbun/__init__.py
 -rw-r--r--  2.0 unx     1086 b- defN 22-Sep-16 10:32 suparkanbun/download.py
 -rw-r--r--  2.0 unx    48825 b- defN 24-Feb-29 02:30 suparkanbun/simplify.py
 -rw-r--r--  2.0 unx     7891 b- defN 22-Sep-16 10:09 suparkanbun/suparkanbun.py
 -rw-r--r--  2.0 unx    19301 b- defN 24-Feb-29 02:31 suparkanbun/tradify.py
 -rw-r--r--  2.0 unx   267736 b- defN 24-Feb-29 02:15 suparkanbun/models/gloss.orig.txt
 -rw-r--r--  2.0 unx     4539 b- defN 21-Dec-25 00:11 suparkanbun/models/labelPOS.txt
@@ -62,13 +62,13 @@
 -rw-r--r--  2.0 unx      348 b- defN 21-Oct-03 09:49 suparkanbun/models/sikuroberta.danku/tokenizer_config.json
 -rw-r--r--  2.0 unx   144192 b- defN 21-Oct-03 09:49 suparkanbun/models/sikuroberta.danku/vocab.txt
 -rw-r--r--  2.0 unx    17626 b- defN 21-Dec-25 00:11 suparkanbun/models/sikuroberta.pos/config.json
 -rw-r--r--  2.0 unx       56 b- defN 22-Jan-16 23:49 suparkanbun/models/sikuroberta.pos/filesize.txt
 -rw-r--r--  2.0 unx      112 b- defN 21-May-24 07:52 suparkanbun/models/sikuroberta.pos/special_tokens_map.json
 -rw-r--r--  2.0 unx      348 b- defN 21-Oct-03 09:49 suparkanbun/models/sikuroberta.pos/tokenizer_config.json
 -rw-r--r--  2.0 unx   144192 b- defN 21-Oct-03 09:49 suparkanbun/models/sikuroberta.pos/vocab.txt
--rw-r--r--  2.0 unx     1071 b- defN 24-Feb-29 02:33 suparkanbun-1.5.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4404 b- defN 24-Feb-29 02:33 suparkanbun-1.5.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-29 02:33 suparkanbun-1.5.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Feb-29 02:33 suparkanbun-1.5.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7988 b- defN 24-Feb-29 02:33 suparkanbun-1.5.2.dist-info/RECORD
-72 files, 1853735 bytes uncompressed, 944110 bytes compressed:  49.1%
+-rw-r--r--  2.0 unx     1071 b- defN 24-Jun-02 09:02 suparkanbun-1.5.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4404 b- defN 24-Jun-02 09:02 suparkanbun-1.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Jun-02 09:02 suparkanbun-1.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Jun-02 09:02 suparkanbun-1.5.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7988 b- defN 24-Jun-02 09:02 suparkanbun-1.5.3.dist-info/RECORD
+72 files, 1853735 bytes uncompressed, 944109 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -195,23 +195,23 @@
 
 Filename: suparkanbun/models/sikuroberta.pos/tokenizer_config.json
 Comment: 
 
 Filename: suparkanbun/models/sikuroberta.pos/vocab.txt
 Comment: 
 
-Filename: suparkanbun-1.5.2.dist-info/LICENSE.txt
+Filename: suparkanbun-1.5.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: suparkanbun-1.5.2.dist-info/METADATA
+Filename: suparkanbun-1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: suparkanbun-1.5.2.dist-info/WHEEL
+Filename: suparkanbun-1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: suparkanbun-1.5.2.dist-info/top_level.txt
+Filename: suparkanbun-1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: suparkanbun-1.5.2.dist-info/RECORD
+Filename: suparkanbun-1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `suparkanbun-1.5.2.dist-info/LICENSE.txt` & `suparkanbun-1.5.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `suparkanbun-1.5.2.dist-info/METADATA` & `suparkanbun-1.5.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suparkanbun
-Version: 1.5.2
+Version: 1.5.3
 Summary: Tokenizer POS-tagger and Dependency-parser for Classical Chinese
 Home-page: https://github.com/KoichiYasuoka/SuPar-Kanbun
 Author: Koichi Yasuoka
 Author-email: yasuoka@kanji.zinbun.kyoto-u.ac.jp
 License: MIT
 Project-URL: Source, https://github.com/KoichiYasuoka/SuPar-Kanbun
 Project-URL: Tracker, https://github.com/KoichiYasuoka/SuPar-Kanbun/issues
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: deplacy (>=2.0.8)
+Requires-Dist: deplacy (>=2.1.0)
 Requires-Dist: spacy (>=2.2.2)
 Requires-Dist: supar (>=1.1.4)
 Requires-Dist: transformers (>=4.0.1)
 
 [![Current PyPI packages](https://badge.fury.io/py/suparkanbun.svg)](https://pypi.org/project/suparkanbun/)
 
 # SuPar-Kanbun
```

## Comparing `suparkanbun-1.5.2.dist-info/RECORD` & `suparkanbun-1.5.3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,12 @@
 suparkanbun/models/sikuroberta.danku/tokenizer_config.json,sha256=NmH9XujKnfExC3JZg50eQ7vIKxLX5PSpB-n2fMFpgyM,348
 suparkanbun/models/sikuroberta.danku/vocab.txt,sha256=UdMWHMKdtrXS6EHaViufi1nAUORLyrIxnD6vpxxiUi4,144192
 suparkanbun/models/sikuroberta.pos/config.json,sha256=X0keX2Oy0_qAN_4Eo63kjdqbOURImZ5aLYeDGFsSgNE,17626
 suparkanbun/models/sikuroberta.pos/filesize.txt,sha256=0tGNdJyONmT9LhfOzLVr9EljkPcmJoKSq_YxkScpKyM,56
 suparkanbun/models/sikuroberta.pos/special_tokens_map.json,sha256=MD30WgNgnk6tBLw9wVNtCrGbU1jbaFtvPaEj0F7CAOM,112
 suparkanbun/models/sikuroberta.pos/tokenizer_config.json,sha256=NmH9XujKnfExC3JZg50eQ7vIKxLX5PSpB-n2fMFpgyM,348
 suparkanbun/models/sikuroberta.pos/vocab.txt,sha256=UdMWHMKdtrXS6EHaViufi1nAUORLyrIxnD6vpxxiUi4,144192
-suparkanbun-1.5.2.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
-suparkanbun-1.5.2.dist-info/METADATA,sha256=BUh-okKlbgAkqRPRvJ_IZ-JdcJg4R92agknp51raRws,4404
-suparkanbun-1.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-suparkanbun-1.5.2.dist-info/top_level.txt,sha256=_Z4XHn_aQMDRXLKekMJ-g7mYrdvgV9DxGb-aYp9P1TI,12
-suparkanbun-1.5.2.dist-info/RECORD,,
+suparkanbun-1.5.3.dist-info/LICENSE.txt,sha256=c5zUIy4TBdSWvwjgE_MuQG4kAsjooqTYl9uXpuNTKXE,1071
+suparkanbun-1.5.3.dist-info/METADATA,sha256=T88peAYJ2m-N0Co6f1BMqYw9up1eNuZctkzPj07OSCk,4404
+suparkanbun-1.5.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+suparkanbun-1.5.3.dist-info/top_level.txt,sha256=_Z4XHn_aQMDRXLKekMJ-g7mYrdvgV9DxGb-aYp9P1TI,12
+suparkanbun-1.5.3.dist-info/RECORD,,
```

