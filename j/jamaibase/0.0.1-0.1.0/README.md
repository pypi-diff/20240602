# Comparing `tmp/jamaibase-0.0.1.tar.gz` & `tmp/jamaibase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamaibase-0.0.1.tar", last modified: Thu May 30 12:09:47 2024, max compression
+gzip compressed data, was "jamaibase-0.1.0.tar", last modified: Sun Jun  2 16:22:28 2024, max compression
```

## Comparing `jamaibase-0.0.1.tar` & `jamaibase-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.505776 jamaibase-0.0.1/
--rw-rw-r--   0 akk       (1000) akk       (1000)       16 2024-05-09 04:51:21.000000 jamaibase-0.0.1/.gitignore
--rw-r--r--   0 akk       (1000) akk       (1000)     2730 2024-05-30 12:09:47.505776 jamaibase-0.0.1/PKG-INFO
--rw-rw-r--   0 akk       (1000) akk       (1000)      973 2024-05-30 12:09:33.000000 jamaibase-0.0.1/README.md
--rw-rw-r--   0 akk       (1000) akk       (1000)     3722 2024-05-30 11:59:17.000000 jamaibase-0.0.1/pyproject.toml
--rw-rw-r--   0 akk       (1000) akk       (1000)       38 2024-05-30 12:09:47.505776 jamaibase-0.0.1/setup.cfg
--rw-rw-r--   0 akk       (1000) akk       (1000)       38 2024-05-02 14:54:26.000000 jamaibase-0.0.1/setup.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.477777 jamaibase-0.0.1/src/
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.481777 jamaibase-0.0.1/src/jamaibase/
--rw-rw-r--   0 akk       (1000) akk       (1000)       47 2024-05-30 11:46:36.000000 jamaibase-0.0.1/src/jamaibase/__init__.py
--rw-rw-r--   0 akk       (1000) akk       (1000)    23081 2024-05-30 11:57:22.000000 jamaibase-0.0.1/src/jamaibase/client.py
--rw-rw-r--   0 akk       (1000) akk       (1000)    53500 2024-05-30 11:46:37.000000 jamaibase-0.0.1/src/jamaibase/protocol.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.485777 jamaibase-0.0.1/src/jamaibase/utils/
--rw-rw-r--   0 akk       (1000) akk       (1000)        0 2024-05-09 04:51:21.000000 jamaibase-0.0.1/src/jamaibase/utils/__init__.py
--rw-rw-r--   0 akk       (1000) akk       (1000)     8250 2024-05-30 11:46:37.000000 jamaibase-0.0.1/src/jamaibase/utils/io.py
--rw-rw-r--   0 akk       (1000) akk       (1000)       45 2024-05-09 04:51:21.000000 jamaibase-0.0.1/src/jamaibase/utils/types.py
--rw-rw-r--   0 akk       (1000) akk       (1000)     4679 2024-05-09 04:51:21.000000 jamaibase-0.0.1/src/jamaibase/utils/versioning.py
--rw-rw-r--   0 akk       (1000) akk       (1000)       22 2024-05-09 04:51:21.000000 jamaibase-0.0.1/src/jamaibase/version.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.497776 jamaibase-0.0.1/src/jamaibase.egg-info/
--rw-r--r--   0 akk       (1000) akk       (1000)     2730 2024-05-30 12:09:47.000000 jamaibase-0.0.1/src/jamaibase.egg-info/PKG-INFO
--rw-rw-r--   0 akk       (1000) akk       (1000)     1696 2024-05-30 12:09:47.000000 jamaibase-0.0.1/src/jamaibase.egg-info/SOURCES.txt
--rw-rw-r--   0 akk       (1000) akk       (1000)        1 2024-05-30 12:09:47.000000 jamaibase-0.0.1/src/jamaibase.egg-info/dependency_links.txt
--rw-rw-r--   0 akk       (1000) akk       (1000)      559 2024-05-30 12:09:47.000000 jamaibase-0.0.1/src/jamaibase.egg-info/requires.txt
--rw-rw-r--   0 akk       (1000) akk       (1000)       10 2024-05-30 12:09:47.000000 jamaibase-0.0.1/src/jamaibase.egg-info/top_level.txt
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.489776 jamaibase-0.0.1/tests/
--rw-rw-r--   0 akk       (1000) akk       (1000)        0 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/__init__.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.489776 jamaibase-0.0.1/tests/_loader_check/
--rw-rw-r--   0 akk       (1000) akk       (1000)    10823 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/pdfloader__Swire_AR22_e_230406_sample.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)     6150 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/pdfloader__background-checks.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)    10170 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/pdfloader__sample_tables.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)    14632 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/split_documents__Swire_AR22_e_230406_sample.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)     6537 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/split_documents__background-checks.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)    19047 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/_loader_check/split_documents__sample_tables.pdf.json
--rw-rw-r--   0 akk       (1000) akk       (1000)     2670 2024-05-30 11:46:28.000000 jamaibase-0.0.1/tests/case_embed_files.py
--rw-rw-r--   0 akk       (1000) akk       (1000)      984 2024-05-30 11:46:28.000000 jamaibase-0.0.1/tests/create_long_txt.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.489776 jamaibase-0.0.1/tests/docx/
--rw-rw-r--   0 akk       (1000) akk       (1000)    20509 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/docx/Recommendation Letter.docx
--rw-rw-r--   0 akk       (1000) akk       (1000)      569 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/list_test_files_as_json.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.497776 jamaibase-0.0.1/tests/pdf/
--rw-rw-r--   0 akk       (1000) akk       (1000)   161910 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/Large Language Models as Optimizers [DeepMind ; 2023].pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)   713218 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/Swire_AR22_e_230406_sample.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)   924319 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/System Design Blueprint - The Ultimate Guide.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)   408520 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/Vehicle Detail - MyPUSPAKOM.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)    50918 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/ag-energy-round-up-2017-02-24.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)    90468 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/background-checks.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)   478619 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/ca-warn-report.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)    77168 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/salary 总结.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)   462837 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/sample_tables.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)     6403 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/san-jose-pd-firearm-sample.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)    28240 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/statement_card.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)    16469 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pdf/statement_ewallet.pdf
--rw-rw-r--   0 akk       (1000) akk       (1000)     1554 2024-05-30 11:46:28.000000 jamaibase-0.0.1/tests/populate_test_documents_minio.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.497776 jamaibase-0.0.1/tests/pptx/
--rw-rw-r--   0 akk       (1000) akk       (1000)   145363 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/pptx/(2017.06.30) Neural Machine Translation in Linear Time (ByteNet).pptx
--rw-rw-r--   0 akk       (1000) akk       (1000)     9693 2024-05-30 11:46:28.000000 jamaibase-0.0.1/tests/test_chat.py
--rw-rw-r--   0 akk       (1000) akk       (1000)    19571 2024-05-30 11:46:29.000000 jamaibase-0.0.1/tests/test_gen_executor.py
--rw-rw-r--   0 akk       (1000) akk       (1000)    52033 2024-05-30 11:46:29.000000 jamaibase-0.0.1/tests/test_gen_table.py
--rw-rw-r--   0 akk       (1000) akk       (1000)      996 2024-05-30 11:46:29.000000 jamaibase-0.0.1/tests/test_io.py
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.497776 jamaibase-0.0.1/tests/txt/
--rw-rw-r--   0 akk       (1000) akk       (1000)       50 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/txt/weather.txt
-drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-05-30 12:09:47.497776 jamaibase-0.0.1/tests/xlsx/
--rw-rw-r--   0 akk       (1000) akk       (1000)    86757 2024-05-09 04:51:21.000000 jamaibase-0.0.1/tests/xlsx/Claims Form.xlsx
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.643985 jamaibase-0.1.0/
+-rw-rw-r--   0 akk       (1000) akk       (1000)       16 2024-06-02 16:11:41.000000 jamaibase-0.1.0/.gitignore
+-rw-r--r--   0 akk       (1000) akk       (1000)     2730 2024-06-02 16:22:28.643985 jamaibase-0.1.0/PKG-INFO
+-rw-rw-r--   0 akk       (1000) akk       (1000)      973 2024-06-02 16:11:41.000000 jamaibase-0.1.0/README.md
+-rw-rw-r--   0 akk       (1000) akk       (1000)     3722 2024-06-02 16:11:41.000000 jamaibase-0.1.0/pyproject.toml
+-rw-rw-r--   0 akk       (1000) akk       (1000)       38 2024-06-02 16:22:28.643985 jamaibase-0.1.0/setup.cfg
+-rw-rw-r--   0 akk       (1000) akk       (1000)       38 2024-06-02 16:11:41.000000 jamaibase-0.1.0/setup.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.619985 jamaibase-0.1.0/src/
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.623985 jamaibase-0.1.0/src/jamaibase/
+-rw-rw-r--   0 akk       (1000) akk       (1000)       47 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/__init__.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)    35098 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/client.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)    53770 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/protocol.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.623985 jamaibase-0.1.0/src/jamaibase/utils/
+-rw-rw-r--   0 akk       (1000) akk       (1000)        0 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/utils/__init__.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)     8247 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/utils/io.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)       45 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/utils/types.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)     4679 2024-06-02 16:11:41.000000 jamaibase-0.1.0/src/jamaibase/utils/versioning.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)       22 2024-06-02 16:21:51.000000 jamaibase-0.1.0/src/jamaibase/version.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.639985 jamaibase-0.1.0/src/jamaibase.egg-info/
+-rw-r--r--   0 akk       (1000) akk       (1000)     2730 2024-06-02 16:22:28.000000 jamaibase-0.1.0/src/jamaibase.egg-info/PKG-INFO
+-rw-rw-r--   0 akk       (1000) akk       (1000)     1696 2024-06-02 16:22:28.000000 jamaibase-0.1.0/src/jamaibase.egg-info/SOURCES.txt
+-rw-rw-r--   0 akk       (1000) akk       (1000)        1 2024-06-02 16:22:28.000000 jamaibase-0.1.0/src/jamaibase.egg-info/dependency_links.txt
+-rw-rw-r--   0 akk       (1000) akk       (1000)      559 2024-06-02 16:22:28.000000 jamaibase-0.1.0/src/jamaibase.egg-info/requires.txt
+-rw-rw-r--   0 akk       (1000) akk       (1000)       10 2024-06-02 16:22:28.000000 jamaibase-0.1.0/src/jamaibase.egg-info/top_level.txt
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.627985 jamaibase-0.1.0/tests/
+-rw-rw-r--   0 akk       (1000) akk       (1000)        0 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/__init__.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.631985 jamaibase-0.1.0/tests/_loader_check/
+-rw-rw-r--   0 akk       (1000) akk       (1000)    10823 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/pdfloader__Swire_AR22_e_230406_sample.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)     6150 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/pdfloader__background-checks.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)    10170 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/pdfloader__sample_tables.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)    14632 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/split_documents__Swire_AR22_e_230406_sample.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)     6537 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/split_documents__background-checks.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)    19047 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/_loader_check/split_documents__sample_tables.pdf.json
+-rw-rw-r--   0 akk       (1000) akk       (1000)     2670 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/case_embed_files.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)      984 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/create_long_txt.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.631985 jamaibase-0.1.0/tests/docx/
+-rw-rw-r--   0 akk       (1000) akk       (1000)    20509 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/docx/Recommendation Letter.docx
+-rw-rw-r--   0 akk       (1000) akk       (1000)      569 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/list_test_files_as_json.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.639985 jamaibase-0.1.0/tests/pdf/
+-rw-rw-r--   0 akk       (1000) akk       (1000)   161910 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/Large Language Models as Optimizers [DeepMind ; 2023].pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)   713218 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/Swire_AR22_e_230406_sample.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)   924319 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/System Design Blueprint - The Ultimate Guide.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)   408520 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/Vehicle Detail - MyPUSPAKOM.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)    50918 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/ag-energy-round-up-2017-02-24.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)    90468 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/background-checks.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)   478619 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/ca-warn-report.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)    77168 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/salary 总结.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)   462837 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/sample_tables.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)     6403 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/san-jose-pd-firearm-sample.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)    28240 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/statement_card.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)    16469 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pdf/statement_ewallet.pdf
+-rw-rw-r--   0 akk       (1000) akk       (1000)     1554 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/populate_test_documents_minio.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.639985 jamaibase-0.1.0/tests/pptx/
+-rw-rw-r--   0 akk       (1000) akk       (1000)   145363 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/pptx/(2017.06.30) Neural Machine Translation in Linear Time (ByteNet).pptx
+-rw-rw-r--   0 akk       (1000) akk       (1000)    11058 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/test_chat.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)    29506 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/test_gen_executor.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)    52033 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/test_gen_table.py
+-rw-rw-r--   0 akk       (1000) akk       (1000)      996 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/test_io.py
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.639985 jamaibase-0.1.0/tests/txt/
+-rw-rw-r--   0 akk       (1000) akk       (1000)       50 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/txt/weather.txt
+drwxrwxr-x   0 akk       (1000) akk       (1000)        0 2024-06-02 16:22:28.639985 jamaibase-0.1.0/tests/xlsx/
+-rw-rw-r--   0 akk       (1000) akk       (1000)    86757 2024-06-02 16:11:41.000000 jamaibase-0.1.0/tests/xlsx/Claims Form.xlsx
```

### Comparing `jamaibase-0.0.1/PKG-INFO` & `jamaibase-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamaibase
-Version: 0.0.1
+Version: 0.1.0
 Summary: JamAI Base: Let Your Database Orchestrate LLMs and RAG
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Unix
 Requires-Python: >=3.10
