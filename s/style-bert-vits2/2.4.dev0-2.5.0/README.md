# Comparing `tmp/style_bert_vits2-2.4.dev0.tar.gz` & `tmp/style_bert_vits2-2.5.0.tar.gz`

## Comparing `style_bert_vits2-2.4.dev0.tar` & `style_bert_vits2-2.5.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/.vscode/extensions.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/.vscode/settings.json
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/LGPL_LICENSE
--rw-r--r--   0        0        0    17894 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/docs/CLI.md
--rw-r--r--   0        0        0     7094 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/docs/README_en.md
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/docs/paperspace.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/.editorconfig
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/__init__.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/constants.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/logging.py
--rw-r--r--   0        0        0    18728 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/tts_model.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/voice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/__init__.py
--rw-r--r--   0        0        0    17755 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/attentions.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/commons.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/hyper_parameters.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/infer.py
--rw-r--r--   0        0        0    36778 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/models.py
--rw-r--r--   0        0        0    38227 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/models_jp_extra.py
--rw-r--r--   0        0        0    20636 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/modules.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/monotonic_alignment.py
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/transforms.py
--rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/__init__.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/checkpoints.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/safetensors.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/__init__.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/bert_models.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/symbols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/__init__.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/bert_feature.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/g2p.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/normalizer.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/opencpop-strict.txt
--rw-r--r--   0        0        0    23500 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/tone_sandhi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/__init__.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/bert_feature.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict.py
--rw-r--r--   0        0        0  3969309 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict.rep
--rw-r--r--   0        0        0  6212655 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict_cache.pickle
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/g2p.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/normalizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/__init__.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/bert_feature.py
--rw-r--r--   0        0        0    22167 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/g2p.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/g2p_utils.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/mora_list.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/normalizer.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__main__.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_client.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_common.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_server.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/README.md
--rw-r--r--   0        0        0    16565 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/__init__.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/part_of_speech_data.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/word_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/utils/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/utils/stdout_wrapper.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/utils/strenum.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/style_bert_vits2/utils/subprocess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/tests/__init__.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/tests/test_main.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/dict_data/default.csv
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/LICENSE
--rw-r--r--   0        0        0    17311 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/README.md
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/pyproject.toml
--rw-r--r--   0        0        0    18656 2020-02-02 00:00:00.000000 style_bert_vits2-2.4.dev0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/.vscode/extensions.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/LGPL_LICENSE
+-rw-r--r--   0        0        0    29759 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/CLI.md
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/FAQ.md
+-rw-r--r--   0        0        0    15708 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/Style-Bert-VITS2_en.md
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/TERMS_OF_USE.md
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/docs/paperspace.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/.editorconfig
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/constants.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/logging.py
+-rw-r--r--   0        0        0    22185 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/tts_model.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/voice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/__init__.py
+-rw-r--r--   0        0        0    17755 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/attentions.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/commons.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/hyper_parameters.py
+-rw-r--r--   0        0        0    12250 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/infer.py
+-rw-r--r--   0        0        0    36765 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/models.py
+-rw-r--r--   0        0        0    38214 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/models_jp_extra.py
+-rw-r--r--   0        0        0    20636 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/modules.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/monotonic_alignment.py
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/transforms.py
+-rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/utils/__init__.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/utils/checkpoints.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/models/utils/safetensors.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/__init__.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/bert_models.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/symbols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/__init__.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/bert_feature.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/g2p.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/normalizer.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/opencpop-strict.txt
+-rw-r--r--   0        0        0    23123 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/tone_sandhi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/__init__.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/bert_feature.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict.py
+-rw-r--r--   0        0        0  3969309 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict.rep
+-rw-r--r--   0        0        0  6212655 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict_cache.pickle
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/g2p.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/normalizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/__init__.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/bert_feature.py
+-rw-r--r--   0        0        0    34797 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/g2p.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/g2p_utils.py
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/mora_list.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/normalizer.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__main__.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_client.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_common.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_server.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/README.md
+-rw-r--r--   0        0        0    16565 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/__init__.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/part_of_speech_data.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/word_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/utils/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/utils/stdout_wrapper.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/utils/strenum.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/style_bert_vits2/utils/subprocess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/tests/test_main.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/dict_data/default.csv
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/LICENSE
+-rw-r--r--   0        0        0    17353 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/README.md
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18580 2020-02-02 00:00:00.000000 style_bert_vits2-2.5.0/PKG-INFO
```

### Comparing `style_bert_vits2-2.4.dev0/.vscode/settings.json` & `style_bert_vits2-2.5.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/LGPL_LICENSE` & `style_bert_vits2-2.5.0/LGPL_LICENSE`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/docs/CHANGELOG.md` & `style_bert_vits2-2.5.0/docs/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,133 @@
 # Changelog
 
+## v2.5.0 (2024-06-02)
+
+このバージョンから[利用規約](/docs/TERMS_OF_USE.md)が追加されました。ご利用の際は必ずお読みください。
+
+### 新機能等
+
+- デフォルトモデルに [あみたろの声素材工房](https://amitaro.net/) のあみたろ様が公開しているコーパスとライブ配信音声を利用して学習した**小春音アミ**と**あみたろ**モデルを追加（あみたろ様には事前に連絡して許諾を得ています）
+    - アプデの場合は新たに`App.bat`や`Editor.bat`を起動した際に自動でダウンロードされます
+- 学習時に音声データをスタイルごとにフォルダ分けしておくことで、そのフォルダごとのスタイルを学習時に自動的に作成するように
+    - `inputs`からスライスして使う場合は`inputs`直下に作りたいスタイルだけサブフォルダを作りそこに音声ファイルを配置
+    - `Data/モデル名/raw`から使う場合も`raw`直下に同様に配置
+    - サブフォルダの個数が0または1の場合は、今まで通りのNeutralスタイルのみが作成されます
+- batファイルでのインストールの大幅な高速化（Pythonのライブラリインストールに[uv](https://github.com/astral-sh/uv)を使用）
+- 学習時に「カスタムバッチサンプラーを無効化」オプションを追加。これにより、長い音声ファイルも学習に使われるようになりますが、使用VRAMがかなり増えたり学習が不安定になる可能性があります。
+- [よくある質問](/docs/FAQ.md)を追加
+- 英語の音声合成の速度向上（[gordon0414](https://github.com/gordon0414)さんによる[PR](https://github.com/litagin02/Style-Bert-VITS2/pull/124)です、ありがとうございます！）
+- エディターの各種機能改善（多くが[kamexy](https://github.com/kamexy)様による[エディターリポジトリ](https://github.com/litagin02/Style-Bert-VITS2-Editor)へのプルリク群です、ありがとうございます！）
+    - 選択した行の下に新規の行を作成できるように
+    - Mac使用時に日本語変換のエンターで音声合成が走るバグの修正
+    - ペースト時に改行を含まない場合は通常のペーストの振る舞いになるように修正
+
+
+### その他の改善
+
+- 上のスタイル自動作成機能を既存モデルでも使えるような機能追加。具体的には、スタイル作成タブにて、フォルダ分けされた音声ファイルのディレクトリを任意に指定し、そのフォルダ分けを使って既存のモデルのスタイルの作成が可能に
+- 音声書き起こしに[kotoba-whisper](https://huggingface.co/kotoba-tech/kotoba-whisper-v1.1)を追加
+- 音声書き起こし時にHugging FaceのWhisperモデルを使う際に、書き起こしを順次保存するように改善
+- （**ライブラリとしてのみ**）依存関係の軽量化、音声合成時に読み上げテキストの読みを表す音素列を指定する機能を追加 + 様々な改善 ([tsukumijimaさん](https://github.com/tsukumijima)による[プルリク](https://github.com/litagin02/Style-Bert-VITS2/pull/118)です、ありがとうございます！)
+
+### 内部変更
+
+- これまでpath管理に`configs/paths.yml`を使っていたが、`configs/default_paths.yml`にリネームし、`configs/paths.yml`はgitの管理対象外に変更
+
+### バグ修正
+
+- Gradioのアップデートにより、モデル選択時やスタイルのDBSCAN作成時等に`TypeError: Type is not JSON serializable: WindowsPath`のようなエラーが出る問題を修正
+- TensorboardをWebUIから立ち上げた際にエラーが出る問題の修正 ([#129](https://github.com/litagin02/Style-Bert-VITS2/issues/129))
+
+
+## v2.4.1 (2024-03-16)
+
+**batファイルでのインストール・アップデート方法の変更**（それ以外の変更はありません）
+
+諸事情により、インストール・アップデートのbatファイルを変更しました（Gitが使えないのでバージョンアップ時のアップデートの対応が困難だったため、Gitがない環境の場合はPortableGitをダウンロードして使うように）。
+
+伴って、これまでWindowsでbatファイルをダブルクリックしてインストールしていた方は**再インストールが必須**となります。大変申し訳ありません。
+
+### インストール手順
+
+（インストールの流れは変わりませんが、batファイルは変わっているので、新しいzipを必ずダウンロードしてください）
+
+- [sbv2.zip](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.4.1/sbv2.zip)をダウンロードし、解凍してください。
+- グラボがある方は、`Install-Style-Bert-VITS2.bat`をダブルクリックします。
+- グラボがない方は、`Install-Style-Bert-VITS2-CPU.bat`をダブルクリックします。CPU版では学習はできませんが、音声合成とマージは可能です。
+
+### アップデート手順
+
+**以前のバージョンからのアップデート**
+
+今までの環境を全て削除して新しくインストールする必要があります。
+移行方法：
+- 重要なデータが入っている可能性のある`Data`フォルダと`model_assets`フォルダをバックアップ
+- 上のインストール手順から、新しい場所にStyle-Bert-VITS2をインストール
+- インストールが終了したら、バックアップした`Data`フォルダと`model_assets`フォルダを新しい`Style-Bert-VITS2`フォルダにコピー
+- これまでインストールされていたフォルダ（batファイルたち含む）は削除しても構いません
+
+**今後のアップデート**
+
+今後は、新しくインストールされた中の`Update-Style-Bert-VITS2.bat`をダブルクリックしてください。今までの`Update-Style-Bert-VITS2.bat`等のファイルは使えません。
+
+## v2.4.0 (2024-03-15)
+
+大規模リファクタリング・日本語処理のワーカー化と機能追加等。データセット作り・学習・音声合成・マージ・スタイルWebUIは全て`app.py` (`App.bat`) へ統一されましたのでご注意ください。
+
+### アップデート手順
+- 2.3未満（辞書・エディター追加前）からのアップデートの場合は、[Update-to-Dict-Editor.bat](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.4.0/Update-to-Dict-Editor.bat)をダウンロードし、`Style-Bert-VITS2`フォルダがある場所（インストールbatファイルとかがあったところ）においてダブルクリックしてください。
+- それ以外の場合は、単純に今までの`Update-Style-Bert-VITS2.bat`でアップデートできます。
+- ただしアップデートにより多くのファイルが移動したり不要になったりしたので、それらを削除したい場合は[Clean.bat](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.4.0/Clean.bat)を`Update-Style-Bert-VITS2.bat`と同じ場所に保存して実行してください。
+
+### 内部改善
+
+- [tsukumijimaさんによる大規模リファクタリングのプルリク](https://github.com/litagin02/Style-Bert-VITS2/pull/92) によって、内部コードが非常に整理され可読性が高まりライブラリ化もされた。[tsukumijimaさん](https://github.com/tsukumijima) 大変な作業を本当にありがとうございます！
+- ライブラリとして`pip install style-bert-vits2`によりすぐにインストールでき、音声合成部分の機能が使えます（使用例は[/library.ipynb](/library.ipynb)を参照してください）
+- その他このプルリクに動機づけられ、多くのコードのリファクタリング・型アノテーションの追加等を行った
+- 日本語処理のpyopenjtalkをソケット通信を用いて別プロセス化し、複数同時に学習や音声合成を立ち上げても辞書の競合エラーが起きないように。[kale4eat](https://github.com/kale4eat) さんによる[PR](https://github.com/litagin02/Style-Bert-VITS2/pull/89) です、ありがとうございます！
+
+### バグ修正
+
+- 上記にもある通り、音声合成と学習前処理など、日本語処理を扱うものを2つ以上起動しようとするとエラーが発生する仕様の解決。ユーザー辞書は追加すれば常にどこからでも適応されます。
+- `raw`フォルダの直下でなくサブフォルダ内に音声ファイルがある場合に、`wavs`フォルダでもその構造が保たれてしまい、書き起こしファイルとの整合性が取れなくなる挙動を修正し、常に`wav`フォルダ直下へ`wav`ファイルを保存するように変更
+- スライス時に元ファイル名にピリオド `.` が含まれると、スライス後のファイル名がおかしくなるバグの修正
+
+### 機能改善・追加
+
+- 各種WebUIを一つ`app.py` `App.bat` に統一
+- その他以下の変更や、軽微なUI・説明文の改善等
+
+**データセット作成**
+
+- スライス処理の高速化（マルチスレッドにした、大量にスライス元ファイルファイルがある場合に高速になります）、またスライス元のファイルを`wav`以外の`mp3`や`ogg`などの形式にも対応
+- スライス処理時に、ファイル名にスライスされた開始終了区間を含めるオプションを追加（[aka7774](https://github.com/aka7774) さんによるPRです、ありがとうございます！）
+- 書き起こしの高速化、またHugging FaceのWhisperモデルを使うオプションを追加。バッチサイズを上げることでVRAMを食う代わりに速度が大幅に向上します。
+
+**学習**
+
+- 学習元の音声ファイル（`Data/モデル名/raw`にいれるやつ）を、`wav`以外の`mp3`や`ogg`などの形式にも対応（前処理段階で自動的に`wav`ファイルに変換されます）（ただし変わらず1ファイル2-12秒程度の範囲の長さが望ましい）
+
+**音声合成**
+
+- 音声合成時に、生成音声の音の高さ（音高）と抑揚の幅を調整できるように（ただし音質が少し劣化する）。`App.bat`や`Editor.bat`のどちらからでも使えます。
+- `Editor.bat`の複数話者モデルでの話者指定を可能に
+- `Editor.bat`で、改行を含む文字列をペーストすると自動的に欄が増えるように。また「↑↓」キーで欄を追加・行き来できるように（エディター側で以前に既にアプデしていました）
+- `Editor.bat`でモデル一覧のリロードをメニューに追加
+
+**API**
+
+- `server_fastapi.py`の実行時に全てのモデルファイルを読み込もうとする挙動を修正。音声合成がリクエストされて初めてそのモデルを読み込むように変更（APIを使わない音声合成のときと同じ挙動）
+- `server_fastapi.py`の音声合成エンドポイント`/voice`について、GETメソッドに加えてPOSTメソッドを追加。GETメソッドでは多くの制約があるようなのでPOSTを使うことが推奨されます。
+
+**CLI**
+
+- `preprocess_text.py`で、書き起こしファイルでの音声ファイル名を自動的に正しい`Data/モデル名/wavs/`へ書き換える`--correct_path`オプションの追加（WebUIでは今までもこの挙動でした）
+- その他上述のデータセット作成の機能追加に伴うCLIのオプションの追加（詳しくは[CLI.md](/docs/CLI.md)を参照）
+
 ## v2.3.1 (2024-02-27)
 
 ### バグ修正
 - colabの学習用ノートブックが動かなかったのを修正
 - `App.bat`や`server_fastapi.py`では読めない文字でまだエラーが発生するようになっていたので、推論時は必ず読めない文字を無視して強引に読むように挙動を変更
 
 ### 改善
```

