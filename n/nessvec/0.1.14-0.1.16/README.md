# Comparing `tmp/nessvec-0.1.14.tar.gz` & `tmp/nessvec-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessvec-0.1.14.tar", max compression
+gzip compressed data, was "nessvec-0.1.16.tar", max compression
```

## Comparing `nessvec-0.1.14.tar` & `nessvec-0.1.16.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1099 2023-08-18 21:07:30.101060 nessvec-0.1.14/LICENSE.txt
--rw-r--r--   0        0        0     1115 2023-08-18 21:07:30.101060 nessvec-0.1.14/README.md
--rw-r--r--   0        0        0     2590 2024-01-01 01:31:07.637352 nessvec-0.1.14/pyproject.toml
--rw-r--r--   0        0        0      172 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/__init__.py
--rw-r--r--   0        0        0     7181 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/benchmarking.py
--rw-r--r--   0        0        0        0 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/clean_wiktionary_titles.py
--rw-r--r--   0        0        0    13304 2023-10-10 23:53:10.507141 nessvec-0.1.14/src/nessvec/constants.py
--rw-r--r--   0        0        0     1448 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/crawler-filterlinks.py
--rw-r--r--   0        0        0     2496 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/crawler.py
--rw-r--r--   0        0        0     8258 2023-10-10 23:50:03.799301 nessvec-0.1.14/src/nessvec/data/constants/LANG_INFO.csv
--rw-r--r--   0        0        0     1235 2023-10-10 23:50:03.799301 nessvec-0.1.14/src/nessvec/data/constants/LANG_ISO.csv
--rw-r--r--   0        0        0        0 2023-08-18 21:07:30.167314 nessvec-0.1.14/src/nessvec/data/constants/__init__.py
--rw-r--r--   0        0        0    61619 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/data/constants/tlds-from-iana.csv
--rwxr-xr-x   0        0        0    18419 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/data/constants/uri-schemes.xhtml.csv
--rw-r--r--   0        0        0      391 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/django_project/asgi.py
--rw-r--r--   0        0        0     3065 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/django_project/settings.py
--rw-r--r--   0        0        0      749 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/django_project/urls.py
--rw-r--r--   0        0        0      391 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/django_project/wsgi.py
--rw-r--r--   0        0        0      189 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/2022-01-15-SDML-mixed-precision-optimizers-relu-selu-elu-activation.md
--rw-r--r--   0        0        0     1831 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py
--rw-r--r--   0        0        0    15512 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py.md
--rw-r--r--   0        0        0    18197 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-ch06-extreme-summarization.hist.py
--rw-r--r--   0        0        0    75179 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/ch06/.ipynb_checkpoints/pytorch_word2vec_wikitext2-checkpoint.ipynb
--rw-r--r--   0        0        0     7994 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/ch06/ch06_nessvectors.py
--rw-r--r--   0        0        0     1219 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/ch06/ch06_nessvectors_with_spacy.py
--rw-r--r--   0        0        0     7994 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/ch06/nessvectors.py
--rwxr-xr-x   0        0        0      352 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/clean_ipy.sh
--rw-r--r--   0        0        0    20530 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/np_memmap_test_120GB.hist.ipy
--rw-r--r--   0        0        0      386 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.ipy
--rw-r--r--   0        0        0     1625 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.py
--rw-r--r--   0        0        0     1625 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey.py
--rw-r--r--   0        0        0     2213 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/examples/wikipedia_crawl.hist.py
--rw-r--r--   0        0        0    14415 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/fasttext.py
--rw-r--r--   0        0        0    36643 2023-10-11 00:30:32.117474 nessvec-0.1.14/src/nessvec/files.py
--rw-r--r--   0        0        0    10902 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/glove.py
--rw-r--r--   0        0        0    63413 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/hist/datatable_word_vector_similarity.hist.ipy
--rw-r--r--   0        0        0     2200 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/hist/glove_dataframe_to_hdf5.hist.py
--rw-r--r--   0        0        0    13718 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/hist/pynn_index_king_queen.hist.ipy
--rw-r--r--   0        0        0     3381 2023-08-18 21:07:30.171211 nessvec-0.1.14/src/nessvec/hypervec.py
--rw-r--r--   0        0        0    16243 2023-10-11 16:11:36.830064 nessvec-0.1.14/src/nessvec/indexers.py
--rw-r--r--   0        0        0     8009 2023-08-21 01:53:42.099126 nessvec-0.1.14/src/nessvec/nessvectors.py
--rw-r--r--   0        0        0    35440 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/re_patterns.py
--rw-r--r--   0        0        0     2096 2023-08-21 19:41:33.186791 nessvec-0.1.14/src/nessvec/scripts/test_memory_usage.py
--rw-r--r--   0        0        0      187 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/spacy_language_model.py
--rw-r--r--   0        0        0     4528 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/spell.py
--rw-r--r--   0        0        0     2701 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/text.py
--rw-r--r--   0        0        0     5536 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/translation.py
--rw-r--r--   0        0        0     6885 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/util.py
--rw-r--r--   0        0        0     7167 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wikicrawl.py
--rw-r--r--   0        0        0    11618 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch02_sentiment.py
--rw-r--r--   0        0        0     5318 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06.py
--rw-r--r--   0        0        0     1997 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_glove_dask_dataframe.py
--rw-r--r--   0        0        0     3887 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_glove_nessvectors.py
--rw-r--r--   0        0        0     7975 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_nessvectors.py
--rw-r--r--   0        0        0     8980 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_sentence_embeddings.py
--rw-r--r--   0        0        0     6170 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_w2v_10_us_cities_visualization_.py
--rw-r--r--   0        0        0     6889 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_w2v_us_cities_visualization.py
--rw-r--r--   0        0        0     6998 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_w2v_us_cities_visualization_spacy.py
--rw-r--r--   0        0        0     1792 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch06_word2vec_embedding_viz.py
--rw-r--r--   0        0        0     2032 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch09_imdb_sentiment_lstm_v1.py
--rw-r--r--   0        0        0     1522 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/ch09_imdb_sentiment_lstm_v2.py
--rw-r--r--   0        0        0     2805 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/wip/yaml_graphviz.py
--rw-r--r--   0        0        0     4050 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/word2vec.py
--rw-r--r--   0        0        0     2565 2023-08-18 21:07:30.175108 nessvec-0.1.14/src/nessvec/worder.py
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 nessvec-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1099 2024-06-02 01:49:38.257032 nessvec-0.1.16/LICENSE.txt
+-rw-r--r--   0        0        0     1115 2024-06-02 01:49:38.257032 nessvec-0.1.16/README.md
+-rw-r--r--   0        0        0     2590 2024-06-02 03:17:32.127046 nessvec-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0      172 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/__init__.py
+-rw-r--r--   0        0        0     7181 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/benchmarking.py
+-rw-r--r--   0        0        0        0 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/clean_wiktionary_titles.py
+-rw-r--r--   0        0        0    13421 2024-06-02 03:16:25.632547 nessvec-0.1.16/src/nessvec/constants.py
+-rw-r--r--   0        0        0     1448 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/crawler-filterlinks.py
+-rw-r--r--   0        0        0     2496 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/crawler.py
+-rw-r--r--   0        0        0     8258 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/data/constants/LANG_INFO.csv
+-rw-r--r--   0        0        0     1235 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/data/constants/LANG_ISO.csv
+-rw-r--r--   0        0        0        0 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/data/constants/__init__.py
+-rw-r--r--   0        0        0    61619 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/data/constants/tlds-from-iana.csv
+-rwxr-xr-x   0        0        0    18419 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/data/constants/uri-schemes.xhtml.csv
+-rw-r--r--   0        0        0      391 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/django_project/asgi.py
+-rw-r--r--   0        0        0     3065 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/django_project/settings.py
+-rw-r--r--   0        0        0      749 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/django_project/urls.py
+-rw-r--r--   0        0        0      391 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/django_project/wsgi.py
+-rw-r--r--   0        0        0      189 2024-06-02 01:49:38.373035 nessvec-0.1.16/src/nessvec/examples/2022-01-15-SDML-mixed-precision-optimizers-relu-selu-elu-activation.md
+-rw-r--r--   0        0        0     1831 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py
+-rw-r--r--   0        0        0    15512 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py.md
+-rw-r--r--   0        0        0    18197 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-ch06-extreme-summarization.hist.py
+-rw-r--r--   0        0        0    75179 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/ch06/.ipynb_checkpoints/pytorch_word2vec_wikitext2-checkpoint.ipynb
+-rw-r--r--   0        0        0     7994 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/ch06/ch06_nessvectors.py
+-rw-r--r--   0        0        0     1219 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/ch06/ch06_nessvectors_with_spacy.py
+-rw-r--r--   0        0        0     7994 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/ch06/nessvectors.py
+-rwxr-xr-x   0        0        0      352 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/clean_ipy.sh
+-rw-r--r--   0        0        0    20530 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/np_memmap_test_120GB.hist.ipy
+-rw-r--r--   0        0        0      386 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.ipy
+-rw-r--r--   0        0        0     1625 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.py
+-rw-r--r--   0        0        0     1625 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey.py
+-rw-r--r--   0        0        0     2213 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/examples/wikipedia_crawl.hist.py
+-rw-r--r--   0        0        0    14415 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/fasttext.py
+-rw-r--r--   0        0        0    36643 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/files.py
+-rw-r--r--   0        0        0    10902 2024-06-02 01:49:38.377035 nessvec-0.1.16/src/nessvec/glove.py
+-rw-r--r--   0        0        0    63413 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/hist/datatable_word_vector_similarity.hist.ipy
+-rw-r--r--   0        0        0     2200 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/hist/glove_dataframe_to_hdf5.hist.py
+-rw-r--r--   0        0        0    13718 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/hist/pynn_index_king_queen.hist.ipy
+-rw-r--r--   0        0        0     3381 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/hypervec.py
+-rw-r--r--   0        0        0    16243 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/indexers.py
+-rw-r--r--   0        0        0     8009 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/nessvectors.py
+-rw-r--r--   0        0        0    35440 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/re_patterns.py
+-rw-r--r--   0        0        0     2096 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/scripts/test_memory_usage.py
+-rw-r--r--   0        0        0      187 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/spacy_language_model.py
+-rw-r--r--   0        0        0     4528 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/spell.py
+-rw-r--r--   0        0        0     2701 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/text.py
+-rw-r--r--   0        0        0     5536 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/translation.py
+-rw-r--r--   0        0        0     6885 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/util.py
+-rw-r--r--   0        0        0     7167 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wikicrawl.py
+-rw-r--r--   0        0        0    11618 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch02_sentiment.py
+-rw-r--r--   0        0        0     5318 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06.py
+-rw-r--r--   0        0        0     1997 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_glove_dask_dataframe.py
+-rw-r--r--   0        0        0     3887 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_glove_nessvectors.py
+-rw-r--r--   0        0        0     7975 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_nessvectors.py
+-rw-r--r--   0        0        0     8980 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_sentence_embeddings.py
+-rw-r--r--   0        0        0     6170 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_w2v_10_us_cities_visualization_.py
+-rw-r--r--   0        0        0     6889 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_w2v_us_cities_visualization.py
+-rw-r--r--   0        0        0     6998 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_w2v_us_cities_visualization_spacy.py
+-rw-r--r--   0        0        0     1792 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch06_word2vec_embedding_viz.py
+-rw-r--r--   0        0        0     2032 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch09_imdb_sentiment_lstm_v1.py
+-rw-r--r--   0        0        0     1522 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/ch09_imdb_sentiment_lstm_v2.py
+-rw-r--r--   0        0        0     2805 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/wip/yaml_graphviz.py
+-rw-r--r--   0        0        0     4050 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/word2vec.py
+-rw-r--r--   0        0        0     2565 2024-06-02 01:49:38.381035 nessvec-0.1.16/src/nessvec/worder.py
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 nessvec-0.1.16/PKG-INFO
```

### Comparing `nessvec-0.1.14/LICENSE.txt` & `nessvec-0.1.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/README.md` & `nessvec-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/pyproject.toml` & `nessvec-0.1.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 # https://python-poetry.org/docs/pyproject/
 # https://github.com/python-poetry/poetry/blob/master/pyproject.toml
 name = "nessvec"