```

### Comparing `jamaibase-0.0.1/README.md` & `jamaibase-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/pyproject.toml` & `jamaibase-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/src/jamaibase/client.py` & `jamaibase-0.1.0/src/jamaibase/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -684,7 +684,356 @@
             **kwargs,
         )
         response = self.raise_exception(response)
         if response_model is None:
             return response.text
         else:
             return response_model.model_validate_json(response.text)
+
+    # --- Models and chat --- #
+
+    async def model_info(
+        self,
+        name: str = "",
+        capabilities: list[str] | None = None,
+    ) -> p.ModelInfoResponse:
+        params = {"model": name, "capabilities": capabilities}
+        return await self._get(self.api_base, "/v1/models", params, p.ModelInfoResponse)
+
+    async def model_names(
+        self,
+        prefer: str = "",
+        capabilities: list[str] | None = None,
+    ) -> list[str]:
+        params = {"prefer": prefer, "capabilities": capabilities}
+        return json_loads(await self._get(self.api_base, "/v1/model_names", params))
+
+    async def generate_chat_completions(
+        self, request: p.ChatRequest
+    ) -> p.ChatCompletionChunk | AsyncGenerator[p.References | p.ChatCompletionChunk, None]:
+        """Generates chat completions.
+
+        Args:
+            request (ChatRequest): The request.
+
+        Returns:
+            completion (ChatCompletionChunk | AsyncGenerator): The chat completion.
+                In streaming mode, it is an async generator that yields a `References` object
+                followed by zero or more `ChatCompletionChunk` objects.
+                In non-streaming mode, it is a `ChatCompletionChunk` object.
+        """
+        if request.stream:
+
+            async def gen():
+                references = None
+                async for chunk in self._stream(self.api_base, "/v1/chat/completions", request):
+                    if request.rag_params is not None and references is None:
+                        try:
+                            references = p.References.model_validate_json(chunk[5:])
+                            yield references
+                        except ValidationError:
+                            pass
+                    try:
+                        yield p.ChatCompletionChunk.model_validate_json(chunk[5:])
+                        continue
+                    except ValidationError:
+                        pass
+
+            return gen()
+        else:
+            return await self._post(
+                self.api_base, "/v1/chat/completions", request, p.ChatCompletionChunk
+            )
+
+    # --- Gen Table --- #
+    async def create_action_table(self, request: p.ActionTableSchemaCreate) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base, "/v1/gen_tables/action", request, p.TableMetaResponse
+        )
+
+    async def create_knowledge_table(
+        self, request: p.KnowledgeTableSchemaCreate
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base, "/v1/gen_tables/knowledge", request, p.TableMetaResponse
+        )
+
+    async def create_chat_table(self, request: p.ChatTableSchemaCreate) -> p.TableMetaResponse:
+        return await self._post(self.api_base, "/v1/gen_tables/chat", request, p.TableMetaResponse)
+
+    async def get_table(
+        self, table_type: p.TableType, table_id: p.TableName
+    ) -> p.TableMetaResponse:
+        return await self._get(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/{quote(table_id)}",
+            None,
+            p.TableMetaResponse,
+        )
+
+    async def list_tables(
+        self,
+        table_type: p.TableType,
+        offset: int = 0,
+        limit: int = 100,
+    ) -> p.Page[p.TableMetaResponse]:
+        return await self._get(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}",
+            dict(offset=offset, limit=limit),
+            p.Page[p.TableMetaResponse],
+        )
+
+    async def delete_table(self, table_type: p.TableType, table_id: p.TableName) -> p.OkResponse:
+        return await self._delete(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/{quote(table_id)}",
+            None,
+            p.OkResponse,
+        )
+
+    async def duplicate_table(
+        self,
+        table_type: p.TableType,
+        table_id_src: str,
+        table_id_dst: str,
+        include_data: bool = True,
+        deploy: bool = False,
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/duplicate/{quote(table_id_src)}/{quote(table_id_dst)}",
+            None,
+            p.TableMetaResponse,
+            dict(include_data=include_data, deploy=deploy),
+        )
+
+    async def rename_table(
+        self, table_type: p.TableType, table_id_src: str, table_id_dst: str
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/rename/{quote(table_id_src)}/{quote(table_id_dst)}",
+            None,
+            p.TableMetaResponse,
+        )
+
+    async def update_gen_config(
+        self, table_type: p.TableType, request: p.GenConfigUpdateRequest
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/gen_config/update",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def add_action_columns(self, request: p.AddActionColumnSchema) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            "/v1/gen_tables/action/columns/add",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def add_knowledge_columns(
+        self, request: p.AddKnowledgeColumnSchema
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            "/v1/gen_tables/knowledge/columns/add",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def add_chat_columns(self, request: p.AddChatColumnSchema) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            "/v1/gen_tables/chat/columns/add",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def drop_columns(
+        self, table_type: p.TableType, request: p.ColumnDropRequest
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/columns/drop",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def rename_columns(
+        self, table_type: p.TableType, request: p.ColumnRenameRequest
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/columns/rename",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def reorder_columns(
+        self, table_type: p.TableType, request: p.ColumnReorderRequest
+    ) -> p.TableMetaResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/columns/reorder",
+            request,
+            p.TableMetaResponse,
+        )
+
+    async def list_table_rows(
+        self,
+        table_type: p.TableType,
+        table_id: p.TableName,
+        offset: int = 0,
+        limit: int = 100,
+        columns: list[p.Name] | None = None,
+    ) -> p.Page[dict[p.Name, Any]]:
+        return await self._get(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/{quote(table_id)}/rows",
+            dict(offset=offset, limit=limit, columns=columns),
+            p.Page[dict[p.Name, Any]],
+        )
+
+    async def get_table_row(
+        self,
+        table_type: p.TableType,
+        table_id: p.TableName,
+        row_id: str,
+        columns: list[p.Name] | None = None,
+    ) -> dict[p.Name, Any]:
+        response = await self._get(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/{quote(table_id)}/rows/{quote(row_id)}",
+            dict(columns=columns),
+            None,
+        )
+        return json_loads(response)
+
+    async def add_table_rows(
+        self, table_type: p.TableType, request: p.RowAddRequest
+    ) -> (
+        p.GenTableChatCompletionChunks
+        | AsyncGenerator[p.GenTableStreamReferences | p.GenTableStreamChatCompletionChunk, None]
+    ):
+        if request.stream:
+
+            async def gen():
+                references = None
+                async for chunk in self._stream(
+                    self.api_base,
+                    f"/v1/gen_tables/{table_type.value}/rows/add",
+                    request,
+                ):
+                    if references is None:
+                        try:
+                            references = p.GenTableStreamReferences.model_validate_json(chunk[5:])
+                            yield references
+                        except ValidationError:
+                            pass
+                    try:
+                        chunk_ = p.GenTableStreamChatCompletionChunk.model_validate_json(chunk[5:])
+                        yield chunk_
+                        continue
+                    except ValidationError:
+                        pass
+
+            return gen()
+        else:
+            return await self._post(
+                self.api_base,
+                f"/v1/gen_tables/{table_type.value}/rows/add",
+                request,
+                p.GenTableRowsChatCompletionChunks,
+            )
+
+    async def regen_table_rows(
+        self, table_type: p.TableType, request: p.RowRegenRequest
+    ) -> (
+        p.GenTableChatCompletionChunks
+        | AsyncGenerator[p.GenTableStreamReferences | p.GenTableStreamChatCompletionChunk, None]
+    ):
+        if request.stream:
+
+            async def gen():
+                references = None
+                async for chunk in self._stream(
+                    self.api_base,
+                    f"/v1/gen_tables/{table_type.value}/rows/regen",
+                    request,
+                ):
+                    if references is None:
+                        try:
+                            references = p.GenTableStreamReferences.model_validate_json(chunk[5:])
+                            yield references
+                        except ValidationError:
+                            pass
+                    try:
+                        chunk_ = p.GenTableStreamChatCompletionChunk.model_validate_json(chunk[5:])
+                        yield chunk_
+                        continue
+                    except ValidationError:
+                        pass
+
+            return gen()
+        else:
+            return await self._post(
+                self.api_base,
+                f"/v1/gen_tables/{table_type.value}/rows/regen",
+                request,
+                p.GenTableRowsChatCompletionChunks,
+            )
+
+    async def update_table_row(
+        self, table_type: p.TableType, request: p.RowUpdateRequest
+    ) -> p.OkResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/rows/update",
+            request,
+            p.OkResponse,
+        )
+
+    async def delete_table_rows(
+        self, table_type: p.TableType, request: p.RowDeleteRequest
+    ) -> p.OkResponse:
+        return await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/rows/delete",
+            request,
+            p.OkResponse,
+        )
+
+    async def delete_table_row(
+        self, table_type: p.TableType, table_id: p.TableName, row_id: str
+    ) -> p.OkResponse:
+        return await self._delete(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/{quote(table_id)}/rows/{quote(row_id)}",
+            None,
+            p.OkResponse,
+        )
+
+    async def get_conversation_thread(self, table_id: p.TableName) -> p.ChatThread:
+        return await self._get(
+            self.api_base,
+            f"/v1/gen_tables/chat/{quote(table_id)}/thread",
+            None,
+            p.ChatThread,
+        )
+
+    async def hybrid_search(
+        self,
+        table_type: p.TableType,
+        request: p.SearchRequest,
+    ) -> list[dict[p.Name, Any]]:
+        response = await self._post(
+            self.api_base,
+            f"/v1/gen_tables/{table_type.value}/hybrid_search",
+            request,
+            None,
+        )
+        return json_loads(response)
```

### Comparing `jamaibase-0.0.1/src/jamaibase/protocol.py` & `jamaibase-0.1.0/src/jamaibase/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1202,15 +1202,21 @@
                 if k.lower() in ("id", "updated at"):
                     continue
                 col = cols[k]
                 state = {}
                 if k in failed_cols:
                     d[k], state["original"] = None, d[k]
                 if d[k] is None:
-                    if col.dtype == DtypeEnum.str_:
+                    if col.dtype == DtypeEnum.int_:
+                        d[k] = 0
+                    elif col.dtype == DtypeEnum.float_:
+                        d[k] = 0.0
+                    elif col.dtype == DtypeEnum.bool_:
+                        d[k] = False
+                    elif col.dtype == DtypeEnum.str_:
                         # Store null string as ""
                         # https://github.com/lancedb/lancedb/issues/1160
                         d[k] = ""
                     elif col.vlen > 0:
                         # TODO: Investigate setting null vectors to np.nan
                         # Pros: nan vectors won't show up in vector search
                         # Cons: May cause error during vector indexing
```

### Comparing `jamaibase-0.0.1/src/jamaibase/utils/io.py` & `jamaibase-0.1.0/src/jamaibase/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from pprint import pformat
 from typing import Callable, Iterable
 
 import numpy as np
 import orjson
 import srsly
 import toml
-from jamaibase.utils.types import JSONInput, JSONOutput
 from PIL import ExifTags, Image
 
+from jamaibase.utils.types import JSONInput, JSONOutput
+
 logger = logging.getLogger(__name__)
 
 
 def load_pickle(file_path: str):
     with open(file_path, "rb") as f:
         return pickle.load(f)
 
@@ -45,15 +46,15 @@
 
 def dump_json(data: JSONInput, path: str, **kwargs) -> str:
     """Writes a JSON file.
 
     Args:
         data (JSONInput): The data.
         path (str): Path to the file.
-        **kwargs: Other keyword arguments to pass into `srsly.write_json`.
+        **kwargs: Other keyword arguments to pass into `orjson.dumps`.
 
     Returns:
         path (str): Path to the file.
     """
     with open(path, "wb") as f:
         f.write(orjson.dumps(data, **kwargs))
     return path
```

### Comparing `jamaibase-0.0.1/src/jamaibase/utils/versioning.py` & `jamaibase-0.1.0/src/jamaibase/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/src/jamaibase.egg-info/PKG-INFO` & `jamaibase-0.1.0/src/jamaibase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamaibase
-Version: 0.0.1
+Version: 0.1.0
 Summary: JamAI Base: Let Your Database Orchestrate LLMs and RAG
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: Unix
 Requires-Python: >=3.10