### Comparing `style_bert_vits2-2.4.dev0/docs/CLI.md` & `style_bert_vits2-2.5.0/docs/CLI.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,58 +3,65 @@
 ## 0. Install and global paths settings
 
 ```bash
 git clone https://github.com/litagin02/Style-Bert-VITS2.git
 cd Style-Bert-VITS2
 python -m venv venv
 venv\Scripts\activate
-pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118
+pip install torch torchaudio --index-url https://download.pytorch.org/whl/cu118
 pip install -r requirements.txt
 ```
 
 Then download the necessary models and the default TTS model, and set the global paths.
 ```bash
-python initialize.py [--skip_jvnv] [--dataset_root <path>] [--assets_root <path>]
+python initialize.py [--skip_default_models] [--dataset_root <path>] [--assets_root <path>]
 ```
 
 Optional:
-- `--skip_jvnv`: Skip downloading the default JVNV voice models (use this if you only have to train your own models).
+- `--skip_default_models`: Skip downloading the default voice models (use this if you only have to train your own models).
 - `--dataset_root`: Default: `Data`. Root directory of the training dataset. The training dataset of `{model_name}` should be placed in `{dataset_root}/{model_name}`.
 - `--assets_root`: Default: `model_assets`. Root directory of the model assets (for inference). In training, the model assets will be saved to `{assets_root}/{model_name}`, and in inference, we load all the models from `{assets_root}`.
 
 
 ## 1. Dataset preparation
 
-### 1.1. Slice wavs
+### 1.1. Slice audio files
+
+The following audio formats are supported: ".wav", ".flac", ".mp3", ".ogg", ".opus", ".m4a".
 ```bash
-python slice.py --model_name <model_name> [-i <input_dir>] [-m <min_sec>] [-M <max_sec>]
+python slice.py --model_name <model_name> [-i <input_dir>] [-m <min_sec>] [-M <max_sec>] [--time_suffix]
 ```
 
 Required:
 - `model_name`: Name of the speaker (to be used as the name of the trained model).
 
 Optional:
 - `input_dir`: Path to the directory containing the audio files to slice (default: `inputs`)
 - `min_sec`: Minimum duration of the sliced audio files in seconds (default: 2).
 - `max_sec`: Maximum duration of the sliced audio files in seconds (default: 12).
+- `--time_suffix`: Make the filename end with -start_ms-end_ms when saving wav.
 
-### 1.2. Transcribe wavs
+### 1.2. Transcribe audio files
 
 ```bash
 python transcribe.py --model_name <model_name>
 ```
 Required:
 - `model_name`: Name of the speaker (to be used as the name of the trained model).
 
 Optional
 - `--initial_prompt`: Initial prompt to use for the transcription (default value is specific to Japanese).
 - `--device`: `cuda` or `cpu` (default: `cuda`).
 - `--language`: `jp`, `en`, or `en` (default: `jp`).
 - `--model`: Whisper model, default: `large-v3`
-- `--compute_type`: default: `bfloat16`
+- `--compute_type`: default: `bfloat16`. Only used if not `--use_hf_whisper`.
+- `--use_hf_whisper`: Use Hugging Face's whisper model instead of default faster-whisper (HF whisper is faster but requires more VRAM).
+- `--batch_size`: Batch size (default: 16). Only used if `--use_hf_whisper`.
+- `--num_beams`: Beam size (default: 1).
+- `--no_repeat_ngram_size`: N-gram size for no repeat (default: 10).
 
 ## 2. Preprocess
 
 ```bash
 python preprocess_all.py -m <model_name> [--use_jp_extra] [-b <batch_size>] [-e <epochs>] [-s <save_every_steps>] [--num_processes <num_processes>] [--normalize] [--trim] [--val_per_lang <val_per_lang>] [--log_interval <log_interval>] [--freeze_EN_bert] [--freeze_JP_bert] [--freeze_ZH_bert] [--freeze_style] [--freeze_decoder] [--yomi_error <yomi_error>]
 ```
 
@@ -90,8 +97,8 @@
 If using JP-Extra model:
 ```bash
 python train_ms_jp_extra.py [--repo_id <username>/<repo_name>] [--skip_default_style]
 ```
 
 Optional:
 - `--repo_id`: Hugging Face repository ID to upload the trained model to. You should have logged in using `huggingface-cli login` before running this command.
-- `--skip_default_style`: Skip making the default style vector. Use this if you want to resume training (since the default style vector is already made).
+- `--skip_default_style`: Skip making the default style vector. Use this if you want to resume training (since the default style vector has been already made).
```

### Comparing `style_bert_vits2-2.4.dev0/docs/paperspace.md` & `style_bert_vits2-2.5.0/docs/paperspace.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 mkdir -p /storage/sbv2
 cd /storage/sbv2
 git clone https://github.com/litagin02/Style-Bert-VITS2.git
 ```
 環境構築（デフォルトはPyTorch 1.x系、Python 3.9の模様）
 ```bash
 cd /storage/sbv2/Style-Bert-VITS2
-pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118 && pip install -r requirements.txt
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118 && pip install -r requirements.txt
 ```
 事前学習済みモデル等のダウンロード、またパスを`/notebooks/`以下のものに設定
 ```bash
 python initialize.py --skip_jvnv --dataset_root /notebooks/Data --assets_root /notebooks/model_assets
 ```
 
 ### 2. データセットの準備
@@ -53,15 +53,15 @@
 
 - zipファイルが音声ファイルのみの場合
 ```bash
 mkdir inputs
 unzip Foo.zip -d inputs
 cd /storage/sbv2/Style-Bert-VITS2
 python slice.py --model_name Foo -i /notebooks/inputs