-version = "0.1.14"
+version = "0.1.16"
 description = "Word embeddings with meaningful dimensions for better explainability."
 license = "GPLv3"
 readme = "README.md"
 authors = [
     "Hobson Lane <hobson@tangibleai.com>",
     "Hobson Lane <hobson@tangibleai.com>",
     "Maria Dyshel <maria@tangibleai.com>",
```

### Comparing `nessvec-0.1.14/src/nessvec/benchmarking.py` & `nessvec-0.1.16/src/nessvec/benchmarking.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/constants.py` & `nessvec-0.1.16/src/nessvec/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,34 +13,29 @@
 import numpy as np
 import pandas as pd
 
 log = logging.getLogger(__name__)
 
 PKG_DIR = Path(__file__).absolute().resolve().parent
 PKG_NAME = PKG_DIR.name
-SRC_DIR = PKG_DIR.parent
-REPO_DIR = SRC_DIR.parent
+REPO_DIR = SRC_DIR = PKG_DIR
+
+# When `pip installed --editable` (source code from git clone) SRC and REPO dir are PKG.parent and PKG.parent.parent
+if PKG_DIR.parent.name == 'src' or PKG_DIR.parent.parent.name == PKG_NAME:
+    SRC_DIR = PKG_DIR.parent
+    REPO_DIR = SRC_DIR.parent
+assert REPO_DIR.name == PKG_NAME
+assert SRC_DIR.name in (PKG_NAME, 'src')
 
 DATA_DIR_NAME = '.nlpia2-data'
 HOME_DIR = Path.home()
 DATA_DIR = HOME_DIR / DATA_DIR_NAME
 
 TOML_VERSION_PATTERN = re.compile(r'(version\s*=\s*)[\'"]?(\d(\.\d+)+)[\'"]?\s*')
 
-# SRC_DIR will be the lib/pythonX.X/site-packages directory if nessvec installed with pip from PyPi
-SRC_DIR = PKG_DIR.parent
-
-# REPO_DIR will be either ...
-#    1. the parent of site-packages (if pip installed into ananconda3 env):
-#       `~/anaconda3/envs/nessvec/lib/python3.8/`
-#    OR
-#    2. the git local clone of the git repository (if cloned into ~):
-#       `~/nessvec/`
-REPO_DIR = SRC_DIR.parent
-
 
 ############################################################################
 # setup DATA_DIR
 # TODO: setup.py should handle all this
 
 DATA_CONSTANTS_BASEURL = 'https://gitlab.com/tangibleai/nessvec/-/raw/main/src/nessvec/data/constants'
 DATA_CONSTANTS_FILENAMES = [
@@ -322,18 +317,23 @@
 
 # from pugnlp.constants
 #########################################################
 
 
 def get_version(repo_dir=REPO_DIR, pattern=TOML_VERSION_PATTERN):
     """ Read the pyproject.toml file to extract the package version number """
-    with (repo_dir / 'pyproject.toml').open() as fin:
-        for line in fin:
-            match = pattern.match(line)
-            if match:
-                log.debug(f'Found match.groups(): {dict(list(enumerate(match.groups())))}')
-                return match.groups()[1]
-                # version_ints = [int(x) for x in version.split('.')]
-    return '0.0.0'
+    __version__ = '0.1.16'
+    try:
+        with (repo_dir / 'pyproject.toml').open() as fin:
+            for line in fin:
+                match = pattern.match(line)
+                if match:
+                    log.debug(f'Found match.groups(): {dict(list(enumerate(match.groups())))}')
+                    return match.groups()[1]
+                    # version_ints = [int(x) for x in version.split('.')]
+    except Exception as e:
+        log.warning(str(e))
+        log.warning(f"Unable to find 'pyproject.toml' so assuming default version {__version__}")
+    return __version__
 
 
 __version__ = get_version()
```

### Comparing `nessvec-0.1.14/src/nessvec/crawler-filterlinks.py` & `nessvec-0.1.16/src/nessvec/crawler-filterlinks.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/crawler.py` & `nessvec-0.1.16/src/nessvec/crawler.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/data/constants/LANG_INFO.csv` & `nessvec-0.1.16/src/nessvec/data/constants/LANG_INFO.csv`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/data/constants/LANG_ISO.csv` & `nessvec-0.1.16/src/nessvec/data/constants/LANG_ISO.csv`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/data/constants/tlds-from-iana.csv` & `nessvec-0.1.16/src/nessvec/data/constants/tlds-from-iana.csv`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/data/constants/uri-schemes.xhtml.csv` & `nessvec-0.1.16/src/nessvec/data/constants/uri-schemes.xhtml.csv`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/django_project/settings.py` & `nessvec-0.1.16/src/nessvec/django_project/settings.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/django_project/urls.py` & `nessvec-0.1.16/src/nessvec/django_project/urls.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py` & `nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py.md` & `nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-after-party-ch06-extreme-summarization-closest-stopword.hist.py.md`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/2022-03-30-mob-programming-ch06-extreme-summarization.hist.py` & `nessvec-0.1.16/src/nessvec/examples/2022-03-30-mob-programming-ch06-extreme-summarization.hist.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/ch06/.ipynb_checkpoints/pytorch_word2vec_wikitext2-checkpoint.ipynb` & `nessvec-0.1.16/src/nessvec/examples/ch06/.ipynb_checkpoints/pytorch_word2vec_wikitext2-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/ch06/ch06_nessvectors.py` & `nessvec-0.1.16/src/nessvec/examples/ch06/ch06_nessvectors.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/ch06/ch06_nessvectors_with_spacy.py` & `nessvec-0.1.16/src/nessvec/examples/ch06/ch06_nessvectors_with_spacy.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/ch06/nessvectors.py` & `nessvec-0.1.16/src/nessvec/examples/ch06/nessvectors.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/np_memmap_test_120GB.hist.ipy` & `nessvec-0.1.16/src/nessvec/examples/np_memmap_test_120GB.hist.ipy`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.py` & `nessvec-0.1.16/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey-edited.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey.py` & `nessvec-0.1.16/src/nessvec/examples/tbd/etl_pocket_bookmarks_brian_piercey.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/examples/wikipedia_crawl.hist.py` & `nessvec-0.1.16/src/nessvec/examples/wikipedia_crawl.hist.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/fasttext.py` & `nessvec-0.1.16/src/nessvec/fasttext.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/files.py` & `nessvec-0.1.16/src/nessvec/files.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/glove.py` & `nessvec-0.1.16/src/nessvec/glove.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/hist/datatable_word_vector_similarity.hist.ipy` & `nessvec-0.1.16/src/nessvec/hist/datatable_word_vector_similarity.hist.ipy`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/hist/glove_dataframe_to_hdf5.hist.py` & `nessvec-0.1.16/src/nessvec/hist/glove_dataframe_to_hdf5.hist.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/hist/pynn_index_king_queen.hist.ipy` & `nessvec-0.1.16/src/nessvec/hist/pynn_index_king_queen.hist.ipy`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/hypervec.py` & `nessvec-0.1.16/src/nessvec/hypervec.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/indexers.py` & `nessvec-0.1.16/src/nessvec/indexers.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/nessvectors.py` & `nessvec-0.1.16/src/nessvec/nessvectors.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/re_patterns.py` & `nessvec-0.1.16/src/nessvec/re_patterns.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/scripts/test_memory_usage.py` & `nessvec-0.1.16/src/nessvec/scripts/test_memory_usage.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/spell.py` & `nessvec-0.1.16/src/nessvec/spell.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/text.py` & `nessvec-0.1.16/src/nessvec/text.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/translation.py` & `nessvec-0.1.16/src/nessvec/translation.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/util.py` & `nessvec-0.1.16/src/nessvec/util.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wikicrawl.py` & `nessvec-0.1.16/src/nessvec/wikicrawl.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch02_sentiment.py` & `nessvec-0.1.16/src/nessvec/wip/ch02_sentiment.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06.py` & `nessvec-0.1.16/src/nessvec/wip/ch06.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_glove_dask_dataframe.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_glove_dask_dataframe.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_glove_nessvectors.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_glove_nessvectors.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_nessvectors.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_nessvectors.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_sentence_embeddings.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_sentence_embeddings.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_w2v_10_us_cities_visualization_.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_w2v_10_us_cities_visualization_.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_w2v_us_cities_visualization.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_w2v_us_cities_visualization.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_w2v_us_cities_visualization_spacy.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_w2v_us_cities_visualization_spacy.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch06_word2vec_embedding_viz.py` & `nessvec-0.1.16/src/nessvec/wip/ch06_word2vec_embedding_viz.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch09_imdb_sentiment_lstm_v1.py` & `nessvec-0.1.16/src/nessvec/wip/ch09_imdb_sentiment_lstm_v1.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/ch09_imdb_sentiment_lstm_v2.py` & `nessvec-0.1.16/src/nessvec/wip/ch09_imdb_sentiment_lstm_v2.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/wip/yaml_graphviz.py` & `nessvec-0.1.16/src/nessvec/wip/yaml_graphviz.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/word2vec.py` & `nessvec-0.1.16/src/nessvec/word2vec.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/src/nessvec/worder.py` & `nessvec-0.1.16/src/nessvec/worder.py`

 * *Files identical despite different names*

### Comparing `nessvec-0.1.14/PKG-INFO` & `nessvec-0.1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessvec
-Version: 0.1.14
+Version: 0.1.16
 Summary: Word embeddings with meaningful dimensions for better explainability.
 Home-page: https://gitlab.com/tangibleai/nessvec
 License: GPLv3
 Keywords: NLP,Natural Language Processing,Virtual Assistant,chatbot,Text Processing,Machine Learning,Text Mining,Deep Learning
 Author: Hobson Lane
 Author-email: hobson@tangibleai.com
 Requires-Python: >=3.9
```