```

### Comparing `jamaibase-0.0.1/src/jamaibase.egg-info/SOURCES.txt` & `jamaibase-0.1.0/src/jamaibase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/src/jamaibase.egg-info/requires.txt` & `jamaibase-0.1.0/src/jamaibase.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/pdfloader__Swire_AR22_e_230406_sample.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/pdfloader__Swire_AR22_e_230406_sample.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/pdfloader__background-checks.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/pdfloader__background-checks.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/pdfloader__sample_tables.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/pdfloader__sample_tables.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/split_documents__Swire_AR22_e_230406_sample.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/split_documents__Swire_AR22_e_230406_sample.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/split_documents__background-checks.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/split_documents__background-checks.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/_loader_check/split_documents__sample_tables.pdf.json` & `jamaibase-0.1.0/tests/_loader_check/split_documents__sample_tables.pdf.json`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/case_embed_files.py` & `jamaibase-0.1.0/tests/case_embed_files.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/create_long_txt.py` & `jamaibase-0.1.0/tests/create_long_txt.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/docx/Recommendation Letter.docx` & `jamaibase-0.1.0/tests/docx/Recommendation Letter.docx`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/list_test_files_as_json.py` & `jamaibase-0.1.0/tests/list_test_files_as_json.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/Large Language Models as Optimizers [DeepMind ; 2023].pdf` & `jamaibase-0.1.0/tests/pdf/Large Language Models as Optimizers [DeepMind ; 2023].pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/Swire_AR22_e_230406_sample.pdf` & `jamaibase-0.1.0/tests/pdf/Swire_AR22_e_230406_sample.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/System Design Blueprint - The Ultimate Guide.pdf` & `jamaibase-0.1.0/tests/pdf/System Design Blueprint - The Ultimate Guide.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/Vehicle Detail - MyPUSPAKOM.pdf` & `jamaibase-0.1.0/tests/pdf/Vehicle Detail - MyPUSPAKOM.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/ag-energy-round-up-2017-02-24.pdf` & `jamaibase-0.1.0/tests/pdf/ag-energy-round-up-2017-02-24.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/background-checks.pdf` & `jamaibase-0.1.0/tests/pdf/background-checks.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/ca-warn-report.pdf` & `jamaibase-0.1.0/tests/pdf/ca-warn-report.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/salary 总结.pdf` & `jamaibase-0.1.0/tests/pdf/salary 总结.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/sample_tables.pdf` & `jamaibase-0.1.0/tests/pdf/sample_tables.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/san-jose-pd-firearm-sample.pdf` & `jamaibase-0.1.0/tests/pdf/san-jose-pd-firearm-sample.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/statement_card.pdf` & `jamaibase-0.1.0/tests/pdf/statement_card.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pdf/statement_ewallet.pdf` & `jamaibase-0.1.0/tests/pdf/statement_ewallet.pdf`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/populate_test_documents_minio.py` & `jamaibase-0.1.0/tests/populate_test_documents_minio.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/pptx/(2017.06.30) Neural Machine Translation in Linear Time (ByteNet).pptx` & `jamaibase-0.1.0/tests/pptx/(2017.06.30) Neural Machine Translation in Linear Time (ByteNet).pptx`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/test_chat.py` & `jamaibase-0.1.0/tests/test_chat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,117 +1,148 @@
-from typing import Type
+from asyncio.coroutines import iscoroutine
+from typing import AsyncGenerator, Generator, Type
 
 import pytest
 from flaky import flaky
+from loguru import logger
 
-from jamaibase import JamAI
+from jamaibase import JamAI, JamAIAsync
 from jamaibase import protocol as p
 