-python transcribe.py --model_name Foo
+python transcribe.py --model_name Foo --use_hf_whisper
 ```
 
 それが終わったら、以下のコマンドで一括前処理を行う（パラメータは各自お好み、バッチサイズ5か6でVRAM 16GBギリくらい）。
 ```bash
 python preprocess_all.py --model_name Foo -b 5 -e 300 --use_jp_extra
 ```
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/constants.py` & `style_bert_vits2-2.5.0/style_bert_vits2/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 from style_bert_vits2.utils.strenum import StrEnum
 
 
 # Style-Bert-VITS2 のバージョン
-VERSION = "2.4.dev"
+VERSION = "2.5.0"
 
 # Style-Bert-VITS2 のベースディレクトリ
 BASE_DIR = Path(__file__).parent.parent
 
 
 # 利用可能な言語
 ## JP-Extra モデル利用時は JP 以外の言語の音声合成はできない
@@ -28,15 +28,15 @@
 # デフォルトのユーザー辞書ディレクトリ
 ## style_bert_vits2.nlp.japanese.user_dict モジュールのデフォルト値として利用される
 ## ライブラリとしての利用などで外部のユーザー辞書を指定したい場合は、user_dict 以下の各関数の実行時、引数に辞書データファイルのパスを指定する
 DEFAULT_USER_DICT_DIR = BASE_DIR / "dict_data"
 
 # デフォルトの推論パラメータ
 DEFAULT_STYLE = "Neutral"
-DEFAULT_STYLE_WEIGHT = 5.0
+DEFAULT_STYLE_WEIGHT = 1.0
 DEFAULT_SDP_RATIO = 0.2
 DEFAULT_NOISE = 0.6
 DEFAULT_NOISEW = 0.8
 DEFAULT_LENGTH = 1.0
 DEFAULT_LINE_SPLIT = True
 DEFAULT_SPLIT_INTERVAL = 0.5
 DEFAULT_ASSIST_TEXT_WEIGHT = 0.7
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/tts_model.py` & `style_bert_vits2-2.5.0/style_bert_vits2/tts_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import warnings
 from pathlib import Path
 from typing import Any, Optional, Union
 
-import gradio as gr
 import numpy as np
-import pyannote.audio
 import torch
-from gradio.processing_utils import convert_to_16_bit_wav
 from numpy.typing import NDArray
 from pydantic import BaseModel
 
 from style_bert_vits2.constants import (
     DEFAULT_ASSIST_TEXT_WEIGHT,
     DEFAULT_LENGTH,
     DEFAULT_LINE_SPLIT,
@@ -28,60 +24,86 @@
 from style_bert_vits2.models.models import SynthesizerTrn
 from style_bert_vits2.models.models_jp_extra import (
     SynthesizerTrn as SynthesizerTrnJPExtra,
 )
 from style_bert_vits2.voice import adjust_voice
 
 
+# Gradio の import は重いため、ここでは型チェック時のみ import する
+# ライブラリとしての利用を考慮し、TTSModelHolder の _for_gradio() 系メソッド以外では Gradio に依存しないようにする
+# _for_gradio() 系メソッドの戻り値の型アノテーションを文字列としているのは、Gradio なしで実行できるようにするため
+# if TYPE_CHECKING:
+#     import gradio as gr
+
+
 class TTSModel:
     """
     Style-Bert-Vits2 の音声合成モデルを操作するクラス。
     モデル/ハイパーパラメータ/スタイルベクトルのパスとデバイスを指定して初期化し、model.infer() メソッドを呼び出すと音声合成を行える。
     """
 
     def __init__(
-        self, model_path: Path, config_path: Path, style_vec_path: Path, device: str
+        self,
+        model_path: Path,
+        config_path: Union[Path, HyperParameters],
+        style_vec_path: Union[Path, NDArray[Any]],
+        device: str,
     ) -> None:
         """
         Style-Bert-Vits2 の音声合成モデルを初期化する。
         この時点ではモデルはロードされていない (明示的にロードしたい場合は model.load() を呼び出す)。
 
         Args:
             model_path (Path): モデル (.safetensors) のパス
-            config_path (Path): ハイパーパラメータ (config.json) のパス
-            style_vec_path (Path): スタイルベクトル (style_vectors.npy) のパス
+            config_path (Union[Path, HyperParameters]): ハイパーパラメータ (config.json) のパス (直接 HyperParameters を指定することも可能)
+            style_vec_path (Union[Path, NDArray[Any]]): スタイルベクトル (style_vectors.npy) のパス (直接 NDArray を指定することも可能)
             device (str): 音声合成時に利用するデバイス (cpu, cuda, mps など)
         """
 
         self.model_path: Path = model_path
-        self.config_path: Path = config_path
-        self.style_vec_path: Path = style_vec_path
         self.device: str = device
-        self.hyper_parameters: HyperParameters = HyperParameters.load_from_json(
-            self.config_path
-        )
+
+        # ハイパーパラメータの Pydantic モデルが直接指定された
+        if isinstance(config_path, HyperParameters):
+            self.config_path: Path = Path("")  # 互換性のため空の Path を設定
+            self.hyper_parameters: HyperParameters = config_path
+        # ハイパーパラメータのパスが指定された
+        else:
+            self.config_path: Path = config_path
+            self.hyper_parameters: HyperParameters = HyperParameters.load_from_json(
+                self.config_path
+            )
+
+        # スタイルベクトルの NDArray が直接指定された
+        if isinstance(style_vec_path, np.ndarray):
+            self.style_vec_path: Path = Path("")  # 互換性のため空の Path を設定
+            self.__style_vectors: NDArray[Any] = style_vec_path
+        # スタイルベクトルのパスが指定された
+        else:
+            self.style_vec_path: Path = style_vec_path
+            self.__style_vectors: NDArray[Any] = np.load(self.style_vec_path)
+
         self.spk2id: dict[str, int] = self.hyper_parameters.data.spk2id
         self.id2spk: dict[int, str] = {v: k for k, v in self.spk2id.items()}
 
         num_styles: int = self.hyper_parameters.data.num_styles
         if hasattr(self.hyper_parameters.data, "style2id"):
             self.style2id: dict[str, int] = self.hyper_parameters.data.style2id
         else:
             self.style2id: dict[str, int] = {str(i): i for i in range(num_styles)}
         if len(self.style2id) != num_styles:
             raise ValueError(
                 f"Number of styles ({num_styles}) does not match the number of style2id ({len(self.style2id)})"
             )
 
-        self.__style_vector_inference: Optional[pyannote.audio.Inference] = None
-        self.__style_vectors: NDArray[Any] = np.load(self.style_vec_path)
         if self.__style_vectors.shape[0] != num_styles:
             raise ValueError(
                 f"The number of styles ({num_styles}) does not match the number of style vectors ({self.__style_vectors.shape[0]})"
             )
+        self.__style_vector_inference: Optional[Any] = None
 
         self.__net_g: Union[SynthesizerTrn, SynthesizerTrnJPExtra, None] = None
 
     def load(self) -> None:
         """
         音声合成モデルをデバイスにロードする。
         """
@@ -117,30 +139,77 @@
         Args:
             audio_path (str): 音声ファイルのパス
             weight (float, optional): スタイルベクトルの重み. Defaults to 1.0.
         Returns:
             NDArray[Any]: スタイルベクトル
         """
 
-        # スタイルベクトルを取得するための推論モデルを初期化
         if self.__style_vector_inference is None:
+
+            # pyannote.audio は scikit-learn などの大量の重量級ライブラリに依存しているため、
+            # TTSModel.infer() に reference_audio_path を指定し音声からスタイルベクトルを推論する場合のみ遅延 import する
+            try:
+                import pyannote.audio
+            except ImportError:
+                raise ImportError(
+                    "pyannote.audio is required to infer style vector from audio"
+                )
+
+            # スタイルベクトルを取得するための推論モデルを初期化
             self.__style_vector_inference = pyannote.audio.Inference(
                 model=pyannote.audio.Model.from_pretrained(
                     "pyannote/wespeaker-voxceleb-resnet34-LM"
                 ),
                 window="whole",
             )
             self.__style_vector_inference.to(torch.device(self.device))
 
         # 音声からスタイルベクトルを推論
         xvec = self.__style_vector_inference(audio_path)
         mean = self.__style_vectors[0]
         xvec = mean + (xvec - mean) * weight
         return xvec
 
+    def __convert_to_16_bit_wav(self, data: NDArray[Any]) -> NDArray[Any]:
+        """
+        音声データを 16-bit int 形式に変換する。
+        gradio.processing_utils.convert_to_16_bit_wav() を移植したもの。
+
+        Args:
+            data (NDArray[Any]): 音声データ
+
+        Returns:
+            NDArray[Any]: 16-bit int 形式の音声データ
+        """
+        # Based on: https://docs.scipy.org/doc/scipy/reference/generated/scipy.io.wavfile.write.html
+        if data.dtype in [np.float64, np.float32, np.float16]:  # type: ignore
+            data = data / np.abs(data).max()
+            data = data * 32767
+            data = data.astype(np.int16)
+        elif data.dtype == np.int32:
+            data = data / 65536
+            data = data.astype(np.int16)
+        elif data.dtype == np.int16:
+            pass
+        elif data.dtype == np.uint16:
+            data = data - 32768
+            data = data.astype(np.int16)
+        elif data.dtype == np.uint8:
+            data = data * 257 - 32768
+            data = data.astype(np.int16)
+        elif data.dtype == np.int8:
+            data = data * 256
+            data = data.astype(np.int16)
+        else:
+            raise ValueError(
+                "Audio data cannot be converted automatically from "
+                f"{data.dtype} to 16-bit int format."
+            )
+        return data
+
     def infer(
         self,
         text: str,
         language: Languages = Languages.JP,
         speaker_id: int = 0,
         reference_audio_path: Optional[str] = None,
         sdp_ratio: float = DEFAULT_SDP_RATIO,
@@ -150,14 +219,15 @@
         line_split: bool = DEFAULT_LINE_SPLIT,
         split_interval: float = DEFAULT_SPLIT_INTERVAL,
         assist_text: Optional[str] = None,
         assist_text_weight: float = DEFAULT_ASSIST_TEXT_WEIGHT,
         use_assist_text: bool = False,
         style: str = DEFAULT_STYLE,
         style_weight: float = DEFAULT_STYLE_WEIGHT,
+        given_phone: Optional[list[str]] = None,
         given_tone: Optional[list[int]] = None,
         pitch_scale: float = 1.0,
         intonation_scale: float = 1.0,
     ) -> tuple[int, NDArray[Any]]:
         """
         テキストから音声を合成する。
 
@@ -166,24 +236,25 @@
             language (Languages, optional): 言語. Defaults to Languages.JP.
             speaker_id (int, optional): 話者 ID. Defaults to 0.
             reference_audio_path (Optional[str], optional): 音声スタイルの参照元の音声ファイルのパス. Defaults to None.
             sdp_ratio (float, optional): DP と SDP の混合比。0 で DP のみ、1で SDP のみを使用 (値を大きくするとテンポに緩急がつく). Defaults to DEFAULT_SDP_RATIO.
             noise (float, optional): DP に与えられるノイズ. Defaults to DEFAULT_NOISE.
             noise_w (float, optional): SDP に与えられるノイズ. Defaults to DEFAULT_NOISEW.
             length (float, optional): 生成音声の長さ（話速）のパラメータ。大きいほど生成音声が長くゆっくり、小さいほど短く早くなる。 Defaults to DEFAULT_LENGTH.
-            line_split (bool, optional): テキストを改行ごとに分割して生成するかどうか. Defaults to DEFAULT_LINE_SPLIT.
+            line_split (bool, optional): テキストを改行ごとに分割して生成するかどうか (True の場合 given_phone/given_tone は無視される). Defaults to DEFAULT_LINE_SPLIT.
             split_interval (float, optional): 改行ごとに分割する場合の無音 (秒). Defaults to DEFAULT_SPLIT_INTERVAL.
             assist_text (Optional[str], optional): 感情表現の参照元の補助テキスト. Defaults to None.
             assist_text_weight (float, optional): 感情表現の補助テキストを適用する強さ. Defaults to DEFAULT_ASSIST_TEXT_WEIGHT.
             use_assist_text (bool, optional): 音声合成時に感情表現の補助テキストを使用するかどうか. Defaults to False.
             style (str, optional): 音声スタイル (Neutral, Happy など). Defaults to DEFAULT_STYLE.
             style_weight (float, optional): 音声スタイルを適用する強さ. Defaults to DEFAULT_STYLE_WEIGHT.
+            given_phone (Optional[list[int]], optional): 読み上げテキストの読みを表す音素列。指定する場合は given_tone も別途指定が必要. Defaults to None.
             given_tone (Optional[list[int]], optional): アクセントのトーンのリスト. Defaults to None.
             pitch_scale (float, optional): ピッチの高さ (1.0 から変更すると若干音質が低下する). Defaults to 1.0.
-            intonation_scale (float, optional): イントネーションの高さ (1.0 から変更すると若干音質が低下する). Defaults to 1.0.
+            intonation_scale (float, optional): 抑揚の平均からの変化幅 (1.0 から変更すると若干音質が低下する). Defaults to 1.0.
 
         Returns:
             tuple[int, NDArray[Any]]: サンプリングレートと音声データ (16bit PCM)
         """
 
         logger.info(f"Start generating audio data from text:\n{text}")
         if language != "JP" and self.hyper_parameters.version.endswith("JP-Extra"):
@@ -217,14 +288,15 @@
                     language=language,
                     hps=self.hyper_parameters,
                     net_g=self.__net_g,
                     device=self.device,
                     assist_text=assist_text,
                     assist_text_weight=assist_text_weight,
                     style_vec=style_vector,
+                    given_phone=given_phone,
                     given_tone=given_tone,
                 )
         else:
             texts = text.split("\n")
             texts = [t for t in texts if t != ""]
             audios = []
             with torch.no_grad():
@@ -253,17 +325,15 @@
         if not (pitch_scale == 1.0 and intonation_scale == 1.0):
             _, audio = adjust_voice(
                 fs=self.hyper_parameters.data.sampling_rate,
                 wave=audio,
                 pitch_scale=pitch_scale,
                 intonation_scale=intonation_scale,
             )
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            audio = convert_to_16_bit_wav(audio)
+        audio = self.__convert_to_16_bit_wav(audio)
         return (self.hyper_parameters.data.sampling_rate, audio)
 
 
 class TTSModelInfo(BaseModel):
     name: str
     files: list[str]
     styles: list[str]
@@ -372,17 +442,17 @@
                 config_path=self.root_dir / model_name / "config.json",
                 style_vec_path=self.root_dir / model_name / "style_vectors.npy",
                 device=self.device,
             )
 
         return self.current_model
 
-    def get_model_for_gradio(
-        self, model_name: str, model_path_str: str
-    ) -> tuple[gr.Dropdown, gr.Button, gr.Dropdown]:
+    def get_model_for_gradio(self, model_name: str, model_path_str: str):
+        import gradio as gr
+
         model_path = Path(model_path_str)
         if model_name not in self.model_files_dict:
             raise ValueError(f"Model `{model_name}` is not found")
         if model_path not in self.model_files_dict[model_name]:
             raise ValueError(f"Model file `{model_path}` is not found")
         if (
             self.current_model is not None
@@ -406,22 +476,28 @@
         styles = list(self.current_model.style2id.keys())
         return (
             gr.Dropdown(choices=styles, value=styles[0]),  # type: ignore
             gr.Button(interactive=True, value="音声合成"),
             gr.Dropdown(choices=speakers, value=speakers[0]),  # type: ignore
         )
 
-    def update_model_files_for_gradio(self, model_name: str) -> gr.Dropdown:
-        model_files = self.model_files_dict[model_name]
+    def update_model_files_for_gradio(self, model_name: str):
+        import gradio as gr
+
+        model_files = [str(f) for f in self.model_files_dict[model_name]]
         return gr.Dropdown(choices=model_files, value=model_files[0])  # type: ignore
 
     def update_model_names_for_gradio(
         self,
-    ) -> tuple[gr.Dropdown, gr.Dropdown, gr.Button]:
+    ):
+        import gradio as gr
+
         self.refresh()
         initial_model_name = self.model_names[0]
-        initial_model_files = self.model_files_dict[initial_model_name]
+        initial_model_files = [
+            str(f) for f in self.model_files_dict[initial_model_name]
+        ]
         return (
             gr.Dropdown(choices=self.model_names, value=initial_model_name),  # type: ignore
             gr.Dropdown(choices=initial_model_files, value=initial_model_files[0]),  # type: ignore
             gr.Button(interactive=False),  # For tts_button
         )
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/voice.py` & `style_bert_vits2-2.5.0/style_bert_vits2/voice.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 def adjust_voice(
     fs: int,
     wave: NDArray[Any],
     pitch_scale: float = 1.0,
     intonation_scale: float = 1.0,
 ) -> tuple[int, NDArray[Any]]:
     """
-    音声のピッチとイントネーションを調整する。
+    音声のピッチと抑揚を調整する。
     変更すると若干音質が劣化するので、どちらも初期値のままならそのまま返す。
 
     Args:
         fs (int): 音声のサンプリング周波数
         wave (NDArray[Any]): 音声データ
         pitch_scale (float, optional): ピッチの高さ. Defaults to 1.0.
-        intonation_scale (float, optional): イントネーションの平均からの変更比率. Defaults to 1.0.
+        intonation_scale (float, optional): 抑揚の平均からの変更比率. Defaults to 1.0.
 
     Returns:
         tuple[int, NDArray[Any]]: 調整後の音声データのサンプリング周波数と音声データ
     """
 
     if pitch_scale == 1.0 and intonation_scale == 1.0:
         # 初期値の場合は、音質劣化を避けるためにそのまま返す
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/attentions.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/attentions.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/commons.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/commons.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/hyper_parameters.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/hyper_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Style-Bert-VITS2 モデルのハイパーパラメータを表す Pydantic モデル。
-デフォルト値は configs/configs_jp_extra.json 内の定義と概ね同一で、
+デフォルト値は configs/config_jp_extra.json 内の定義と概ね同一で、
 万が一ロードした config.json に存在しないキーがあった際のフェイルセーフとして適用される。
 """
 
 from pathlib import Path
 from typing import Optional, Union
 
 from pydantic import BaseModel, ConfigDict
@@ -121,9 +121,9 @@
         Args:
             json_path (Union[str, Path]): JSON ファイルのパス
 
         Returns:
             HyperParameters: ハイパーパラメータ
         """
 
-        with open(json_path, "r", encoding="utf-8") as f:
+        with open(json_path, encoding="utf-8") as f:
             return HyperParameters.model_validate_json(f.read())
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/models.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,15 +782,15 @@
                     stride=(2, 2),
                     padding=(1, 1),
                 )
             )
             for i in range(K)
         ]
         self.convs = nn.ModuleList(convs)
-        # self.wns = nn.ModuleList([weight_norm(num_features=ref_enc_filters[i]) for i in range(K)]) # noqa: E501
+        # self.wns = nn.ModuleList([weight_norm(num_features=ref_enc_filters[i]) for i in range(K)])
 
         out_channels = self.calculate_channels(spec_channels, 3, 2, 1, K)
         self.gru = nn.GRU(
             input_size=ref_enc_filters[-1] * out_channels,
             hidden_size=256 // 2,
             batch_first=True,
         )
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/models_jp_extra.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/models_jp_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -840,15 +840,15 @@
                     stride=(2, 2),
                     padding=(1, 1),
                 )
             )
             for i in range(K)
         ]
         self.convs = nn.ModuleList(convs)
-        # self.wns = nn.ModuleList([weight_norm(num_features=ref_enc_filters[i]) for i in range(K)]) # noqa: E501
+        # self.wns = nn.ModuleList([weight_norm(num_features=ref_enc_filters[i]) for i in range(K)])
 
         out_channels = self.calculate_channels(spec_channels, 3, 2, 1, K)
         self.gru = nn.GRU(
             input_size=ref_enc_filters[-1] * out_channels,
             hidden_size=256 // 2,
             batch_first=True,
         )
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/modules.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/modules.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/monotonic_alignment.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/monotonic_alignment.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/transforms.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/transforms.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/__init__.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 import numpy as np
 import torch
 from numpy.typing import NDArray
-from scipy.io.wavfile import read
 
 from style_bert_vits2.logging import logger
 from style_bert_vits2.models.utils import checkpoints  # type: ignore
 from style_bert_vits2.models.utils import safetensors  # type: ignore
 
 
 if TYPE_CHECKING:
@@ -158,14 +157,21 @@
     Args:
         full_path (Union[str, Path]): 音声ファイルのパス
 
     Returns:
         tuple[torch.FloatTensor, int]: 音声データのテンソルとサンプリングレート
     """
 
+    # この関数は学習時以外使われないため、ライブラリとしての style_bert_vits2 が
+    # 重たい scipy に依存しないように遅延 import する
+    try:
+        from scipy.io.wavfile import read
+    except ImportError:
+        raise ImportError("scipy is required to load wav file")
+
     sampling_rate, data = read(full_path)
     return torch.FloatTensor(data.astype(np.float32)), sampling_rate
 
 
 def load_filepaths_and_text(
     filename: Union[str, Path], split: str = "|"
 ) -> list[list[str]]:
@@ -176,15 +182,15 @@
         filename (Union[str, Path]): ファイルのパス
         split (str): ファイルの区切り文字 (デフォルト: "|")
 
     Returns:
         list[list[str]]: ファイルパスとテキストのリスト
     """
 
-    with open(filename, "r", encoding="utf-8") as f:
+    with open(filename, encoding="utf-8") as f:
         filepaths_and_text = [line.strip().split(split) for line in f]
     return filepaths_and_text
 
 
 def get_logger(
     model_dir_path: Union[str, Path], filename: str = "train.log"
 ) -> logging.Logger:
@@ -235,28 +241,24 @@
     Args:
         model_dir_path (Union[str, Path]): モデルのディレクトリのパス
     """
 
     source_dir = os.path.dirname(os.path.realpath(__file__))
     if not os.path.exists(os.path.join(source_dir, ".git")):
         logger.warning(
-            "{} is not a git repository, therefore hash value comparison will be ignored.".format(
-                source_dir
-            )
+            f"{source_dir} is not a git repository, therefore hash value comparison will be ignored."
         )
         return
 
     cur_hash = subprocess.getoutput("git rev-parse HEAD")
 
     path = os.path.join(model_dir_path, "githash")
     if os.path.exists(path):
-        with open(path, "r", encoding="utf-8") as f:
+        with open(path, encoding="utf-8") as f:
             saved_hash = f.read()
         if saved_hash != cur_hash:
             logger.warning(
-                "git hash values are different. {}(saved) != {}(current)".format(
-                    saved_hash[:8], cur_hash[:8]
-                )
+                f"git hash values are different. {saved_hash[:8]}(saved) != {cur_hash[:8]}(current)"
             )
     else:
         with open(path, "w", encoding="utf-8") as f:
             f.write(cur_hash)
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/checkpoints.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/models/utils/safetensors.py` & `style_bert_vits2-2.5.0/style_bert_vits2/models/utils/safetensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     if hasattr(model, "module"):
         state_dict = model.module.state_dict()
     else:
         state_dict = model.state_dict()
     keys = []
     for k in state_dict:
         if "enc_q" in k and for_infer:
-            continue  # noqa: E701
+            continue
         keys.append(k)
 
     new_dict = (
         {k: state_dict[k].half() for k in keys}
         if is_half
         else {k: state_dict[k] for k in keys}
     )
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/__init__.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/bert_models.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/bert_models.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/symbols.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/symbols.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/bert_feature.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/bert_feature.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/g2p.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/g2p.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import jieba.posseg as psg
 from pypinyin import Style, lazy_pinyin
 
 from style_bert_vits2.nlp.chinese.tone_sandhi import ToneSandhi
 from style_bert_vits2.nlp.symbols import PUNCTUATIONS
 
 
-with open(Path(__file__).parent / "opencpop-strict.txt", "r", encoding="utf-8") as f:
+with open(Path(__file__).parent / "opencpop-strict.txt", encoding="utf-8") as f:
     __PINYIN_TO_SYMBOL_MAP = {
         line.split("\t")[0]: line.strip().split("\t")[1] for line in f.readlines()
     }
 
 
 def g2p(text: str) -> tuple[list[str], list[int], list[int]]:
     pattern = r"(?<=[{0}])\s*".format("".join(PUNCTUATIONS))
@@ -69,37 +69,37 @@
                 if c:
                     # 多音节
                     v_rep_map = {
                         "uei": "ui",
                         "iou": "iu",
                         "uen": "un",
                     }
-                    if v_without_tone in v_rep_map.keys():
+                    if v_without_tone in v_rep_map:
                         pinyin = c + v_rep_map[v_without_tone]
                 else:
                     # 单音节
                     pinyin_rep_map = {
                         "ing": "ying",
                         "i": "yi",
                         "in": "yin",
                         "u": "wu",
                     }
-                    if pinyin in pinyin_rep_map.keys():
+                    if pinyin in pinyin_rep_map:
                         pinyin = pinyin_rep_map[pinyin]
                     else:
                         single_rep_map = {
                             "v": "yu",
                             "e": "e",
                             "i": "y",
                             "u": "w",
                         }
-                        if pinyin[0] in single_rep_map.keys():
+                        if pinyin[0] in single_rep_map:
                             pinyin = single_rep_map[pinyin[0]] + pinyin[1:]
 
-                assert pinyin in __PINYIN_TO_SYMBOL_MAP.keys(), (
+                assert pinyin in __PINYIN_TO_SYMBOL_MAP, (
                     pinyin,
                     seg,
                     raw_pinyin,
                 )
                 phone = __PINYIN_TO_SYMBOL_MAP[pinyin].split(" ")
                 word2ph.append(len(phone))
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/normalizer.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/normalizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 import re
 
 import cn2an
 
 from style_bert_vits2.nlp.symbols import PUNCTUATIONS
 
 
+__REPLACE_MAP = {
+    "：": ",",
+    "；": ",",
+    "，": ",",
+    "。": ".",
+    "！": "!",
+    "？": "?",
+    "\n": ".",
+    "·": ",",
+    "、": ",",
+    "...": "…",
+    "$": ".",
+    "“": "'",
+    "”": "'",
+    '"': "'",
+    "‘": "'",
+    "’": "'",
+    "（": "'",
+    "）": "'",
+    "(": "'",
+    ")": "'",
+    "《": "'",
+    "》": "'",
+    "【": "'",
+    "】": "'",
+    "[": "'",
+    "]": "'",
+    "—": "-",
+    "～": "-",
+    "~": "-",
+    "「": "'",
+    "」": "'",
+}
+
+
 def normalize_text(text: str) -> str:
     numbers = re.findall(r"\d+(?:\.?\d+)?", text)
     for number in numbers:
         text = text.replace(number, cn2an.an2cn(number), 1)
     text = replace_punctuation(text)
     return text
 
 
 def replace_punctuation(text: str) -> str:
 
-    REPLACE_MAP = {
-        "：": ",",
-        "；": ",",
-        "，": ",",
-        "。": ".",
-        "！": "!",
-        "？": "?",
-        "\n": ".",
-        "·": ",",
-        "、": ",",
-        "...": "…",
-        "$": ".",
-        "“": "'",
-        "”": "'",
-        '"': "'",
-        "‘": "'",
-        "’": "'",
-        "（": "'",
-        "）": "'",
-        "(": "'",
-        ")": "'",
-        "《": "'",
-        "》": "'",
-        "【": "'",
-        "】": "'",
-        "[": "'",
-        "]": "'",
-        "—": "-",
-        "～": "-",
-        "~": "-",
-        "「": "'",
-        "」": "'",
-    }
-
     text = text.replace("嗯", "恩").replace("呣", "母")
-    pattern = re.compile("|".join(re.escape(p) for p in REPLACE_MAP.keys()))
+    pattern = re.compile("|".join(re.escape(p) for p in __REPLACE_MAP))
 
-    replaced_text = pattern.sub(lambda x: REPLACE_MAP[x.group()], text)
+    replaced_text = pattern.sub(lambda x: __REPLACE_MAP[x.group()], text)
 
     replaced_text = re.sub(
         r"[^\u4e00-\u9fa5" + "".join(PUNCTUATIONS) + r"]+", "", replaced_text
     )
 
     return replaced_text
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/opencpop-strict.txt` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/opencpop-strict.txt`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/chinese/tone_sandhi.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/chinese/tone_sandhi.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,49 +467,49 @@
                 j - 1 >= 0
                 and item == word[j - 1]
                 and pos[0] in {"n", "v", "a"}
                 and word not in self.must_not_neural_tone_words
             ):
                 finals[j] = finals[j][:-1] + "5"
         ge_idx = word.find("个")
-        if len(word) >= 1 and word[-1] in "吧呢啊呐噻嘛吖嗨呐哦哒额滴哩哟喽啰耶喔诶":
-            finals[-1] = finals[-1][:-1] + "5"
-        elif len(word) >= 1 and word[-1] in "的地得":
-            finals[-1] = finals[-1][:-1] + "5"
-        # e.g. 走了, 看着, 去过
-        # elif len(word) == 1 and word in "了着过" and pos in {"ul", "uz", "ug"}:
-        #     finals[-1] = finals[-1][:-1] + "5"
-        elif (
-            len(word) > 1
-            and word[-1] in "们子"
-            and pos in {"r", "n"}
-            and word not in self.must_not_neural_tone_words
+        if (
+            len(word) >= 1
+            and word[-1] in "吧呢啊呐噻嘛吖嗨呐哦哒额滴哩哟喽啰耶喔诶"
+            or len(word) >= 1
+            and word[-1] in "的地得"
+            or (
+                (
+                    len(word) > 1
+                    and word[-1] in "们子"
+                    and pos in {"r", "n"}
+                    and word not in self.must_not_neural_tone_words
+                )
+                or len(word) > 1
+                and word[-1] in "上下里"
+                and pos in {"s", "l", "f"}
+            )
+            or len(word) > 1
+            and word[-1] in "来去"
+            and word[-2] in "上下进出回过起开"
         ):
             finals[-1] = finals[-1][:-1] + "5"
-        # e.g. 桌上, 地下, 家里
-        elif len(word) > 1 and word[-1] in "上下里" and pos in {"s", "l", "f"}:
-            finals[-1] = finals[-1][:-1] + "5"
-        # e.g. 上来, 下去
-        elif len(word) > 1 and word[-1] in "来去" and word[-2] in "上下进出回过起开":
-            finals[-1] = finals[-1][:-1] + "5"
         # 个做量词
         elif (
             ge_idx >= 1
             and (
                 word[ge_idx - 1].isnumeric()
                 or word[ge_idx - 1] in "几有两半多各整每做是"
             )
         ) or word == "个":
             finals[ge_idx] = finals[ge_idx][:-1] + "5"
-        else:
-            if (
-                word in self.must_neural_tone_words
-                or word[-2:] in self.must_neural_tone_words
-            ):
-                finals[-1] = finals[-1][:-1] + "5"
+        elif (
+            word in self.must_neural_tone_words
+            or word[-2:] in self.must_neural_tone_words
+        ):
+            finals[-1] = finals[-1][:-1] + "5"
 
         word_list = self._split_word(word)
         finals_list = [finals[: len(word_list[0])], finals[len(word_list[0]) :]]
         for i, word in enumerate(word_list):
             # conventional neural in Chinese
             if (
                 word in self.must_neural_tone_words
@@ -545,18 +545,16 @@
         else:
             for i, char in enumerate(word):
                 if char == "一" and i + 1 < len(word):
                     # "一" before tone4 should be yi2, e.g. 一段
                     if finals[i + 1][-1] == "4":
                         finals[i] = finals[i][:-1] + "2"
                     # "一" before non-tone4 should be yi4, e.g. 一天
-                    else:
-                        # "一" 后面如果是标点，还读一声
-                        if word[i + 1] not in self.punc:
-                            finals[i] = finals[i][:-1] + "4"
+                    elif word[i + 1] not in self.punc:
+                        finals[i] = finals[i][:-1] + "4"
         return finals
 
     def _split_word(self, word: str) -> list[str]:
         word_list = jieba.cut_for_search(word)
         word_list = sorted(word_list, key=lambda i: len(i), reverse=False)  # type: ignore
         first_subword = word_list[0]
         first_begin_idx = word.find(first_subword)
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/bert_feature.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/bert_feature.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     return g2p_dict
 
 
 def read_dict() -> dict[str, list[list[str]]]:
     g2p_dict = {}
     start_line = 49
-    with open(CMU_DICT_PATH, "r", encoding="utf-8") as f:
+    with open(CMU_DICT_PATH, encoding="utf-8") as f:
         line = f.readline()
         line_index = 1
         while line:
             if line_index >= start_line:
                 line = line.strip()
                 word_split = line.split("  ")
                 word = word_split[0]
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict.rep` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict.rep`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/cmudict_cache.pickle` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/cmudict_cache.pickle`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/g2p.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/g2p.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,139 +4,134 @@
 
 from style_bert_vits2.constants import Languages
 from style_bert_vits2.nlp import bert_models
 from style_bert_vits2.nlp.english.cmudict import get_dict
 from style_bert_vits2.nlp.symbols import PUNCTUATIONS, SYMBOLS
 
 
-def g2p(text: str) -> tuple[list[str], list[int], list[int]]:
-
-    ARPA = {
-        "AH0",
-        "S",
-        "AH1",
-        "EY2",
-        "AE2",
-        "EH0",
-        "OW2",
-        "UH0",
-        "NG",
-        "B",
-        "G",
-        "AY0",
-        "M",
-        "AA0",
-        "F",
-        "AO0",
-        "ER2",
-        "UH1",
-        "IY1",
-        "AH2",
-        "DH",
-        "IY0",
-        "EY1",
-        "IH0",
-        "K",
-        "N",
-        "W",
-        "IY2",
-        "T",
-        "AA1",
-        "ER1",
-        "EH2",
-        "OY0",
-        "UH2",
-        "UW1",
-        "Z",
-        "AW2",
-        "AW1",
-        "V",
-        "UW2",
-        "AA2",
-        "ER",
-        "AW0",
-        "UW0",
-        "R",
-        "OW1",
-        "EH1",
-        "ZH",
-        "AE0",
-        "IH2",
-        "IH",
-        "Y",
-        "JH",
-        "P",
-        "AY1",
-        "EY0",
-        "OY2",
-        "TH",
-        "HH",
-        "D",
-        "ER0",
-        "CH",
-        "AO1",
-        "AE1",
-        "AO2",
-        "OY1",
-        "AY2",
-        "IH1",
-        "OW0",
-        "L",
-        "SH",
-    }
+# Initialize global variables once
+ARPA = {
+    "AH0",
+    "S",
+    "AH1",
+    "EY2",
+    "AE2",
+    "EH0",
+    "OW2",
+    "UH0",
+    "NG",
+    "B",
+    "G",
+    "AY0",
+    "M",
+    "AA0",
+    "F",
+    "AO0",
+    "ER2",
+    "UH1",
+    "IY1",
+    "AH2",
+    "DH",
+    "IY0",
+    "EY1",
+    "IH0",
+    "K",
+    "N",
+    "W",
+    "IY2",
+    "T",
+    "AA1",
+    "ER1",
+    "EH2",
+    "OY0",
+    "UH2",
+    "UW1",
+    "Z",
+    "AW2",
+    "AW1",
+    "V",
+    "UW2",
+    "AA2",
+    "ER",
+    "AW0",
+    "UW0",
+    "R",
+    "OW1",
+    "EH1",
+    "ZH",
+    "AE0",
+    "IH2",
+    "IH",
+    "Y",
+    "JH",
+    "P",
+    "AY1",
+    "EY0",
+    "OY2",
+    "TH",
+    "HH",
+    "D",
+    "ER0",
+    "CH",
+    "AO1",
+    "AE1",
+    "AO2",
+    "OY1",
+    "AY2",
+    "IH1",
+    "OW0",
+    "L",
+    "SH",
+}
+_g2p = G2p()
+eng_dict = get_dict()
 
-    _g2p = G2p()
 
+def g2p(text: str) -> tuple[list[str], list[int], list[int]]:
     phones = []
     tones = []
     phone_len = []
-    # tokens = [tokenizer.tokenize(i) for i in words]
     words = __text_to_words(text)
-    eng_dict = get_dict()
 
     for word in words:
         temp_phones, temp_tones = [], []
-        if len(word) > 1:
-            if "'" in word:
-                word = ["".join(word)]
+        if len(word) > 1 and "'" in word:
+            word = ["".join(word)]
+
         for w in word:
             if w in PUNCTUATIONS:
                 temp_phones.append(w)
                 temp_tones.append(0)
                 continue
             if w.upper() in eng_dict:
                 phns, tns = __refine_syllables(eng_dict[w.upper()])
                 temp_phones += [__post_replace_ph(i) for i in phns]
                 temp_tones += tns
-                # w2ph.append(len(phns))
             else:
-                phone_list = list(filter(lambda p: p != " ", _g2p(w)))  # type: ignore
-                phns = []
-                tns = []
+                phone_list = list(filter(lambda p: p != " ", _g2p(w)))
+                phns, tns = [], []
                 for ph in phone_list:
                     if ph in ARPA:
                         ph, tn = __refine_ph(ph)
                         phns.append(ph)
                         tns.append(tn)
                     else:
                         phns.append(ph)
                         tns.append(0)
                 temp_phones += [__post_replace_ph(i) for i in phns]
                 temp_tones += tns
+
         phones += temp_phones
         tones += temp_tones
         phone_len.append(len(temp_phones))
-        # phones = [post_replace_ph(i) for i in phones]
 
     word2ph = []
     for token, pl in zip(words, phone_len):
         word_len = len(token)
-
-        aaa = __distribute_phone(pl, word_len)
-        word2ph += aaa
+        word2ph += __distribute_phone(pl, word_len)
 
     phones = ["_"] + phones + ["_"]
     tones = [0] + tones + [0]
     word2ph = [1] + word2ph + [1]
     assert len(phones) == len(tones), text
     assert len(phones) == sum(word2ph), text
 
@@ -155,21 +150,19 @@
         "·": ",",
         "、": ",",
         "…": "...",
         "···": "...",
         "・・・": "...",
         "v": "V",
     }
-    if ph in REPLACE_MAP.keys():
+    if ph in REPLACE_MAP:
         ph = REPLACE_MAP[ph]
     if ph in SYMBOLS:
         return ph
-    if ph not in SYMBOLS:
-        ph = "UNK"
-    return ph
+    return "UNK"
 
 
 def __refine_ph(phn: str) -> tuple[str, int]:
     tone = 0
     if re.search(r"\d$", phn):
         tone = int(phn[-1]) + 1
         phn = phn[:-1]
@@ -178,16 +171,15 @@
     return phn.lower(), tone
 
 
 def __refine_syllables(syllables: list[list[str]]) -> tuple[list[str], list[int]]:
     tones = []
     phonemes = []
     for phn_list in syllables:
-        for i in range(len(phn_list)):
-            phn = phn_list[i]
+        for phn in phn_list:
             phn, tone = __refine_ph(phn)
             phonemes.append(phn)
             tones.append(tone)
     return phonemes, tones
 
 
 def __distribute_phone(n_phone: int, n_word: int) -> list[int]:
@@ -202,32 +194,30 @@
 def __text_to_words(text: str) -> list[list[str]]:
     tokenizer = bert_models.load_tokenizer(Languages.EN)
     tokens = tokenizer.tokenize(text)
     words = []
     for idx, t in enumerate(tokens):
         if t.startswith("▁"):
             words.append([t[1:]])
-        else:
-            if t in PUNCTUATIONS:
-                if idx == len(tokens) - 1:
-                    words.append([f"{t}"])
-                else:
-                    if (
-                        not tokens[idx + 1].startswith("▁")
-                        and tokens[idx + 1] not in PUNCTUATIONS
-                    ):
-                        if idx == 0:
-                            words.append([])
-                        words[-1].append(f"{t}")
-                    else:
-                        words.append([f"{t}"])
-            else:
+        elif t in PUNCTUATIONS:
+            if idx == len(tokens) - 1:
+                words.append([f"{t}"])
+            elif (
+                not tokens[idx + 1].startswith("▁")
+                and tokens[idx + 1] not in PUNCTUATIONS
+            ):
                 if idx == 0:
                     words.append([])
                 words[-1].append(f"{t}")
+            else:
+                words.append([f"{t}"])
+        else:
+            if idx == 0:
+                words.append([])
+            words[-1].append(f"{t}")
     return words
 
 
 if __name__ == "__main__":
     # print(get_dict())
     # print(eng_word_to_phoneme("hello"))
     print(g2p("In this paper, we propose 1 DSPGAN, a GAN-based universal vocoder."))
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/english/normalizer.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/english/normalizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         "—": "-",
         "−": "-",
         "～": "-",
         "~": "-",
         "「": "'",
         "」": "'",
     }
-    pattern = re.compile("|".join(re.escape(p) for p in REPLACE_MAP.keys()))
+    pattern = re.compile("|".join(re.escape(p) for p in REPLACE_MAP))
     replaced_text = pattern.sub(lambda x: REPLACE_MAP[x.group()], text)
     # replaced_text = re.sub(
     #     r"[^\u3040-\u309F\u30A0-\u30FF\u4E00-\u9FFF\u3400-\u4DBF\u3005"
     #     + "".join(punctuation)
     #     + r"]+",
     #     "",
     #     replaced_text,
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/bert_feature.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/bert_feature.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/g2p_utils.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/g2p_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from style_bert_vits2.nlp.japanese.g2p import g2p
 from style_bert_vits2.nlp.japanese.mora_list import (
+    CONSONANTS,
     MORA_KATA_TO_MORA_PHONEMES,
     MORA_PHONEMES_TO_MORA_KATA,
 )
 from style_bert_vits2.nlp.symbols import PUNCTUATIONS
 
 
 def g2kata_tone(norm_text: str) -> list[tuple[str, int]]:
@@ -29,23 +30,14 @@
     Args:
         phone_tone: 音素と音高のリスト。
 
     Returns:
         カタカナと音高のリスト。
     """
 
-    # 子音の集合
-    CONSONANTS = set(
-        [
-            consonant
-            for consonant, _ in MORA_KATA_TO_MORA_PHONEMES.values()
-            if consonant is not None
-        ]
-    )
-
     phone_tone = phone_tone[1:]  # 最初の("_", 0)を無視
     phones = [phone for phone, _ in phone_tone]
     tones = [tone for _, tone in phone_tone]
     result: list[tuple[str, int]] = []
     current_mora = ""
     for phone, next_phone, tone, next_tone in zip(phones, phones[1:], tones, tones[1:]):
         # zip の関係で最後の ("_", 0) は無視されている
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/mora_list.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/mora_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,7 +230,19 @@
 
 # モーラのカタカナ表記と音素の対応表
 # 例: "ヴォ" -> ("v", "o"), "ア" -> (None, "a")
 MORA_KATA_TO_MORA_PHONEMES: dict[str, tuple[Optional[str], str]] = {
     kana: (consonant, vowel)
     for [kana, consonant, vowel] in __MORA_LIST_MINIMUM + __MORA_LIST_ADDITIONAL
 }
+
+# 子音の集合
+CONSONANTS = set(
+    [
+        consonant
+        for consonant, _ in MORA_KATA_TO_MORA_PHONEMES.values()
+        if consonant is not None
+    ]
+)
+
+# 母音の集合 (便宜上「ん」を含める)
+VOWELS = {"a", "i", "u", "e", "o", "N"}
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/normalizer.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/normalizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,89 @@
 import unicodedata
 
 from num2words import num2words
 
 from style_bert_vits2.nlp.symbols import PUNCTUATIONS
 
 
+# 記号類の正規化マップ
+__REPLACE_MAP = {
+    "：": ",",
+    "；": ",",
+    "，": ",",
+    "。": ".",
+    "！": "!",
+    "？": "?",
+    "\n": ".",
+    "．": ".",
+    "…": "...",
+    "···": "...",
+    "・・・": "...",
+    "·": ",",
+    "・": ",",
+    "、": ",",
+    "$": ".",
+    "“": "'",
+    "”": "'",
+    '"': "'",
+    "‘": "'",
+    "’": "'",
+    "（": "'",
+    "）": "'",
+    "(": "'",
+    ")": "'",
+    "《": "'",
+    "》": "'",
+    "【": "'",
+    "】": "'",
+    "[": "'",
+    "]": "'",
+    # NFKC 正規化後のハイフン・ダッシュの変種を全て通常半角ハイフン - \u002d に変換
+    "\u02d7": "\u002d",  # ˗, Modifier Letter Minus Sign
+    "\u2010": "\u002d",  # ‐, Hyphen,
+    # "\u2011": "\u002d",  # ‑, Non-Breaking Hyphen, NFKC により \u2010 に変換される
+    "\u2012": "\u002d",  # ‒, Figure Dash
+    "\u2013": "\u002d",  # –, En Dash
+    "\u2014": "\u002d",  # —, Em Dash
+    "\u2015": "\u002d",  # ―, Horizontal Bar
+    "\u2043": "\u002d",  # ⁃, Hyphen Bullet
+    "\u2212": "\u002d",  # −, Minus Sign
+    "\u23af": "\u002d",  # ⎯, Horizontal Line Extension
+    "\u23e4": "\u002d",  # ⏤, Straightness
+    "\u2500": "\u002d",  # ─, Box Drawings Light Horizontal
+    "\u2501": "\u002d",  # ━, Box Drawings Heavy Horizontal
+    "\u2e3a": "\u002d",  # ⸺, Two-Em Dash
+    "\u2e3b": "\u002d",  # ⸻, Three-Em Dash
+    # "～": "-",  # これは長音記号「ー」として扱うよう変更
+    # "~": "-",  # これも長音記号「ー」として扱うよう変更
+    "「": "'",
+    "」": "'",
+}
+# 記号類の正規化パターン
+__REPLACE_PATTERN = re.compile("|".join(re.escape(p) for p in __REPLACE_MAP))
+# 句読点等の正規化パターン
+__PUNCTUATION_CLEANUP_PATTERN = re.compile(
+    # ↓ ひらがな、カタカナ、漢字
+    r"[^\u3040-\u309F\u30A0-\u30FF\u4E00-\u9FFF\u3400-\u4DBF\u3005"
+    # ↓ 半角アルファベット（大文字と小文字）
+    + r"\u0041-\u005A\u0061-\u007A"
+    # ↓ 全角アルファベット（大文字と小文字）
+    + r"\uFF21-\uFF3A\uFF41-\uFF5A"
+    # ↓ ギリシャ文字
+    + r"\u0370-\u03FF\u1F00-\u1FFF"
+    # ↓ "!", "?", "…", ",", ".", "'", "-", 但し`…`はすでに`...`に変換されている
+    + "".join(PUNCTUATIONS) + r"]+",  # fmt: skip
+)
+# 数字・通貨記号の正規化パターン
+__CURRENCY_MAP = {"$": "ドル", "¥": "円", "£": "ポンド", "€": "ユーロ"}
+__CURRENCY_PATTERN = re.compile(r"([$¥£€])([0-9.]*[0-9])")
+__NUMBER_PATTERN = re.compile(r"[0-9]+(\.[0-9]+)?")
+__NUMBER_WITH_SEPARATOR_PATTERN = re.compile("[0-9]{1,3}(,[0-9]{3})+")
+
+
 def normalize_text(text: str) -> str:
     """
     日本語のテキストを正規化する。
     結果は、ちょうど次の文字のみからなる：
     - ひらがな
     - カタカナ（全角長音記号「ー」が入る！）
     - 漢字
@@ -32,17 +107,18 @@
 
     Returns:
         str: 正規化されたテキスト
     """
 
     res = unicodedata.normalize("NFKC", text)  # ここでアルファベットは半角になる
     res = __convert_numbers_to_words(res)  # 「100円」→「百円」等
-    # 「～」と「~」も長音記号として扱う
+    # 「～」と「〜」と「~」も長音記号として扱う
     res = res.replace("~", "ー")
     res = res.replace("～", "ー")
+    res = res.replace("〜", "ー")
 
     res = replace_punctuation(res)  # 句読点等正規化、読めない文字を削除
 
     # 結合文字の濁点・半濁点を削除
     # 通常の「ば」等はそのままのこされる、「あ゛」は上で「あ゙」になりここで「あ」になる
     res = res.replace("\u3099", "")  # 結合文字の濁点を削除、る゙ → る
     res = res.replace("\u309A", "")  # 結合文字の半濁点を削除、な゚ → な
@@ -57,88 +133,19 @@
     Args:
         text (str): 正規化するテキスト
 
     Returns:
         str: 正規化されたテキスト
     """
 
-    # 記号類の正規化変換マップ
-    REPLACE_MAP = {
-        "：": ",",
-        "；": ",",
-        "，": ",",
-        "。": ".",
-        "！": "!",
-        "？": "?",
-        "\n": ".",
-        "．": ".",
-        "…": "...",
-        "···": "...",
-        "・・・": "...",
-        "·": ",",
-        "・": ",",
-        "、": ",",
-        "$": ".",
-        "“": "'",
-        "”": "'",
-        '"': "'",
-        "‘": "'",
-        "’": "'",
-        "（": "'",
-        "）": "'",
-        "(": "'",
-        ")": "'",
-        "《": "'",
-        "》": "'",
-        "【": "'",
-        "】": "'",
-        "[": "'",
-        "]": "'",
-        # NFKC 正規化後のハイフン・ダッシュの変種を全て通常半角ハイフン - \u002d に変換
-        "\u02d7": "\u002d",  # ˗, Modifier Letter Minus Sign
-        "\u2010": "\u002d",  # ‐, Hyphen,
-        # "\u2011": "\u002d",  # ‑, Non-Breaking Hyphen, NFKC により \u2010 に変換される
-        "\u2012": "\u002d",  # ‒, Figure Dash
-        "\u2013": "\u002d",  # –, En Dash
-        "\u2014": "\u002d",  # —, Em Dash
-        "\u2015": "\u002d",  # ―, Horizontal Bar
-        "\u2043": "\u002d",  # ⁃, Hyphen Bullet
-        "\u2212": "\u002d",  # −, Minus Sign
-        "\u23af": "\u002d",  # ⎯, Horizontal Line Extension
-        "\u23e4": "\u002d",  # ⏤, Straightness
-        "\u2500": "\u002d",  # ─, Box Drawings Light Horizontal
-        "\u2501": "\u002d",  # ━, Box Drawings Heavy Horizontal
-        "\u2e3a": "\u002d",  # ⸺, Two-Em Dash
-        "\u2e3b": "\u002d",  # ⸻, Three-Em Dash
-        # "～": "-",  # これは長音記号「ー」として扱うよう変更
-        # "~": "-",  # これも長音記号「ー」として扱うよう変更
-        "「": "'",
-        "」": "'",
-    }
-
-    pattern = re.compile("|".join(re.escape(p) for p in REPLACE_MAP.keys()))
-
     # 句読点を辞書で置換
-    replaced_text = pattern.sub(lambda x: REPLACE_MAP[x.group()], text)
+    replaced_text = __REPLACE_PATTERN.sub(lambda x: __REPLACE_MAP[x.group()], text)
 
-    replaced_text = re.sub(
-        # ↓ ひらがな、カタカナ、漢字
-        r"[^\u3040-\u309F\u30A0-\u30FF\u4E00-\u9FFF\u3400-\u4DBF\u3005"
-        # ↓ 半角アルファベット（大文字と小文字）
-        + r"\u0041-\u005A\u0061-\u007A"
-        # ↓ 全角アルファベット（大文字と小文字）
-        + r"\uFF21-\uFF3A\uFF41-\uFF5A"
-        # ↓ ギリシャ文字
-        + r"\u0370-\u03FF\u1F00-\u1FFF"
-        # ↓ "!", "?", "…", ",", ".", "'", "-", 但し`…`はすでに`...`に変換されている
-        + "".join(PUNCTUATIONS) + r"]+",
-        # 上述以外の文字を削除
-        "",
-        replaced_text,
-    )
+    # 上述以外の文字を削除
+    replaced_text = __PUNCTUATION_CLEANUP_PATTERN.sub("", replaced_text)
 
     return replaced_text
 
 
 def __convert_numbers_to_words(text: str) -> str:
     """
     記号や数字を日本語の文字表現に変換する。
@@ -146,17 +153,12 @@
     Args:
         text (str): 変換するテキスト
 
     Returns:
         str: 変換されたテキスト
     """
 
-    NUMBER_WITH_SEPARATOR_PATTERN = re.compile("[0-9]{1,3}(,[0-9]{3})+")
-    CURRENCY_MAP = {"$": "ドル", "¥": "円", "£": "ポンド", "€": "ユーロ"}
-    CURRENCY_PATTERN = re.compile(r"([$¥£€])([0-9.]*[0-9])")
-    NUMBER_PATTERN = re.compile(r"[0-9]+(\.[0-9]+)?")
-
-    res = NUMBER_WITH_SEPARATOR_PATTERN.sub(lambda m: m[0].replace(",", ""), text)
-    res = CURRENCY_PATTERN.sub(lambda m: m[2] + CURRENCY_MAP.get(m[1], m[1]), res)
-    res = NUMBER_PATTERN.sub(lambda m: num2words(m[0], lang="ja"), res)
+    res = __NUMBER_WITH_SEPARATOR_PATTERN.sub(lambda m: m[0].replace(",", ""), text)
+    res = __CURRENCY_PATTERN.sub(lambda m: m[2] + __CURRENCY_MAP.get(m[1], m[1]), res)
+    res = __NUMBER_PATTERN.sub(lambda m: num2words(m[0], lang="ja"), res)
 
     return res
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__init__.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     global WORKER_CLIENT
     if WORKER_CLIENT:
         return
 
     client = None
     try:
         client = WorkerClient(port)
-    except (socket.timeout, socket.error):
+    except (OSError, socket.timeout):
         logger.debug("try starting pyopenjtalk worker server")
         import os
         import subprocess
 
         worker_pkg_path = os.path.relpath(
             os.path.dirname(__file__), os.getcwd()
         ).replace(os.sep, ".")
@@ -116,15 +116,15 @@
 
         # wait until server listening
         count = 0
         while True:
             try:
                 client = WorkerClient(port)
                 break
-            except socket.error:
+            except OSError:
                 time.sleep(0.5)
                 count += 1
                 # 20: max number of retries
                 if count == 20:
                     raise TimeoutError("サーバーに接続できませんでした")
 
     logger.debug("pyopenjtalk worker server started")
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_client.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_client.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_common.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_common.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_server.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/pyopenjtalk_worker/worker_server.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/README.md` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/README.md`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/__init__.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/__init__.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/part_of_speech_data.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/part_of_speech_data.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/nlp/japanese/user_dict/word_model.py` & `style_bert_vits2-2.5.0/style_bert_vits2/nlp/japanese/user_dict/word_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     """
 
     part_of_speech: str = Field(title="品詞")
     part_of_speech_detail_1: str = Field(title="品詞細分類1")
     part_of_speech_detail_2: str = Field(title="品詞細分類2")
     part_of_speech_detail_3: str = Field(title="品詞細分類3")
     # context_idは辞書の左・右文脈IDのこと
-    # https://github.com/VOICEVOX/open_jtalk/blob/427cfd761b78efb6094bea3c5bb8c968f0d711ab/src/mecab-naist-jdic/_left-id.def # noqa
+    # https://github.com/VOICEVOX/open_jtalk/blob/427cfd761b78efb6094bea3c5bb8c968f0d711ab/src/mecab-naist-jdic/_left-id.def
     context_id: int = Field(title="文脈ID")
     cost_candidates: List[int] = Field(title="コストのパーセンタイル")
     accent_associative_rules: List[str] = Field(title="アクセント結合規則の一覧")
 
 
 class WordTypes(str, Enum):
     """
```

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/utils/stdout_wrapper.py` & `style_bert_vits2-2.5.0/style_bert_vits2/utils/stdout_wrapper.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/utils/strenum.py` & `style_bert_vits2-2.5.0/style_bert_vits2/utils/strenum.py`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/style_bert_vits2/utils/subprocess.py` & `style_bert_vits2-2.5.0/style_bert_vits2/utils/subprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     logger.info(f"Running: {' '.join(cmd)}")
     result = subprocess.run(
         [sys.executable] + cmd,
         stdout=SAFE_STDOUT,
         stderr=subprocess.PIPE,
         text=True,
         encoding="utf-8",
+        check=False,
     )
     if result.returncode != 0:
         logger.error(f"Error: {' '.join(cmd)}\n{result.stderr}")
         return False, result.stderr
     elif result.stderr and not ignore_warning:
         logger.warning(f"Warning: {' '.join(cmd)}\n{result.stderr}")
         return True, result.stderr
```