-CLIENT_CLS = [JamAI]
+CLIENT_CLS = [JamAI, JamAIAsync]
+
+
+async def run(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if iscoroutine(ret):
+        return await ret
+    return ret
+
+
+async def run_gen_async(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if iscoroutine(ret):
+        ret = await ret
+    if isinstance(ret, AsyncGenerator):
+        async for item in ret:
+            yield item
+    else:
+        yield ret
+
+
+def run_gen_sync(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if isinstance(ret, Generator):
+        for item in ret:
+            yield item
+    else:
+        yield ret
 
 
 @pytest.mark.parametrize("client_cls", CLIENT_CLS)
-def test_model_info(client_cls: Type[JamAI]):
+async def test_model_info(client_cls: Type[JamAI | JamAIAsync]):
     jamai = client_cls(project_id="", api_key="")
-    response = jamai.model_info()
+    response = await run(jamai.model_info)
 
     # Get all model info
     assert isinstance(response, p.ModelInfoResponse)
     assert len(response.data) > 0
     assert isinstance(response.data[0], p.ModelInfo)
     model = response.data[0]
     assert isinstance(model.id, str)
     assert isinstance(model.context_length, int)
     assert model.context_length > 0
     assert isinstance(model.languages, list)
     assert len(model.languages) > 0
 
     # Get specific model info
-    response = jamai.model_info(name=model.id)
+    response = await run(jamai.model_info, name=model.id)
     assert isinstance(response, p.ModelInfoResponse)
     assert len(response.data) == 1
     assert response.data[0].id == model.id
 
     # Filter based on capability
-    response = jamai.model_info(capabilities=["chat"])
+    response = await run(jamai.model_info, capabilities=["chat"])
     assert isinstance(response, p.ModelInfoResponse)
     for m in response.data:
         assert "chat" in m.capabilities
         assert "embed" not in m.capabilities
         assert "rerank" not in m.capabilities
 
-    response = jamai.model_info(capabilities=["chat", "image"])
+    response = await run(jamai.model_info, capabilities=["chat", "image"])
     assert isinstance(response, p.ModelInfoResponse)
     for m in response.data:
         assert "chat" in m.capabilities
         assert "image" in m.capabilities
         assert "embed" not in m.capabilities
         assert "rerank" not in m.capabilities
 
-    response = jamai.model_info(capabilities=["embed"])
+    response = await run(jamai.model_info, capabilities=["embed"])
     assert isinstance(response, p.ModelInfoResponse)
     for m in response.data:
         assert "chat" not in m.capabilities
         assert "embed" in m.capabilities
         assert "rerank" not in m.capabilities
 
-    response = jamai.model_info(capabilities=["rerank"])
+    response = await run(jamai.model_info, capabilities=["rerank"])
     assert isinstance(response, p.ModelInfoResponse)
     for m in response.data:
         assert "chat" not in m.capabilities
         assert "embed" not in m.capabilities
         assert "rerank" in m.capabilities
 
 
 @pytest.mark.parametrize("client_cls", CLIENT_CLS)
-def test_model_names(client_cls: Type[JamAI]):
+async def test_model_names(client_cls: Type[JamAI | JamAIAsync]):
     jamai = client_cls(project_id="", api_key="")
-    response = jamai.model_names()
+    response = await run(jamai.model_names)
+    logger.info(f"response: {response}")
+    logger.info(f"type(response): {type(response)}")
 
     # Get all model info
     assert isinstance(response, list)
     assert len(response) > 0
     assert all(isinstance(r, str) for r in response)
     model = response[0]
 
     # Get specific model info
-    response = jamai.model_names(prefer=model)
+    response = await run(jamai.model_names, prefer=model)
     assert isinstance(response, list)
     assert len(response) > 0
     assert response[0] == model
 
     # Preferred model can be non-existent
-    response = jamai.model_names(prefer="dummy")
+    response = await run(jamai.model_names, prefer="dummy")
     assert isinstance(response, list)
     assert len(response) > 0
     assert isinstance(response[0], str)
 
     # Filter based on capability
-    response = jamai.model_names(capabilities=["chat"])
+    response = await run(jamai.model_names, capabilities=["chat"])
     assert isinstance(response, list)
     name_cat = ",".join(response)
     assert "gpt-3.5-turbo" in name_cat
     assert "embedding" not in name_cat
     assert "rerank" not in name_cat
 
-    response = jamai.model_names(capabilities=["chat", "image"])
+    response = await run(jamai.model_names, capabilities=["chat", "image"])
     assert isinstance(response, list)
     name_cat = ",".join(response)
     assert "gpt-4" in name_cat
     assert "embedding" not in name_cat
     assert "rerank" not in name_cat
 
-    response = jamai.model_names(capabilities=["embed"])
+    response = await run(jamai.model_names, capabilities=["embed"])
     assert isinstance(response, list)
     name_cat = ",".join(response)
     assert "gpt-3.5-turbo" not in name_cat
     assert "embedding" in name_cat
     assert "rerank" not in name_cat
 
-    response = jamai.model_names(capabilities=["rerank"])
+    response = await run(jamai.model_names, capabilities=["rerank"])
     assert isinstance(response, list)
     name_cat = ",".join(response)
     assert "gpt-3.5-turbo" not in name_cat
     assert "embedding" not in name_cat
     assert "rerank" in name_cat
 
 
@@ -141,30 +172,38 @@
         selected.append([m for m in models if m.startswith(provider)][0])
     return selected
 
 
 @flaky(max_runs=3, min_passes=1)
 @pytest.mark.parametrize("client_cls", CLIENT_CLS)
 @pytest.mark.parametrize("model", _get_models())
-def test_chat_completion(client_cls: Type[JamAI], model: str):
+async def test_chat_completion(client_cls: Type[JamAI | JamAIAsync], model: str):
     jamai = client_cls(project_id="", api_key="")
 
     # Non-streaming
     request = _get_chat_request(model, stream=False)
-    response = jamai.generate_chat_completions(request)
+    if isinstance(jamai, JamAIAsync):
+        response = [r async for r in run_gen_async(jamai.generate_chat_completions, request)]
+    else:
+        response = [r for r in run_gen_sync(jamai.generate_chat_completions, request)]
+    assert len(response) == 1
+    response = response[0]
     assert isinstance(response, p.ChatCompletionChunk)
     assert isinstance(response.text, str)
     assert len(response.text) > 1
     assert isinstance(response.prompt_tokens, int)
     assert isinstance(response.completion_tokens, int)
     assert response.references is None
 
     # Streaming
     request.stream = True
-    responses = [r for r in jamai.generate_chat_completions(request)]
+    if isinstance(jamai, JamAIAsync):
+        responses = [r async for r in run_gen_async(jamai.generate_chat_completions, request)]
+    else:
+        responses = [r for r in run_gen_sync(jamai.generate_chat_completions, request)]
     assert len(responses) > 0
     assert all(isinstance(r, p.ChatCompletionChunk) for r in responses)
     assert all(isinstance(r.text, str) for r in responses)
     assert all(r.references is None for r in responses)
 
 
 # def pdf_s3files():
```

### Comparing `jamaibase-0.0.1/tests/test_gen_executor.py` & `jamaibase-0.1.0/tests/test_gen_executor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,59 @@
 import random
 import time
+from asyncio.coroutines import iscoroutine
+from typing import AsyncGenerator, Generator, Type
 
 import pytest
 from loguru import logger
 
-from jamaibase import JamAI
+from jamaibase import JamAI, JamAIAsync
 from jamaibase.protocol import (
     ColumnSchemaCreate,
     GenConfigUpdateRequest,
+    GenTableRowsChatCompletionChunks,
     RowAddRequest,
     RowRegenRequest,
     TableSchemaCreate,
     TableType,
 )
 
+CLIENT_CLS = [JamAI, JamAIAsync]
 GEN_TYPES = ["REGEN"]
 
 
-@pytest.fixture
-def jamai_client():
-    yield JamAI()
+async def run(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if iscoroutine(ret):
+        return await ret
+    return ret
 
 
-def _create_table(
-    jamai_client: JamAI,
+async def run_gen_async(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if iscoroutine(ret):
+        ret = await ret
+    if isinstance(ret, AsyncGenerator):
+        async for item in ret:
+            yield item
+    else:
+        yield ret
+
+
+def run_gen_sync(fn, *args, **kwargs):
+    ret = fn(*args, **kwargs)
+    if isinstance(ret, Generator):
+        for item in ret:
+            yield item
+    else:
+        yield ret
+
+
+async def _create_table(
+    jamai: JamAI | JamAIAsync,
     table_type: TableType,
     cols_info: tuple[dict[str, str], dict[str, str]] = None,
 ):
     table_id = f"{table_type.value}_{random.randint(10000, 99999)}"
     schema = TableSchemaCreate(
         id=table_id,
         cols=(
@@ -39,24 +65,24 @@
             else (
                 [ColumnSchemaCreate(id=k, dtype=v) for k, v in cols_info[0].items()]
                 + [ColumnSchemaCreate(id=k, dtype=v) for k, v in cols_info[1].items()]
             )
         ),
     )
     if table_type == TableType.action:
-        table = jamai_client.create_action_table(schema)
+        table = await run(jamai.create_action_table, schema)
     else:
         raise ValueError(f"Invalid table type: {table_type}")
     return table, table_id
 
 
-def _update_gen_config(
-    jamai_client: JamAI, table_type: TableType, gen_config: GenConfigUpdateRequest
+async def _update_gen_config(
+    jamai: JamAI | JamAIAsync, table_type: TableType, gen_config: GenConfigUpdateRequest
 ):
-    jamai_client.update_gen_config(table_type, gen_config)
+    await run(jamai.update_gen_config, table_type, gen_config)
 
 
 # ---------------------------------------------------------
 # Test Cases for concurrent Execution
 # ---------------------------------------------------------
 def column_map_prompt(content: str, max_tokens: int):
     return {
@@ -82,22 +108,22 @@
         "stop": [],
         "max_tokens": max_tokens,
     }
 
 
 def data():
     input_dict = {"xx": "str", "yy": "str", "zz": "str"}
-    # output_dict = {
-    #     "aa": "str",
-    #     "bb": "str",
-    #     "cc": "str",
-    #     "dd": "str",
-    #     "ee": "str",
-    #     "ff": "str",
-    # }
+    output_dict = {
+        "aa": "str",
+        "bb": "str",
+        "cc": "str",
+        "dd": "str",
+        "ee": "str",
+        "ff": "str",
+    }
     output_dict2 = {
         "aa": "str",
         "bb": "str",
         "cc": "str",
         # ---
         "dd": "str",
         "ee": "str",
@@ -113,87 +139,87 @@
         "ee3": "str",
         "ff3": "str",
         "dd23": "str",
         "ee23": "str",
         "ff23": "str",
     }
     row = {"xx": "1", "yy": "2", "zz": "3"}
-    # inv_nodes = [  # map - end: (start, expected_gen_output)
-    #     # {
-    #     #     "aa": (["xx"], "<xx:1>"),
-    #     #     "bb": (["yy"], "<yy:2>"),
-    #     #     "cc": (["zz"], "<zz:3>"),
-    #     #     # "dd": (["xx"], "<xx:1>"),
-    #     #     # "ee": (["yy"], "<yy:2>"),
-    #     #     # "ff": (["zz"], "<zz:3>"),
-    #     # },
-    #     {
-    #         "aa": (["xx"], "<xx:1>"),
-    #         "bb": (["yy"], "<yy:2>"),
-    #         "cc": (["zz"], "<zz:3>"),
-    #         "dd": (["aa"], "<aa:<xx:1>>"),
-    #         "ee": (["bb"], "<bb:<yy:2>>"),
-    #         "ff": (["cc"], "<cc:<zz:3>>"),
-    #     },
-    #     # {
-    #     #     "aa": (["xx"], "<xx:1>"),
-    #     #     "bb": (["yy"], "<yy:2>"),
-    #     #     "cc": (["zz"], "<zz:3>"),
-    #     #     "dd": (["aa", "bb"], "(<aa:<xx:1>> & <bb:<yy:2>>)"),
-    #     #     "ee": (["cc"], "<cc:<zz:3>>"),
-    #     #     "ff": (
-    #     #         ["dd", "ee"],
-    #     #         "(<dd:(<aa:<xx:1>> & <bb:<yy:2>>)> & <ee:<cc:<zz:3>>>)",
-    #     #     ),
-    #     # },
-    #     # {
-    #     #     "aa": (["xx"], "<xx:1>"),
-    #     #     "bb": (["yy"], "<yy:2>"),
-    #     #     "cc": (["zz"], "<zz:3>"),
-    #     #     "dd": (["aa", "bb"], "(<aa:<xx:1>> & <bb:<yy:2>>)"),
-    #     #     "ee": (["cc", "dd"], "(<cc:<zz:3>> & <dd:(<aa:<xx:1>> & <bb:<yy:2>>)>)"),
-    #     #     "ff": (
-    #     #         ["dd", "ee"],
-    #     #         "(<dd:(<aa:<xx:1>> & <bb:<yy:2>>)> & <ee:(<cc:<zz:3>> & <dd:(<aa:<xx:1>> & <bb:<yy:2>>)>)>)",
-    #     #     ),
-    #     # },
-    #     # {
-    #     #     "aa": (["xx", "yy"], "(<xx:1> & <yy:2>)"),
-    #     #     "bb": (["aa"], "<aa:(<xx:1> & <yy:2>)>"),
-    #     #     "cc": (["zz", "bb"], "(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)"),
-    #     #     "dd": (["cc"], "<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>"),
-    #     #     "ee": (
-    #     #         ["cc", "dd"],
-    #     #         "(<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>>)",
-    #     #     ),
-    #     #     "ff": (
-    #     #         ["aa", "bb", "cc", "dd", "ee"],
-    #     #         "(<aa:(<xx:1> & <yy:2>)> & <bb:<aa:(<xx:1> & <yy:2>)>> & <cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>> & <ee:(<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>>)>)",
-    #     #     ),
-    #     # },
-    #     # {
-    #     #     "aa": (["xx", "yy", "zz"], "(<xx:1> & <yy:2> & <zz:3>)"),
-    #     #     "bb": (["aa"], "<aa:(<xx:1> & <yy:2> & <zz:3>)>"),
-    #     #     "cc": (["bb"], "<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>"),
-    #     #     "dd": (["cc"], "<cc:<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>>"),
-    #     #     "ee": (["yy", "zz"], "(<yy:2> & <zz:3>)"),
-    #     #     "ff": (
-    #     #         ["dd", "ee"],
-    #     #         "(<dd:<cc:<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>>> & <ee:(<yy:2> & <zz:3>)>)",
-    #     #     ),
-    #     # },
-    #     # {
-    #     #     "aa": (["xx"], "<xx:1>"),
-    #     #     "bb": (["yy"], "<yy:2>"),
-    #     #     "cc": (["zz"], "<zz:3>"),
-    #     #     "dd": (["xx"], "<xx:1>"),
-    #     #     "ee": (["yy"], "<yy:2>"),
-    #     #     "ff": (["zz"], "<zz:3>"),
-    #     # },
-    # ]
+    inv_nodes = [  # map - end: (start, expected_gen_output)
+        # {
+        #     "aa": (["xx"], "<xx:1>"),
+        #     "bb": (["yy"], "<yy:2>"),
+        #     "cc": (["zz"], "<zz:3>"),
+        #     # "dd": (["xx"], "<xx:1>"),
+        #     # "ee": (["yy"], "<yy:2>"),
+        #     # "ff": (["zz"], "<zz:3>"),
+        # },
+        {
+            "aa": (["xx"], "<xx:1>"),
+            "bb": (["yy"], "<yy:2>"),
+            "cc": (["zz"], "<zz:3>"),
+            "dd": (["aa"], "<aa:<xx:1>>"),
+            "ee": (["bb"], "<bb:<yy:2>>"),
+            "ff": (["cc"], "<cc:<zz:3>>"),
+        },
+        # {
+        #     "aa": (["xx"], "<xx:1>"),
+        #     "bb": (["yy"], "<yy:2>"),
+        #     "cc": (["zz"], "<zz:3>"),
+        #     "dd": (["aa", "bb"], "(<aa:<xx:1>> & <bb:<yy:2>>)"),
+        #     "ee": (["cc"], "<cc:<zz:3>>"),
+        #     "ff": (
+        #         ["dd", "ee"],
+        #         "(<dd:(<aa:<xx:1>> & <bb:<yy:2>>)> & <ee:<cc:<zz:3>>>)",
+        #     ),
+        # },
+        # {
+        #     "aa": (["xx"], "<xx:1>"),
+        #     "bb": (["yy"], "<yy:2>"),
+        #     "cc": (["zz"], "<zz:3>"),
+        #     "dd": (["aa", "bb"], "(<aa:<xx:1>> & <bb:<yy:2>>)"),
+        #     "ee": (["cc", "dd"], "(<cc:<zz:3>> & <dd:(<aa:<xx:1>> & <bb:<yy:2>>)>)"),
+        #     "ff": (
+        #         ["dd", "ee"],
+        #         "(<dd:(<aa:<xx:1>> & <bb:<yy:2>>)> & <ee:(<cc:<zz:3>> & <dd:(<aa:<xx:1>> & <bb:<yy:2>>)>)>)",
+        #     ),
+        # },
+        # {
+        #     "aa": (["xx", "yy"], "(<xx:1> & <yy:2>)"),
+        #     "bb": (["aa"], "<aa:(<xx:1> & <yy:2>)>"),
+        #     "cc": (["zz", "bb"], "(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)"),
+        #     "dd": (["cc"], "<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>"),
+        #     "ee": (
+        #         ["cc", "dd"],
+        #         "(<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>>)",
+        #     ),
+        #     "ff": (
+        #         ["aa", "bb", "cc", "dd", "ee"],
+        #         "(<aa:(<xx:1> & <yy:2>)> & <bb:<aa:(<xx:1> & <yy:2>)>> & <cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>> & <ee:(<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)> & <dd:<cc:(<zz:3> & <bb:<aa:(<xx:1> & <yy:2>)>>)>>)>)",
+        #     ),
+        # },
+        # {
+        #     "aa": (["xx", "yy", "zz"], "(<xx:1> & <yy:2> & <zz:3>)"),
+        #     "bb": (["aa"], "<aa:(<xx:1> & <yy:2> & <zz:3>)>"),
+        #     "cc": (["bb"], "<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>"),
+        #     "dd": (["cc"], "<cc:<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>>"),
+        #     "ee": (["yy", "zz"], "(<yy:2> & <zz:3>)"),
+        #     "ff": (
+        #         ["dd", "ee"],
+        #         "(<dd:<cc:<bb:<aa:(<xx:1> & <yy:2> & <zz:3>)>>>> & <ee:(<yy:2> & <zz:3>)>)",
+        #     ),
+        # },
+        # {
+        #     "aa": (["xx"], "<xx:1>"),
+        #     "bb": (["yy"], "<yy:2>"),
+        #     "cc": (["zz"], "<zz:3>"),
+        #     "dd": (["xx"], "<xx:1>"),
+        #     "ee": (["yy"], "<yy:2>"),
+        #     "ff": (["zz"], "<zz:3>"),
+        # },
+    ]
     inv_nodes2 = [  # map - end: (start, expected_gen_output)
         {
             "aa": (["xx"], "<xx:1>"),
             "bb": (["yy"], "<yy:2>"),
             "cc": (["zz"], "<zz:3>"),
             # ---
             "dd": (["aa"], "<aa:<xx:1>>"),
@@ -258,275 +284,538 @@
 
     content_postfix = "Output exactly the content above, don't include any other information."
     # content_postfix2 = "Output exactly the content above, don't include any other information. Then create a story."
     # all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix2, max_tokens=5)
     # all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix2, max_tokens=1000)
     # all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix2, max_tokens=500)
     # all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix2, max_tokens=300)
-    all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix, max_tokens=100)
-    # all_nodes_data = get_nodes_data(inv_nodes, output_dict, content_postfix, max_tokens=100)
+    # all_nodes_data = get_nodes_data(inv_nodes2, output_dict2, content_postfix, max_tokens=100)
+    all_nodes_data = get_nodes_data(inv_nodes, output_dict, content_postfix, max_tokens=100)
     # all_nodes_data = get_nodes_data(inv_nodes, output_dict, content_postfix2, max_tokens=300)
     return all_nodes_data
 
 
+@pytest.mark.parametrize("client_cls", CLIENT_CLS)
 @pytest.mark.parametrize("gen_type", GEN_TYPES)
 @pytest.mark.parametrize("input_dict, output_dict, column_map, row, expected_column_gen", data())
-def test_nonstream_concurrent_execution(
-    jamai_client: JamAI, gen_type, input_dict, output_dict, column_map, row, expected_column_gen
+async def test_nonstream_concurrent_execution(
+    client_cls: JamAI | JamAIAsync,
+    gen_type,
+    input_dict,
+    output_dict,
+    column_map,
+    row,
+    expected_column_gen,
 ):
     """
     Tests concurrent execution in non-streaming mode with dependencies.
     """
-    meta, table_id = _create_table(
-        jamai_client,
+    jamai = client_cls(project_id="", api_key="")
+    meta, table_id = await _create_table(
+        jamai,
         TableType.action,
         cols_info=(
             input_dict,
             output_dict,
         ),
     )
     gen_config = GenConfigUpdateRequest(table_id=table_id, column_map=column_map)
-    _update_gen_config(jamai_client, TableType.action, gen_config)
+    await _update_gen_config(jamai, TableType.action, gen_config)
 
-    response = jamai_client.add_table_rows(
-        TableType.action,
-        RowAddRequest(table_id=table_id, data=[row], stream=False, concurrent=True),
-    )
+    if isinstance(jamai, JamAIAsync):
+        response = [
+            r
+            async for r in run_gen_async(
+                jamai.add_table_rows,
+                TableType.action,
+                RowAddRequest(table_id=table_id, data=[row], stream=False, concurrent=True),
+            )
+        ]
+
+    else:
+        response = [
+            r
+            for r in run_gen_sync(
+                jamai.add_table_rows,
+                TableType.action,
+                RowAddRequest(table_id=table_id, data=[row], stream=False, concurrent=True),
+            )
+        ]
+
+    response = response[0]
+    assert isinstance(response, GenTableRowsChatCompletionChunks)
 
     # Verify all output columns were executed
     for response in response.rows:
         for output_column_name in output_dict.keys():
             assert output_column_name in response.columns
 
     if gen_type == "REGEN":
-        rows = jamai_client.list_table_rows(TableType.action, table_id)
+        rows = await run(jamai.list_table_rows, TableType.action, table_id)
         row_id = rows.items[0]["ID"]
-        response = jamai_client.regen_table_rows(
-            TableType.action,
-            RowRegenRequest(table_id=table_id, row_ids=[row_id], stream=False, concurrent=True),
-        )
+        if isinstance(jamai, JamAIAsync):
+            response = [
+                r
+                async for r in run_gen_async(
+                    jamai.regen_table_rows,
+                    TableType.action,
+                    RowRegenRequest(
+                        table_id=table_id, row_ids=[row_id], stream=False, concurrent=True
+                    ),
+                )
+            ]
+
+        else:
+            response = [
+                r
+                for r in run_gen_sync(
+                    jamai.regen_table_rows,
+                    TableType.action,
+                    RowRegenRequest(
+                        table_id=table_id, row_ids=[row_id], stream=False, concurrent=True
+                    ),
+                )
+            ]
+    response = response[0]
+    assert isinstance(response, GenTableRowsChatCompletionChunks)
 
     # Get rows
-    rows = jamai_client.list_table_rows(TableType.action, table_id)
+    rows = await run(jamai.list_table_rows, TableType.action, table_id)
     for i in range(len(response.rows)):
         row_id = rows.items[i]["ID"]
-        row = jamai_client.get_table_row(TableType.action, table_id, row_id)
+        row = await run(jamai.get_table_row, TableType.action, table_id, row_id)
 
         # Compare generated outputs with expected outputs
         for output_column_name in output_dict.keys():
             expected_gen = expected_column_gen[output_column_name]
             column_gen = row[output_column_name]["value"]
             len_expected_gen = len(expected_gen)
             len_column_gen = len(column_gen)
             if len_column_gen >= len_expected_gen:
                 assert column_gen[:len_expected_gen] == expected_gen
             else:
                 assert column_gen == expected_gen[:len_column_gen]
 
-    jamai_client.delete_table(TableType.action, table_id)
+    await run(jamai.delete_table, TableType.action, table_id)
 
 
+@pytest.mark.parametrize("client_cls", CLIENT_CLS)
 @pytest.mark.parametrize("gen_type", GEN_TYPES)
 @pytest.mark.parametrize("input_dict, output_dict, column_map, row, expected_column_gen", data())
-def test_stream_concurrent_execution(
-    jamai_client: JamAI, gen_type, input_dict, output_dict, column_map, row, expected_column_gen
+async def test_stream_concurrent_execution(
+    client_cls: JamAI | JamAIAsync,
+    gen_type,
+    input_dict,
+    output_dict,
+    column_map,
+    row,
+    expected_column_gen,
 ):
     """
     Tests concurrent execution in streaming mode with dependencies.
     """
-    meta, table_id = _create_table(
-        jamai_client,
+    jamai = client_cls(project_id="", api_key="")
+    meta, table_id = await _create_table(
+        jamai,
         TableType.action,
         cols_info=(
             input_dict,
             output_dict,
         ),
     )
     gen_config = GenConfigUpdateRequest(table_id=table_id, column_map=column_map)
-    _update_gen_config(jamai_client, TableType.action, gen_config)
-
-    response = jamai_client.add_table_rows(
-        TableType.action,
-        RowAddRequest(table_id=table_id, data=[row], stream=True, concurrent=True),
-    )
+    await _update_gen_config(jamai, TableType.action, gen_config)
 
-    # Collect streaming response
+    total_start_time = time.time()
+    first_chunk_times = {}
     chunks = []
-    for chunk in response:
-        chunks.append(chunk)
+    if isinstance(jamai, JamAIAsync):
+        async for chunk in run_gen_async(
+            jamai.add_table_rows,
+            TableType.action,
+            RowAddRequest(
+                table_id=table_id,
+                data=[row],
+                stream=True,
+                concurrent=True,
+            ),
+        ):
+            chunks.append(chunk)
+            if chunk.row_id not in first_chunk_times.keys():
+                first_chunk_times[chunk.row_id] = {}
+            if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                    time.time() - total_start_time
+                )
+
+    else:
+        for chunk in run_gen_sync(
+            jamai.add_table_rows,
+            TableType.action,
+            RowAddRequest(
+                table_id=table_id,
+                data=[row],
+                stream=True,
+                concurrent=True,
+            ),
+        ):
+            chunks.append(chunk)
+            if chunk.row_id not in first_chunk_times.keys():
+                first_chunk_times[chunk.row_id] = {}
+            if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                    time.time() - total_start_time
+                )
+
+    for row_id_ in first_chunk_times.keys():
+        for output_column_name in first_chunk_times[row_id_].keys():
+            logger.debug(
+                f"> [Test] Time to first chunk for {output_column_name}: {first_chunk_times[row_id_].get(output_column_name, 'N/A'):.2f} seconds"
+            )
+        break
+
+    logger.debug(
+        f"> [Test] Stream Total Add Rows Time: {time.time() - total_start_time:.2f} seconds"
+    )
 
     if gen_type == "REGEN":
-        rows = jamai_client.list_table_rows(TableType.action, table_id)
-        # logger.info(f"rows.items: {rows.items}")
+        rows = await run(jamai.list_table_rows, TableType.action, table_id)
         row_id = rows.items[0]["ID"]
         total_start_time = time.time()
-        response = jamai_client.regen_table_rows(
-            TableType.action,
-            RowRegenRequest(table_id=table_id, row_ids=[row_id], stream=True, concurrent=True),
-        )
-        # Collect streaming response
+        first_chunk_times = {}
         chunks = []
-        for chunk in response:
-            chunks.append(chunk)
-        logger.info(f"> Total Regen Rows Time: {time.time() - total_start_time}")
+        if isinstance(jamai, JamAIAsync):
+            async for chunk in run_gen_async(
+                jamai.regen_table_rows,
+                TableType.action,
+                RowRegenRequest(
+                    table_id=table_id,
+                    row_ids=[row_id],
+                    stream=True,
+                    concurrent=True,
+                ),
+            ):
+                chunks.append(chunk)
+                if chunk.row_id not in first_chunk_times.keys():
+                    first_chunk_times[chunk.row_id] = {}
+                if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                    first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                        time.time() - total_start_time
+                    )
+
+        else:
+            for chunk in run_gen_sync(
+                jamai.regen_table_rows,
+                TableType.action,
+                RowRegenRequest(
+                    table_id=table_id,
+                    row_ids=[row_id],
+                    stream=True,
+                    concurrent=True,
+                ),
+            ):
+                chunks.append(chunk)
+                if chunk.row_id not in first_chunk_times.keys():
+                    first_chunk_times[chunk.row_id] = {}
+                if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                    first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                        time.time() - total_start_time
+                    )
+
+        for row_id_ in first_chunk_times.keys():
+            for output_column_name in first_chunk_times[row_id_].keys():
+                logger.debug(
+                    f"> [Test] Time to first chunk for {output_column_name}: {first_chunk_times[row_id_].get(output_column_name, 'N/A'):.2f} seconds"
+                )
+            break
+
+        logger.debug(
+            f"> [Test] Stream Total Regen Rows Time: {time.time() - total_start_time:.2f} seconds"
+        )
 
     # Get first rows
-    rows = jamai_client.list_table_rows(TableType.action, table_id)
+    rows = await run(jamai.list_table_rows, TableType.action, table_id)
     row_id = rows.items[0]["ID"]
-    row = jamai_client.get_table_row(TableType.action, table_id, row_id)
+    row = await run(jamai.get_table_row, TableType.action, table_id, row_id)
 
     # Compare generated outputs with expected outputs
     for output_column_name in output_dict.keys():
         expected_gen = expected_column_gen[output_column_name]
         column_gen = row[output_column_name]["value"]
         len_expected_gen = len(expected_gen)
         len_column_gen = len(column_gen)
         if len_column_gen >= len_expected_gen:
             assert column_gen[:len_expected_gen] == expected_gen
         else:
             assert column_gen == expected_gen[:len_column_gen]
 
-    jamai_client.delete_table(TableType.action, table_id)
+    await run(jamai.delete_table, TableType.action, table_id)
 
 
+@pytest.mark.parametrize("client_cls", CLIENT_CLS)
 @pytest.mark.parametrize("gen_type", GEN_TYPES)
 @pytest.mark.parametrize("input_dict, output_dict, column_map, row, expected_column_gen", data())
-def test_multirows_nonstream_concurrent_execution(
-    jamai_client: JamAI, gen_type, input_dict, output_dict, column_map, row, expected_column_gen
+async def test_multirows_nonstream_concurrent_execution(
+    client_cls: JamAI | JamAIAsync,
+    gen_type,
+    input_dict,
+    output_dict,
+    column_map,
+    row,
+    expected_column_gen,
 ):
     """
     Tests concurrent execution in non-streaming mode with dependencies.
     """
-    meta, table_id = _create_table(
-        jamai_client,
+    jamai = client_cls(project_id="", api_key="")
+    meta, table_id = await _create_table(
+        jamai,
         TableType.action,
         cols_info=(
             input_dict,
             output_dict,
         ),
     )
     gen_config = GenConfigUpdateRequest(table_id=table_id, column_map=column_map)
-    _update_gen_config(jamai_client, TableType.action, gen_config)
+    await _update_gen_config(jamai, TableType.action, gen_config)
 
     total_start_time = time.time()
-    response = jamai_client.add_table_rows(
-        TableType.action,
-        RowAddRequest(
-            table_id=table_id,
-            data=[row, row, row],
-            stream=False,
-            concurrent=True,
-        ),
-    )
+    if isinstance(jamai, JamAIAsync):
+        response = [
+            r
+            async for r in run_gen_async(
+                jamai.add_table_rows,
+                TableType.action,
+                RowAddRequest(
+                    table_id=table_id, data=[row, row, row], stream=False, concurrent=True
+                ),
+            )
+        ]
+
+    else:
+        response = [
+            r
+            for r in run_gen_sync(
+                jamai.add_table_rows,
+                TableType.action,
+                RowAddRequest(
+                    table_id=table_id, data=[row, row, row], stream=False, concurrent=True
+                ),
+            )
+        ]
+
+    response = response[0]
+    assert isinstance(response, GenTableRowsChatCompletionChunks)
     logger.debug(f"> Non-Stream Total Rows Time: {time.time() - total_start_time}")
 
     # Verify all output columns were executed
     for response in response.rows:
         for output_column_name in output_dict.keys():
             assert output_column_name in response.columns
 
     if gen_type == "REGEN":
         total_start_time = time.time()
-        rows = jamai_client.list_table_rows(TableType.action, table_id)
-        response = jamai_client.regen_table_rows(
-            TableType.action,
-            RowRegenRequest(
-                table_id=table_id,
-                row_ids=[row_item["ID"] for row_item in rows.items],
-                stream=False,
-                concurrent=True,
-            ),
-        )
-        logger.debug(f"> Non-Stream Total Regen Rows Time: {time.time() - total_start_time}")
+        rows = await run(jamai.list_table_rows, TableType.action, table_id)
+        if isinstance(jamai, JamAIAsync):
+            response = [
+                r
+                async for r in run_gen_async(
+                    jamai.regen_table_rows,
+                    TableType.action,
+                    RowRegenRequest(
+                        table_id=table_id,
+                        row_ids=[row_item["ID"] for row_item in rows.items],
+                        stream=False,
+                        concurrent=True,
+                    ),
+                )
+            ]
+
+        else:
+            response = [
+                r
+                for r in run_gen_sync(
+                    jamai.regen_table_rows,
+                    TableType.action,
+                    RowRegenRequest(
+                        table_id=table_id,
+                        row_ids=[row_item["ID"] for row_item in rows.items],
+                        stream=False,
+                        concurrent=True,
+                    ),
+                )
+            ]
+    response = response[0]
+    assert isinstance(response, GenTableRowsChatCompletionChunks)
+    logger.debug(f"> Non-Stream Total Regen Rows Time: {time.time() - total_start_time}")
 
     # Get rows
-    rows = jamai_client.list_table_rows(TableType.action, table_id)
+    rows = await run(jamai.list_table_rows, TableType.action, table_id)
     for i in range(len(response.rows)):
         row_id = rows.items[i]["ID"]
-        row = jamai_client.get_table_row(TableType.action, table_id, row_id)
+        row = await run(jamai.get_table_row, TableType.action, table_id, row_id)
 
         # Compare generated outputs with expected outputs
         for output_column_name in output_dict.keys():
             expected_gen = expected_column_gen[output_column_name]
             column_gen = row[output_column_name]["value"]
             len_expected_gen = len(expected_gen)
             len_column_gen = len(column_gen)
             if len_column_gen >= len_expected_gen:
                 assert column_gen[:len_expected_gen] == expected_gen
             else:
                 assert column_gen == expected_gen[:len_column_gen]
 
-    jamai_client.delete_table(TableType.action, table_id)
+    await run(jamai.delete_table, TableType.action, table_id)
 
 
+@pytest.mark.parametrize("client_cls", CLIENT_CLS)
 @pytest.mark.parametrize("gen_type", GEN_TYPES)
 @pytest.mark.parametrize("input_dict, output_dict, column_map, row, expected_column_gen", data())
-def test_multirows_stream_concurrent_execution(
-    jamai_client: JamAI, gen_type, input_dict, output_dict, column_map, row, expected_column_gen
+async def test_multirows_stream_concurrent_execution(
+    client_cls: JamAI | JamAIAsync,
+    gen_type,
+    input_dict,
+    output_dict,
+    column_map,
+    row,
+    expected_column_gen,
 ):
     """
     Tests concurrent execution in streaming mode with dependencies.
     """
-    meta, table_id = _create_table(
-        jamai_client,
+    jamai = client_cls(project_id="", api_key="")
+    meta, table_id = await _create_table(
+        jamai,
         TableType.action,
         cols_info=(
             input_dict,
             output_dict,
         ),
     )
     gen_config = GenConfigUpdateRequest(table_id=table_id, column_map=column_map)
-    _update_gen_config(jamai_client, TableType.action, gen_config)
+    await _update_gen_config(jamai, TableType.action, gen_config)
 
     total_start_time = time.time()
-    response = jamai_client.add_table_rows(
-        TableType.action,
-        RowAddRequest(
-            table_id=table_id,
-            data=[row, row, row],
-            stream=True,
-            concurrent=True,
-        ),
-    )
-
-    # Collect streaming response
+    first_chunk_times = {}
     chunks = []
-    for chunk in response:
-        chunks.append(chunk)
-    logger.debug(f"> Stream Total Rows Time: {time.time() - total_start_time}")
+    if isinstance(jamai, JamAIAsync):
+        async for chunk in run_gen_async(
+            jamai.add_table_rows,
+            TableType.action,
+            RowAddRequest(
+                table_id=table_id,
+                data=[row, row, row],
+                stream=True,
+                concurrent=True,
+            ),
+        ):
+            chunks.append(chunk)
+            if chunk.row_id not in first_chunk_times.keys():
+                first_chunk_times[chunk.row_id] = {}
+            if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                    time.time() - total_start_time
+                )
 
-    if gen_type == "REGEN":
-        rows = jamai_client.list_table_rows(TableType.action, table_id)
-        logger.info(f"rows.items: {rows.items}")
-        total_start_time = time.time()
-        response = jamai_client.regen_table_rows(
+    else:
+        for chunk in run_gen_sync(
+            jamai.add_table_rows,
             TableType.action,
-            RowRegenRequest(
+            RowAddRequest(
                 table_id=table_id,
-                row_ids=[row_item["ID"] for row_item in rows.items],
+                data=[row],
                 stream=True,
                 concurrent=True,
             ),
-        )
-        # Collect streaming response
-        chunks = []
-        for chunk in response:
+        ):
             chunks.append(chunk)
-        logger.debug(f"> Stream Total Regen Rows Time: {time.time() - total_start_time}")
+            if chunk.row_id not in first_chunk_times.keys():
+                first_chunk_times[chunk.row_id] = {}
+            if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                    time.time() - total_start_time
+                )
+
+    for row_id_ in first_chunk_times.keys():
+        for output_column_name in first_chunk_times[row_id_].keys():
+            logger.debug(
+                f"> [Test] Time to first chunk for {output_column_name}: {first_chunk_times[row_id_].get(output_column_name, 'N/A'):.2f} seconds"
+            )
+        break
+
+    logger.debug(
+        f"> [Test] Stream Total Add Rows Time: {time.time() - total_start_time:.2f} seconds"
+    )
+
+    if gen_type == "REGEN":
+        rows = await run(jamai.list_table_rows, TableType.action, table_id)
+        total_start_time = time.time()
+        total_start_time = time.time()
+        first_chunk_times = {}
+        chunks = []
+        if isinstance(jamai, JamAIAsync):
+            async for chunk in run_gen_async(
+                jamai.regen_table_rows,
+                TableType.action,
+                RowRegenRequest(
+                    table_id=table_id,
+                    row_ids=[row_item["ID"] for row_item in rows.items],
+                    stream=True,
+                    concurrent=True,
+                ),
+            ):
+                chunks.append(chunk)
+                if chunk.row_id not in first_chunk_times.keys():
+                    first_chunk_times[chunk.row_id] = {}
+                if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                    first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                        time.time() - total_start_time
+                    )
+
+        else:
+            for chunk in run_gen_sync(
+                jamai.regen_table_rows,
+                TableType.action,
+                RowRegenRequest(
+                    table_id=table_id,
+                    row_ids=[row_item["ID"] for row_item in rows.items],
+                    stream=True,
+                    concurrent=True,
+                ),
+            ):
+                chunks.append(chunk)
+                if chunk.row_id not in first_chunk_times.keys():
+                    first_chunk_times[chunk.row_id] = {}
+                if chunk.output_column_name not in first_chunk_times[chunk.row_id].keys():
+                    first_chunk_times[chunk.row_id][chunk.output_column_name] = (
+                        time.time() - total_start_time
+                    )
+
+        for row_id_ in first_chunk_times.keys():
+            for output_column_name in first_chunk_times[row_id_].keys():
+                logger.debug(
+                    f"> [Test] Time to first chunk for {output_column_name}: {first_chunk_times[row_id_].get(output_column_name, 'N/A'):.2f} seconds"
+                )
+            break
+
+        logger.debug(
+            f"> [Test] Stream Total Regen Rows Time: {time.time() - total_start_time:.2f} seconds"
+        )
 
     # Get first rows
-    rows = jamai_client.list_table_rows(TableType.action, table_id)
+    rows = await run(jamai.list_table_rows, TableType.action, table_id)
     row_id = rows.items[0]["ID"]
-    row = jamai_client.get_table_row(TableType.action, table_id, row_id)
+    row = await run(jamai.get_table_row, TableType.action, table_id, row_id)
 
     # Compare generated outputs with expected outputs
     for output_column_name in output_dict.keys():
         expected_gen = expected_column_gen[output_column_name]
         column_gen = row[output_column_name]["value"]
         len_expected_gen = len(expected_gen)
         len_column_gen = len(column_gen)
         if len_column_gen >= len_expected_gen:
             assert column_gen[:len_expected_gen] == expected_gen
         else:
             assert column_gen == expected_gen[:len_column_gen]
 
-    jamai_client.delete_table(TableType.action, table_id)
+    await run(jamai.delete_table, TableType.action, table_id)
```

### Comparing `jamaibase-0.0.1/tests/test_gen_table.py` & `jamaibase-0.1.0/tests/test_gen_table.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/test_io.py` & `jamaibase-0.1.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `jamaibase-0.0.1/tests/xlsx/Claims Form.xlsx` & `jamaibase-0.1.0/tests/xlsx/Claims Form.xlsx`

 * *Files identical despite different names*