### Comparing `style_bert_vits2-2.4.dev0/tests/test_main.py` & `style_bert_vits2-2.5.0/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,9 +47,10 @@
         pytest.skip("音声合成モデルが見つかりませんでした。")
 
 
 def test_synthesize_cpu():
     synthesize(device="cpu")
 
 
-def test_synthesize_cuda():
-    synthesize(device="cuda")
+# Windows環境ではtorchのcudaが簡単に入らないため、テストをスキップ
+# def test_synthesize_cuda():
+#     synthesize(device="cuda")
```

### Comparing `style_bert_vits2-2.4.dev0/dict_data/default.csv` & `style_bert_vits2-2.5.0/dict_data/default.csv`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/LICENSE` & `style_bert_vits2-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `style_bert_vits2-2.4.dev0/README.md` & `style_bert_vits2-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # Style-Bert-VITS2
 
+**利用の際は必ず[利用規約](/docs/TERMS_OF_USE.md)をお読みください。**
+
 Bert-VITS2 with more controllable voice styles.
 
 https://github.com/litagin02/Style-Bert-VITS2/assets/139731664/e853f9a2-db4a-4202-a1dd-56ded3c562a0
 
+You can install via `pip install style-bert-vits2` (inference only), see [library.ipynb](/library.ipynb) for example usage.
+
 - **解説チュートリアル動画** [YouTube](https://youtu.be/aTUSzgDl1iY)　[ニコニコ動画](https://www.nicovideo.jp/watch/sm43391524)
-- [English README](docs/README_en.md)
 - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/litagin02/Style-Bert-VITS2/blob/master/colab.ipynb)
+- [FAQ](/docs/FAQ.md)
 - [🤗 オンラインデモはこちらから](https://huggingface.co/spaces/litagin/Style-Bert-VITS2-Editor-Demo)
 - [Zennの解説記事](https://zenn.dev/litagin/articles/034819a5256ff4)
 
 - [**リリースページ**](https://github.com/litagin02/Style-Bert-VITS2/releases/)、[更新履歴](/docs/CHANGELOG.md)
-
+  - 2024-06-01: Ver 2.5.0 (**[利用規約](/docs/TERMS_OF_USE.md)の追加**、フォルダ分けからのスタイル生成、小春音アミ・あみたろモデルの追加、インストールの高速化等)
+  - 2024-03-16: ver 2.4.1 (**batファイルによるインストール方法の変更**)
+  - 2024-03-15: ver 2.4.0 (大規模リファクタリングや種々の改良、ライブラリ化)
   - 2024-02-26: ver 2.3 (辞書機能とエディター機能)
   - 2024-02-09: ver 2.2
   - 2024-02-07: ver 2.1
   - 2024-02-03: ver 2.0 (JP-Extra)
   - 2024-01-09: ver 1.3
   - 2023-12-31: ver 1.2
   - 2023-12-29: ver 1.1
@@ -24,51 +30,59 @@
 This repository is based on [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2) v2.1 and Japanese-Extra, so many thanks to the original author!
 
 **概要**
 
 - 入力されたテキストの内容をもとに感情豊かな音声を生成する[Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)のv2.1とJapanese-Extraを元に、感情や発話スタイルを強弱込みで自由に制御できるようにしたものです。
 - GitやPythonがない人でも（Windowsユーザーなら）簡単にインストールでき、学習もできます (多くを[EasyBertVits2](https://github.com/Zuntan03/EasyBertVits2/)からお借りしました)。またGoogle Colabでの学習もサポートしています: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/litagin02/Style-Bert-VITS2/blob/master/colab.ipynb)
 - 音声合成のみに使う場合は、グラボがなくてもCPUで動作します。
+- 音声合成のみに使う場合、Pythonライブラリとして`pip install style-bert-vits2`でインストールできます。例は[library.ipynb](/library.ipynb)を参照してください。
 - 他との連携に使えるAPIサーバーも同梱しています ([@darai0512](https://github.com/darai0512) 様によるPRです、ありがとうございます)。
 - 元々「楽しそうな文章は楽しそうに、悲しそうな文章は悲しそうに」読むのがBert-VITS2の強みですので、スタイル指定がデフォルトでも感情豊かな音声を生成することができます。
 
 
 ## 使い方
 
-CLIでの使い方は[こちら](/docs/CLI.md)を参照してください。
+- CLIでの使い方は[こちら](/docs/CLI.md)を参照してください。
+- [よくある質問](/docs/FAQ.md)も参照してください。
 
 ### 動作環境
 
 各UIとAPI Serverにおいて、Windows コマンドプロンプト・WSL2・Linux(Ubuntu Desktop)での動作を確認しています(WSLでのパス指定は相対パスなど工夫ください)。NVidiaのGPUが無い場合は学習はできませんが音声合成とマージは可能です。
 
 ### インストール
 
+Pythonライブラリとしてのpipでのインストールや使用例は[library.ipynb](/library.ipynb)を参照してください。
+
 #### GitやPythonに馴染みが無い方
 
 Windowsを前提としています。
 
-1. [このzipファイル](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.3/Style-Bert-VITS2.zip)を**パスに日本語や空白が含まれない場所に**ダウンロードして展開します。
+1. [このzipファイル](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.5.0/sbv2.zip)を**パスに日本語や空白が含まれない場所に**ダウンロードして展開します。
   - グラボがある方は、`Install-Style-Bert-VITS2.bat`をダブルクリックします。
   - グラボがない方は、`Install-Style-Bert-VITS2-CPU.bat`をダブルクリックします。CPU版では学習はできませんが、音声合成とマージは可能です。
 2. 待つと自動で必要な環境がインストールされます。
 3. その後、自動的に音声合成するためのエディターが起動したらインストール成功です。デフォルトのモデルがダウンロードされるているので、そのまま遊ぶことができます。
 
-またアップデートをしたい場合は、`Update-Style-Bert-VITS2.bat`をダブルクリックしてください。ただし以下の場合は、専用のアップデートbatファイルを`Style-Bert-VITS2`フォルダがあるフォルダ（`Update-Style-Bert-VITS2.bat`等があるフォルダ）へ保存してからダブルクリックしてください。
-- **2.3以前**から**2.3以上**（辞書・エディター付き）へアップデート: [Update-to-Dict-Editor.bat](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.3/Update-to-Dict-Editor.bat)
+またアップデートをしたい場合は、`Update-Style-Bert-VITS2.bat`をダブルクリックしてください。
+
+ただし2024-03-16の**2.4.1**バージョン未満からのアップデートの場合は、全てを削除してから再びインストールする必要があります。申し訳ありません。移行方法は[CHANGELOG.md](/docs/CHANGELOG.md)を参照してください。
 
 #### GitやPython使える人
 
+Pythonの仮想環境・パッケージ管理ツールである[uv](https://github.com/astral-sh/uv)がpipより高速なので、それを使ってインストールすることをお勧めします。
+（使いたくない場合は通常のpipでも大丈夫です。）
+
 ```bash
+powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
 git clone https://github.com/litagin02/Style-Bert-VITS2.git
 cd Style-Bert-VITS2
-python -m venv venv
+uv venv venv
+uv pip install torch torchaudio --index-url https://download.pytorch.org/whl/cu118
+uv pip install -r requirements.txt
 venv\Scripts\activate
-# PyTorch 2.2.x系は今のところは学習エラーが出るので前のバージョンを使う
-pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118
-pip install -r requirements.txt
 python initialize.py  # 必要なモデルとデフォルトTTSモデルをダウンロード
 ```
 最後を忘れずに。
 
 ### 音声合成
 
 音声合成エディターは`Editor.bat`をダブルクリックか、`python server_editor.py --inbrowser`すると起動します（`--device cpu`でCPUモードで起動）。画面内で各セリフごとに設定を変えて原稿を作ったり、保存や読み込みや辞書の編集等ができます。
@@ -103,31 +117,27 @@
 学習には2-14秒程度の音声ファイルが複数と、それらの書き起こしデータが必要です。
 
 - 既存コーパスなどですでに分割された音声ファイルと書き起こしデータがある場合はそのまま（必要に応じて書き起こしファイルを修正して）使えます。下の「学習WebUI」を参照してください。
 - そうでない場合、（長さは問わない）音声ファイルのみがあれば、そこから学習にすぐに使えるようにデータセットを作るためのツールを同梱しています。
 
 #### データセット作り
 
-- `Dataset.bat`をダブルクリックか`python webui_dataset.py`すると、音声ファイルからデータセットを作るためのWebUIが起動します（音声ファイルを適切な長さにスライスし、その後に文字の書き起こしを自動で行います）。
-- 指示に従った後、閉じて下の「学習WebUI」でそのまま学習を行うことができます。
-
-注意: データセットの手動修正やノイズ除去等、細かい修正を行いたい場合は[Aivis](https://github.com/tsukumijima/Aivis)や、そのデータセット部分のWindows対応版 [Aivis Dataset](https://github.com/litagin02/Aivis-Dataset) を使うといいかもしれません。ですがファイル数が多い場合などは、このツールで簡易的に切り出してデータセットを作るだけでも十分という気もしています。
-
-データセットがどのようなものがいいかは各自試行錯誤中してください。
+- `App.bat`をダブルクリックか`python app.py`したところの「データセット作成」タブから、音声ファイルを適切な長さにスライスし、その後に文字の書き起こしを自動で行えます。
+- 指示に従った後、下の「学習」タブでそのまま学習を行うことができます。
 
 #### 学習WebUI
 
-- `Train.bat`をダブルクリックか`python webui_train.py`するとWebUIが起動するので指示に従ってください。
+- `App.bat`をダブルクリックか`python app.py`して開くWebUIの「学習」タブから指示に従ってください。
 
 ### スタイルの生成
 
-- デフォルトスタイル「Neutral」以外のスタイルを使いたい人向けです。
-- `Style.bat`をダブルクリックか`python webui_style_vectors.py`するとWebUIが起動します。
+- デフォルトでは、デフォルトスタイル「Neutral」の他、学習フォルダのフォルダ分けに応じたスタイルが生成されます。
+- それ以外の方法で手動でスタイルを作成したい人向けです。
+- `App.bat`をダブルクリックか`python app.py`して開くWebUIの「スタイル作成」タブから、音声ファイルを使ってスタイルを生成できます。
 - 学習とは独立しているので、学習中でもできるし、学習が終わっても何度もやりなおせます（前処理は終わらせている必要があります）。
-- スタイルについての仕様の詳細は[clustering.ipynb](clustering.ipynb)を参照してください。
 
 ### API Server
 
 構築した環境下で`python server_fastapi.py`するとAPIサーバーが起動します。
 API仕様は起動後に`/docs`にて確認ください。
 
 - 入力文字数はデフォルトで100文字が上限となっています。これは`config.yml`の`server.limit`で変更できます。
@@ -136,15 +146,15 @@
 また音声合成エディターのAPIサーバーは`python server_editor.py`で起動します。があまりまだ整備をしていません。[エディターのリポジトリ](https://github.com/litagin02/Style-Bert-VITS2-Editor)から必要な最低限のAPIしか現在は実装していません。
 
 音声合成エディターのウェブデプロイについては[このDockerfile](Dockerfile.deploy)を参考にしてください。
 
 ### マージ
 
 2つのモデルを、「声質」「声の高さ」「感情表現」「テンポ」の4点で混ぜ合わせて、新しいモデルを作ることが出来ます。
-`Merge.bat`をダブルクリックか`python webui_merge.py`するとWebUIが起動します。
+`App.bat`をダブルクリックか`python app.py`して開くWebUIの「マージ」タブから、2つのモデルを選択してマージすることができます。
 
 ### 自然性評価
 
 学習結果のうちどのステップ数がいいかの「一つの」指標として、[SpeechMOS](https://github.com/tarepan/SpeechMOS) を使うスクリプトを用意しています:
 ```bash
 python speech_mos.py -m <model_name>
 ```
@@ -161,32 +171,25 @@
 - 感情埋め込みもベクトル量子化を取り払い、単なる全結合層に。
 - スタイルベクトルファイル`style_vectors.npy`を作ることで、そのスタイルを使って効果の強さも連続的に指定しつつ音声を生成することができる。
 - 各種WebUIを作成
 - bf16での学習のサポート
 - safetensors形式のサポート、デフォルトでsafetensorsを使用するように
 - その他軽微なbugfixやリファクタリング
 
-## TODO
-- [x] デフォルトのJVNVモデルにJP-Extra版のものを追加
-- [x] LinuxやWSL等、Windowsの通常環境以外でのサポート ← おそらく問題ないとの報告あり
-- [x] 複数話者学習での音声合成対応（学習は現在でも可能）
-- [x] `server_fastapi.py`の対応、とくにAPIで使えるようになると嬉しい人が増えるのかもしれない
-- [x] モデルのマージで声音と感情表現を混ぜる機能の実装
-- [ ] 英語等多言語対応？
 
 ## References
 In addition to the original reference (written below), I used the following repositories:
 - [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)
 - [EasyBertVits2](https://github.com/Zuntan03/EasyBertVits2)
 
 [The pretrained model](https://huggingface.co/litagin/Style-Bert-VITS2-1.0-base) and [JP-Extra version](https://huggingface.co/litagin/Style-Bert-VITS2-2.0-base-JP-Extra) is essentially taken from [the original base model of Bert-VITS2 v2.1](https://huggingface.co/Garydesu/bert-vits2_base_model-2.1) and [JP-Extra pretrained model of Bert-VITS2](https://huggingface.co/Stardust-minus/Bert-VITS2-Japanese-Extra), so all the credits go to the original author ([Fish Audio](https://github.com/fishaudio)):
 
 
 In addition, [text/user_dict/](text/user_dict) module is based on the following repositories:
-- [voicevox_engine](https://github.com/VOICEVOX/voicevox_engine)]
+- [voicevox_engine](https://github.com/VOICEVOX/voicevox_engine)
 and the license of this module is LGPL v3.
 
 ## LICENSE
 
 This repository is licensed under the GNU Affero General Public License v3.0, the same as the original Bert-VITS2 repository. For more details, see [LICENSE](LICENSE).
 
 In addition, [text/user_dict/](text/user_dict) module is licensed under the GNU Lesser General Public License v3.0, inherited from the original VOICEVOX engine repository. For more details, see [LGPL_LICENSE](LGPL_LICENSE).
```

### Comparing `style_bert_vits2-2.4.dev0/pyproject.toml` & `style_bert_vits2-2.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "style-bert-vits2"
 dynamic = ["version"]
-description = 'Style-Bert-VITS2: Bert-VITS2 with more controllable voice styles.'
+description = "Style-Bert-VITS2: Bert-VITS2 with more controllable voice styles."
 readme = "README.md"
 requires-python = ">=3.9"
 license = "AGPL-3.0"
 keywords = []
 authors = [
     { name = "litagin02", email = "139731664+litagin02@users.noreply.github.com" },
 ]
@@ -18,33 +18,29 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-    'cmudict',
-    'cn2an',
-    'g2p_en',
-    'gradio',
-    'jieba',
-    'librosa==0.9.2',
-    'loguru',
-    'num2words',
-    'numba',
-    'numpy',
-    'pyannote.audio>=3.1.0',
-    'pydantic>=2.0',
-    'pyopenjtalk-dict',
-    'pypinyin',
-    'pyworld-prebuilt',
-    'safetensors',
-    'scipy',
-    'torch>=2.1,<2.2',
-    'transformers',
+    "cmudict",
+    "cn2an",
+    "g2p_en",
+    "jieba",
+    "loguru",
+    "num2words",
+    "numba",
+    "numpy",
+    "pydantic>=2.0",
+    "pyopenjtalk-dict",
+    "pypinyin",
+    "pyworld-prebuilt",
+    "safetensors",
+    "torch>=2.1",
+    "transformers",
 ]
 
 [project.urls]
 Documentation = "https://github.com/litagin02/Style-Bert-VITS2#readme"
 Issues = "https://github.com/litagin02/Style-Bert-VITS2/issues"
 Source = "https://github.com/litagin02/Style-Bert-VITS2"
 
@@ -59,75 +55,59 @@
     "style_bert_vits2",
     "tests",
     "LGPL_LICENSE",
     "LICENSE",
     "pyproject.toml",
     "README.md",
 ]
-exclude = [
-    ".git",
-    ".gitignore",
-    ".gitattributes",
-]
+exclude = [".git", ".gitignore", ".gitattributes"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["style_bert_vits2"]
 
 [tool.hatch.envs.test]
-dependencies = [
-    "coverage[toml]>=6.5",
-    "pytest",
-]
+dependencies = ["coverage[toml]>=6.5", "pytest"]
 [tool.hatch.envs.test.scripts]
 # Usage: `hatch run test:test`
 test = "pytest {args:tests}"
 # Usage: `hatch run test:coverage`
 test-cov = "coverage run -m pytest {args:tests}"
 # Usage: `hatch run test:cov-report`
-cov-report = [
-    "- coverage combine",
-    "coverage report",
-]
+cov-report = ["- coverage combine", "coverage report"]
 # Usage: `hatch run test:cov`
-cov = [
-    "test-cov",
-    "cov-report",
-]
+cov = ["test-cov", "cov-report"]
 
 [tool.hatch.envs.style]
 detached = true
-dependencies = [
-    "black",
-    "isort",
-]
+dependencies = ["black[jupyter]", "isort"]
 [tool.hatch.envs.style.scripts]
 check = [
     "black --check --diff .",
-    "isort --check-only --diff --profile black --gitignore --lai 2 .",
+    "isort --check-only --diff --profile black --gitignore --lai 2 . --sg \"Data/*\" --sg \"inputs/*\" --sg \"model_assets/*\" --sg \"static/*\"",
 ]
 fmt = [
     "black .",
-    "isort --profile black --gitignore --lai 2 .",
+    "isort --profile black --gitignore --lai 2 . --sg \"Data/*\" --sg \"inputs/*\" --sg \"model_assets/*\" --sg \"static/*\"",
     "check",
 ]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.9", "3.10", "3.11"]
 
 [tool.coverage.run]
 source_pkgs = ["style_bert_vits2", "tests"]
 branch = true
 parallel = true
-omit = [
-    "style_bert_vits2/constants.py",
-]
+omit = ["style_bert_vits2/constants.py"]
 
 [tool.coverage.paths]
 style_bert_vits2 = ["style_bert_vits2", "*/style-bert-vits2/style_bert_vits2"]
 tests = ["tests", "*/style-bert-vits2/tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-    "no cov",
-    "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:",
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+
+[tool.ruff]
+extend-select = ["I"]
+
+[tool.ruff.lint.isort]
+lines-after-imports = 2
```

### Comparing `style_bert_vits2-2.4.dev0/PKG-INFO` & `style_bert_vits2-2.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: style-bert-vits2
-Version: 2.4.dev0
+Version: 2.5.0
 Summary: Style-Bert-VITS2: Bert-VITS2 with more controllable voice styles.
 Project-URL: Documentation, https://github.com/litagin02/Style-Bert-VITS2#readme
 Project-URL: Issues, https://github.com/litagin02/Style-Bert-VITS2/issues
 Project-URL: Source, https://github.com/litagin02/Style-Bert-VITS2
 Author-email: litagin02 <139731664+litagin02@users.noreply.github.com>
 License-Expression: AGPL-3.0
 License-File: LICENSE
@@ -14,46 +14,48 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Requires-Dist: cmudict
 Requires-Dist: cn2an
 Requires-Dist: g2p-en
-Requires-Dist: gradio
 Requires-Dist: jieba
-Requires-Dist: librosa==0.9.2
 Requires-Dist: loguru
 Requires-Dist: num2words
 Requires-Dist: numba
 Requires-Dist: numpy
-Requires-Dist: pyannote-audio>=3.1.0
 Requires-Dist: pydantic>=2.0
 Requires-Dist: pyopenjtalk-dict
 Requires-Dist: pypinyin
 Requires-Dist: pyworld-prebuilt
 Requires-Dist: safetensors
-Requires-Dist: scipy
-Requires-Dist: torch<2.2,>=2.1
+Requires-Dist: torch>=2.1
 Requires-Dist: transformers
 Description-Content-Type: text/markdown
 
 # Style-Bert-VITS2
 
+**利用の際は必ず[利用規約](/docs/TERMS_OF_USE.md)をお読みください。**
+
 Bert-VITS2 with more controllable voice styles.
 
 https://github.com/litagin02/Style-Bert-VITS2/assets/139731664/e853f9a2-db4a-4202-a1dd-56ded3c562a0
 
+You can install via `pip install style-bert-vits2` (inference only), see [library.ipynb](/library.ipynb) for example usage.
+
 - **解説チュートリアル動画** [YouTube](https://youtu.be/aTUSzgDl1iY)　[ニコニコ動画](https://www.nicovideo.jp/watch/sm43391524)
-- [English README](docs/README_en.md)
 - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/litagin02/Style-Bert-VITS2/blob/master/colab.ipynb)
+- [FAQ](/docs/FAQ.md)
 - [🤗 オンラインデモはこちらから](https://huggingface.co/spaces/litagin/Style-Bert-VITS2-Editor-Demo)
 - [Zennの解説記事](https://zenn.dev/litagin/articles/034819a5256ff4)
 
 - [**リリースページ**](https://github.com/litagin02/Style-Bert-VITS2/releases/)、[更新履歴](/docs/CHANGELOG.md)
-
+  - 2024-06-01: Ver 2.5.0 (**[利用規約](/docs/TERMS_OF_USE.md)の追加**、フォルダ分けからのスタイル生成、小春音アミ・あみたろモデルの追加、インストールの高速化等)
+  - 2024-03-16: ver 2.4.1 (**batファイルによるインストール方法の変更**)
+  - 2024-03-15: ver 2.4.0 (大規模リファクタリングや種々の改良、ライブラリ化)
   - 2024-02-26: ver 2.3 (辞書機能とエディター機能)
   - 2024-02-09: ver 2.2
   - 2024-02-07: ver 2.1
   - 2024-02-03: ver 2.0 (JP-Extra)
   - 2024-01-09: ver 1.3
   - 2023-12-31: ver 1.2
   - 2023-12-29: ver 1.1
@@ -62,51 +64,59 @@
 This repository is based on [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2) v2.1 and Japanese-Extra, so many thanks to the original author!
 
 **概要**
 
 - 入力されたテキストの内容をもとに感情豊かな音声を生成する[Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)のv2.1とJapanese-Extraを元に、感情や発話スタイルを強弱込みで自由に制御できるようにしたものです。
 - GitやPythonがない人でも（Windowsユーザーなら）簡単にインストールでき、学習もできます (多くを[EasyBertVits2](https://github.com/Zuntan03/EasyBertVits2/)からお借りしました)。またGoogle Colabでの学習もサポートしています: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/litagin02/Style-Bert-VITS2/blob/master/colab.ipynb)
 - 音声合成のみに使う場合は、グラボがなくてもCPUで動作します。
+- 音声合成のみに使う場合、Pythonライブラリとして`pip install style-bert-vits2`でインストールできます。例は[library.ipynb](/library.ipynb)を参照してください。
 - 他との連携に使えるAPIサーバーも同梱しています ([@darai0512](https://github.com/darai0512) 様によるPRです、ありがとうございます)。
 - 元々「楽しそうな文章は楽しそうに、悲しそうな文章は悲しそうに」読むのがBert-VITS2の強みですので、スタイル指定がデフォルトでも感情豊かな音声を生成することができます。
 
 
 ## 使い方
 
-CLIでの使い方は[こちら](/docs/CLI.md)を参照してください。
+- CLIでの使い方は[こちら](/docs/CLI.md)を参照してください。
+- [よくある質問](/docs/FAQ.md)も参照してください。
 
 ### 動作環境
 
 各UIとAPI Serverにおいて、Windows コマンドプロンプト・WSL2・Linux(Ubuntu Desktop)での動作を確認しています(WSLでのパス指定は相対パスなど工夫ください)。NVidiaのGPUが無い場合は学習はできませんが音声合成とマージは可能です。
 
 ### インストール
 
+Pythonライブラリとしてのpipでのインストールや使用例は[library.ipynb](/library.ipynb)を参照してください。
+
 #### GitやPythonに馴染みが無い方
 
 Windowsを前提としています。
 
-1. [このzipファイル](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.3/Style-Bert-VITS2.zip)を**パスに日本語や空白が含まれない場所に**ダウンロードして展開します。
+1. [このzipファイル](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.5.0/sbv2.zip)を**パスに日本語や空白が含まれない場所に**ダウンロードして展開します。
   - グラボがある方は、`Install-Style-Bert-VITS2.bat`をダブルクリックします。
   - グラボがない方は、`Install-Style-Bert-VITS2-CPU.bat`をダブルクリックします。CPU版では学習はできませんが、音声合成とマージは可能です。
 2. 待つと自動で必要な環境がインストールされます。
 3. その後、自動的に音声合成するためのエディターが起動したらインストール成功です。デフォルトのモデルがダウンロードされるているので、そのまま遊ぶことができます。
 
-またアップデートをしたい場合は、`Update-Style-Bert-VITS2.bat`をダブルクリックしてください。ただし以下の場合は、専用のアップデートbatファイルを`Style-Bert-VITS2`フォルダがあるフォルダ（`Update-Style-Bert-VITS2.bat`等があるフォルダ）へ保存してからダブルクリックしてください。
-- **2.3以前**から**2.3以上**（辞書・エディター付き）へアップデート: [Update-to-Dict-Editor.bat](https://github.com/litagin02/Style-Bert-VITS2/releases/download/2.3/Update-to-Dict-Editor.bat)
+またアップデートをしたい場合は、`Update-Style-Bert-VITS2.bat`をダブルクリックしてください。
+
+ただし2024-03-16の**2.4.1**バージョン未満からのアップデートの場合は、全てを削除してから再びインストールする必要があります。申し訳ありません。移行方法は[CHANGELOG.md](/docs/CHANGELOG.md)を参照してください。
 
 #### GitやPython使える人
 
+Pythonの仮想環境・パッケージ管理ツールである[uv](https://github.com/astral-sh/uv)がpipより高速なので、それを使ってインストールすることをお勧めします。
+（使いたくない場合は通常のpipでも大丈夫です。）
+
 ```bash
+powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
 git clone https://github.com/litagin02/Style-Bert-VITS2.git
 cd Style-Bert-VITS2
-python -m venv venv
+uv venv venv
+uv pip install torch torchaudio --index-url https://download.pytorch.org/whl/cu118
+uv pip install -r requirements.txt
 venv\Scripts\activate
-# PyTorch 2.2.x系は今のところは学習エラーが出るので前のバージョンを使う
-pip install torch==2.1.2 torchvision==0.16.2 torchaudio==2.1.2 --index-url https://download.pytorch.org/whl/cu118
-pip install -r requirements.txt
 python initialize.py  # 必要なモデルとデフォルトTTSモデルをダウンロード
 ```
 最後を忘れずに。
 
 ### 音声合成
 
 音声合成エディターは`Editor.bat`をダブルクリックか、`python server_editor.py --inbrowser`すると起動します（`--device cpu`でCPUモードで起動）。画面内で各セリフごとに設定を変えて原稿を作ったり、保存や読み込みや辞書の編集等ができます。
@@ -141,31 +151,27 @@
 学習には2-14秒程度の音声ファイルが複数と、それらの書き起こしデータが必要です。
 
 - 既存コーパスなどですでに分割された音声ファイルと書き起こしデータがある場合はそのまま（必要に応じて書き起こしファイルを修正して）使えます。下の「学習WebUI」を参照してください。
 - そうでない場合、（長さは問わない）音声ファイルのみがあれば、そこから学習にすぐに使えるようにデータセットを作るためのツールを同梱しています。
 
 #### データセット作り
 
-- `Dataset.bat`をダブルクリックか`python webui_dataset.py`すると、音声ファイルからデータセットを作るためのWebUIが起動します（音声ファイルを適切な長さにスライスし、その後に文字の書き起こしを自動で行います）。
-- 指示に従った後、閉じて下の「学習WebUI」でそのまま学習を行うことができます。
-
-注意: データセットの手動修正やノイズ除去等、細かい修正を行いたい場合は[Aivis](https://github.com/tsukumijima/Aivis)や、そのデータセット部分のWindows対応版 [Aivis Dataset](https://github.com/litagin02/Aivis-Dataset) を使うといいかもしれません。ですがファイル数が多い場合などは、このツールで簡易的に切り出してデータセットを作るだけでも十分という気もしています。
-
-データセットがどのようなものがいいかは各自試行錯誤中してください。
+- `App.bat`をダブルクリックか`python app.py`したところの「データセット作成」タブから、音声ファイルを適切な長さにスライスし、その後に文字の書き起こしを自動で行えます。
+- 指示に従った後、下の「学習」タブでそのまま学習を行うことができます。
 
 #### 学習WebUI
 
-- `Train.bat`をダブルクリックか`python webui_train.py`するとWebUIが起動するので指示に従ってください。
+- `App.bat`をダブルクリックか`python app.py`して開くWebUIの「学習」タブから指示に従ってください。
 
 ### スタイルの生成
 
-- デフォルトスタイル「Neutral」以外のスタイルを使いたい人向けです。
-- `Style.bat`をダブルクリックか`python webui_style_vectors.py`するとWebUIが起動します。
+- デフォルトでは、デフォルトスタイル「Neutral」の他、学習フォルダのフォルダ分けに応じたスタイルが生成されます。
+- それ以外の方法で手動でスタイルを作成したい人向けです。
+- `App.bat`をダブルクリックか`python app.py`して開くWebUIの「スタイル作成」タブから、音声ファイルを使ってスタイルを生成できます。
 - 学習とは独立しているので、学習中でもできるし、学習が終わっても何度もやりなおせます（前処理は終わらせている必要があります）。
-- スタイルについての仕様の詳細は[clustering.ipynb](clustering.ipynb)を参照してください。
 
 ### API Server
 
 構築した環境下で`python server_fastapi.py`するとAPIサーバーが起動します。
 API仕様は起動後に`/docs`にて確認ください。
 
 - 入力文字数はデフォルトで100文字が上限となっています。これは`config.yml`の`server.limit`で変更できます。
@@ -174,15 +180,15 @@
 また音声合成エディターのAPIサーバーは`python server_editor.py`で起動します。があまりまだ整備をしていません。[エディターのリポジトリ](https://github.com/litagin02/Style-Bert-VITS2-Editor)から必要な最低限のAPIしか現在は実装していません。
 
 音声合成エディターのウェブデプロイについては[このDockerfile](Dockerfile.deploy)を参考にしてください。
 
 ### マージ
 
 2つのモデルを、「声質」「声の高さ」「感情表現」「テンポ」の4点で混ぜ合わせて、新しいモデルを作ることが出来ます。
-`Merge.bat`をダブルクリックか`python webui_merge.py`するとWebUIが起動します。
+`App.bat`をダブルクリックか`python app.py`して開くWebUIの「マージ」タブから、2つのモデルを選択してマージすることができます。
 
 ### 自然性評価
 
 学習結果のうちどのステップ数がいいかの「一つの」指標として、[SpeechMOS](https://github.com/tarepan/SpeechMOS) を使うスクリプトを用意しています:
 ```bash
 python speech_mos.py -m <model_name>
 ```
@@ -199,32 +205,25 @@
 - 感情埋め込みもベクトル量子化を取り払い、単なる全結合層に。
 - スタイルベクトルファイル`style_vectors.npy`を作ることで、そのスタイルを使って効果の強さも連続的に指定しつつ音声を生成することができる。
 - 各種WebUIを作成
 - bf16での学習のサポート
 - safetensors形式のサポート、デフォルトでsafetensorsを使用するように
 - その他軽微なbugfixやリファクタリング
 
-## TODO
-- [x] デフォルトのJVNVモデルにJP-Extra版のものを追加
-- [x] LinuxやWSL等、Windowsの通常環境以外でのサポート ← おそらく問題ないとの報告あり
-- [x] 複数話者学習での音声合成対応（学習は現在でも可能）
-- [x] `server_fastapi.py`の対応、とくにAPIで使えるようになると嬉しい人が増えるのかもしれない
-- [x] モデルのマージで声音と感情表現を混ぜる機能の実装
-- [ ] 英語等多言語対応？
 
 ## References
 In addition to the original reference (written below), I used the following repositories:
 - [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)
 - [EasyBertVits2](https://github.com/Zuntan03/EasyBertVits2)
 
 [The pretrained model](https://huggingface.co/litagin/Style-Bert-VITS2-1.0-base) and [JP-Extra version](https://huggingface.co/litagin/Style-Bert-VITS2-2.0-base-JP-Extra) is essentially taken from [the original base model of Bert-VITS2 v2.1](https://huggingface.co/Garydesu/bert-vits2_base_model-2.1) and [JP-Extra pretrained model of Bert-VITS2](https://huggingface.co/Stardust-minus/Bert-VITS2-Japanese-Extra), so all the credits go to the original author ([Fish Audio](https://github.com/fishaudio)):
 
 
 In addition, [text/user_dict/](text/user_dict) module is based on the following repositories:
-- [voicevox_engine](https://github.com/VOICEVOX/voicevox_engine)]
+- [voicevox_engine](https://github.com/VOICEVOX/voicevox_engine)
 and the license of this module is LGPL v3.
 
 ## LICENSE
 
 This repository is licensed under the GNU Affero General Public License v3.0, the same as the original Bert-VITS2 repository. For more details, see [LICENSE](LICENSE).
 
 In addition, [text/user_dict/](text/user_dict) module is licensed under the GNU Lesser General Public License v3.0, inherited from the original VOICEVOX engine repository. For more details, see [LGPL_LICENSE](LGPL_LICENSE).
```

