# Comparing `tmp/hezar-0.38.0.tar.gz` & `tmp/hezar-0.38.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.38.0.tar", max compression
+gzip compressed data, was "hezar-0.38.1.tar", max compression
```

## Comparing `hezar-0.38.0.tar` & `hezar-0.38.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0    11337 2024-06-01 08:04:44.624830 hezar-0.38.0/LICENSE
--rw-r--r--   0        0        0    14442 2024-06-01 08:04:44.624830 hezar-0.38.0/README.md
--rw-r--r--   0        0        0      623 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/__init__.py
--rw-r--r--   0        0        0     5651 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/builders.py
--rw-r--r--   0        0        0    18631 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/configs.py
--rw-r--r--   0        0        0     4752 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/constants.py
--rw-r--r--   0        0        0       83 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/__init__.py
--rw-r--r--   0        0        0    13756 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0     1031 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/data_samplers.py
--rw-r--r--   0        0        0      634 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     3760 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3727 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/image_captioning_dataset.py
--rw-r--r--   0        0        0     7384 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/ocr_dataset.py
--rw-r--r--   0        0        0     5923 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3079 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/speech_recognition_dataset.py
--rw-r--r--   0        0        0     4498 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     4820 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0      202 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0    11544 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     7171 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     7668 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      444 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     2285 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/accuracy.py
--rw-r--r--   0        0        0     2484 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/bleu.py
--rw-r--r--   0        0        0     3711 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/cer.py
--rw-r--r--   0        0        0     3209 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0     1302 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     3566 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/precision.py
--rw-r--r--   0        0        0     3509 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     3155 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/rouge.py
--rw-r--r--   0        0        0     4029 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0     2950 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/metrics/wer.py
--rw-r--r--   0        0        0      362 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/__init__.py
--rw-r--r--   0        0        0       88 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/__init__.py
--rw-r--r--   0        0        0       35 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/__init__.py
--rw-r--r--   0        0        0     2787 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/bert.py
--rw-r--r--   0        0        0      743 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/bert/bert_config.py
--rw-r--r--   0        0        0       53 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/__init__.py
--rw-r--r--   0        0        0     2288 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/distilbert.py
--rw-r--r--   0        0        0      618 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/distilbert/distilbert_config.py
--rw-r--r--   0        0        0       44 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/__init__.py
--rw-r--r--   0        0        0     2788 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/roberta.py
--rw-r--r--   0        0        0      812 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/roberta/roberta_config.py
--rw-r--r--   0        0        0       55 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/__init__.py
--rw-r--r--   0        0        0     2172 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/vit.py
--rw-r--r--   0        0        0      572 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/backbone/vit/vit_config.py
--rw-r--r--   0        0        0      120 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0      131 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/__init__.py
--rw-r--r--   0        0        0     3493 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
--rw-r--r--   0        0        0     2376 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
--rw-r--r--   0        0        0      101 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0     1106 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_decode_utils.py
--rw-r--r--   0        0        0     4649 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text.py
--rw-r--r--   0        0        0      478 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text_config.py
--rw-r--r--   0        0        0      105 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0     3430 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text.py
--rw-r--r--   0        0        0     1899 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text_config.py
--rw-r--r--   0        0        0      115 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/__init__.py
--rw-r--r--   0        0        0     3463 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
--rw-r--r--   0        0        0     1872 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
--rw-r--r--   0        0        0      127 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/__init__.py
--rw-r--r--   0        0        0     3864 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
--rw-r--r--   0        0        0     1952 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
--rw-r--r--   0        0        0       69 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/__init__.py
--rw-r--r--   0        0        0      107 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/__init__.py
--rw-r--r--   0        0        0     4320 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling.py
--rw-r--r--   0        0        0      771 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py
--rw-r--r--   0        0        0      131 2024-06-01 08:04:44.628830 hezar-0.38.0/hezar/models/mask_filling/distilbert/__init__.py
--rw-r--r--   0        0        0     3921 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
--rw-r--r--   0        0        0      637 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
--rw-r--r--   0        0        0      119 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/__init__.py
--rw-r--r--   0        0        0     4384 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py
--rw-r--r--   0        0        0      831 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
--rw-r--r--   0        0        0    20471 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/model.py
--rw-r--r--   0        0        0     2346 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/model_outputs.py
--rw-r--r--   0        0        0       69 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     5118 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      931 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     5172 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      872 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0      139 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/__init__.py
--rw-r--r--   0        0        0     5821 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
--rw-r--r--   0        0        0     1025 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
--rw-r--r--   0        0        0       23 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0      306 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/__init__.py
--rw-r--r--   0        0        0     7713 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
--rw-r--r--   0        0        0     7067 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
--rw-r--r--   0        0        0     2821 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
--rw-r--r--   0        0        0    27594 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
--rw-r--r--   0        0        0       69 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     4796 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      845 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     4357 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      748 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     4963 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      942 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_embedding/__init__.py
--rw-r--r--   0        0        0       38 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/__init__.py
--rw-r--r--   0        0        0      119 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/__init__.py
--rw-r--r--   0        0        0     3324 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py
--rw-r--r--   0        0        0     1148 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
--rw-r--r--   0        0        0      111 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/__init__.py
--rw-r--r--   0        0        0     4053 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation.py
--rw-r--r--   0        0        0      837 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation_config.py
--rw-r--r--   0        0        0      390 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0    13303 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/audio_feature_extractor.py
--rw-r--r--   0        0        0     8292 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/image_processor.py
--rw-r--r--   0        0        0     5043 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     4635 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      337 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     3973 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     4181 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4102 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    27637 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3537 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     6584 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/registry.py
--rw-r--r--   0        0        0      113 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/__init__.py
--rw-r--r--   0        0        0     7345 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/metrics_handlers.py
--rw-r--r--   0        0        0    32462 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/trainer.py
--rw-r--r--   0        0        0     5624 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/trainer/trainer_utils.py
--rw-r--r--   0        0        0      245 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0    23979 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/audio_utils.py
--rw-r--r--   0        0        0     3955 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     7678 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/data_utils.py
--rw-r--r--   0        0        0      976 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/file_utils.py
--rw-r--r--   0        0        0     4145 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0     7352 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/image_utils.py
--rw-r--r--   0        0        0     1376 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/integration_utils.py
--rw-r--r--   0        0        0      622 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/logging.py
--rw-r--r--   0        0        0     4498 2024-06-01 08:04:44.632830 hezar-0.38.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     2602 2024-06-01 08:04:44.632830 hezar-0.38.0/pyproject.toml
--rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.38.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-06-01 18:35:48.814479 hezar-0.38.1/LICENSE
+-rw-r--r--   0        0        0    14442 2024-06-01 18:35:48.814479 hezar-0.38.1/README.md
+-rw-r--r--   0        0        0      623 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/__init__.py
+-rw-r--r--   0        0        0     5651 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/builders.py
+-rw-r--r--   0        0        0    18631 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/configs.py
+-rw-r--r--   0        0        0     4752 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/constants.py
+-rw-r--r--   0        0        0       83 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0    13756 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0     1031 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/data_samplers.py
+-rw-r--r--   0        0        0      634 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     3760 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     3727 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/image_captioning_dataset.py
+-rw-r--r--   0        0        0     7384 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/ocr_dataset.py
+-rw-r--r--   0        0        0     5923 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3079 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/speech_recognition_dataset.py
+-rw-r--r--   0        0        0     4498 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     4820 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0      202 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0    11544 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     7171 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     7668 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      444 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     2285 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/accuracy.py
+-rw-r--r--   0        0        0     2484 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/bleu.py
+-rw-r--r--   0        0        0     3711 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/cer.py
+-rw-r--r--   0        0        0     3209 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/f1.py
+-rw-r--r--   0        0        0     1302 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     3566 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/precision.py
+-rw-r--r--   0        0        0     3509 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     3155 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/rouge.py
+-rw-r--r--   0        0        0     4029 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0     2950 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/metrics/wer.py
+-rw-r--r--   0        0        0      362 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/bert/__init__.py
+-rw-r--r--   0        0        0     2787 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/bert/bert.py
+-rw-r--r--   0        0        0      743 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/bert/bert_config.py
+-rw-r--r--   0        0        0       53 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/distilbert/__init__.py
+-rw-r--r--   0        0        0     2288 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/distilbert/distilbert.py
+-rw-r--r--   0        0        0      618 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/distilbert/distilbert_config.py
+-rw-r--r--   0        0        0       44 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/roberta/__init__.py
+-rw-r--r--   0        0        0     2788 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/roberta/roberta.py
+-rw-r--r--   0        0        0      812 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/roberta/roberta_config.py
+-rw-r--r--   0        0        0       55 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/vit/__init__.py
+-rw-r--r--   0        0        0     2172 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/vit/vit.py
+-rw-r--r--   0        0        0      572 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/backbone/vit/vit_config.py
+-rw-r--r--   0        0        0      120 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0      131 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/beit_roberta/__init__.py
+-rw-r--r--   0        0        0     3493 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py
+-rw-r--r--   0        0        0     2376 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py
+-rw-r--r--   0        0        0      101 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0     1106 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/crnn/crnn_decode_utils.py
+-rw-r--r--   0        0        0     4649 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/crnn/crnn_image2text.py
+-rw-r--r--   0        0        0      478 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/crnn/crnn_image2text_config.py
+-rw-r--r--   0        0        0      105 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0     3430 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/trocr/trocr_image2text.py
+-rw-r--r--   0        0        0     1899 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/trocr/trocr_image2text_config.py
+-rw-r--r--   0        0        0      115 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/vit_gpt2/__init__.py
+-rw-r--r--   0        0        0     3463 2024-06-01 18:35:48.818479 hezar-0.38.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py
+-rw-r--r--   0        0        0     1872 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py
+-rw-r--r--   0        0        0      127 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/image2text/vit_roberta/__init__.py
+-rw-r--r--   0        0        0     3864 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py
+-rw-r--r--   0        0        0     1952 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py
+-rw-r--r--   0        0        0       69 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/__init__.py
+-rw-r--r--   0        0        0      107 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/bert/__init__.py
+-rw-r--r--   0        0        0     4320 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/bert/bert_mask_filling.py
+-rw-r--r--   0        0        0      771 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py
+-rw-r--r--   0        0        0      131 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/distilbert/__init__.py
+-rw-r--r--   0        0        0     3921 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py
+-rw-r--r--   0        0        0      637 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py
+-rw-r--r--   0        0        0      119 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/roberta/__init__.py
+-rw-r--r--   0        0        0     4384 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py
+-rw-r--r--   0        0        0      831 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py
+-rw-r--r--   0        0        0    20471 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/model.py
+-rw-r--r--   0        0        0     2346 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0       69 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     5118 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      931 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     5172 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      872 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      139 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/roberta/__init__.py
+-rw-r--r--   0        0        0     5821 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py
+-rw-r--r--   0        0        0     1025 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py
+-rw-r--r--   0        0        0       23 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0      306 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/whisper/__init__.py
+-rw-r--r--   0        0        0     7713 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py
+-rw-r--r--   0        0        0     7067 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py
+-rw-r--r--   0        0        0     2821 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py
+-rw-r--r--   0        0        0    27594 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py
+-rw-r--r--   0        0        0       69 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     4796 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      845 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     4357 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      748 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      942 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_embedding/__init__.py
+-rw-r--r--   0        0        0       38 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/gpt2/__init__.py
+-rw-r--r--   0        0        0     3324 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py
+-rw-r--r--   0        0        0     1148 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py
+-rw-r--r--   0        0        0      111 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/t5/__init__.py
+-rw-r--r--   0        0        0     4053 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/t5/t5_text_generation.py
+-rw-r--r--   0        0        0      837 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/models/text_generation/t5/t5_text_generation_config.py
+-rw-r--r--   0        0        0      390 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0    13303 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/audio_feature_extractor.py
+-rw-r--r--   0        0        0     8292 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/image_processor.py
+-rw-r--r--   0        0        0     5043 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     4635 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      337 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     3973 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     4181 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4102 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    27637 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3537 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     6584 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/registry.py
+-rw-r--r--   0        0        0      113 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/trainer/__init__.py
+-rw-r--r--   0        0        0     7345 2024-06-01 18:35:48.822479 hezar-0.38.1/hezar/trainer/metrics_handlers.py
+-rw-r--r--   0        0        0    32579 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/trainer/trainer.py
+-rw-r--r--   0        0        0     5624 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/trainer/trainer_utils.py
+-rw-r--r--   0        0        0      245 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0    23979 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/audio_utils.py
+-rw-r--r--   0        0        0     3955 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     7678 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/data_utils.py
+-rw-r--r--   0        0        0      976 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/file_utils.py
+-rw-r--r--   0        0        0     4145 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0     7352 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/image_utils.py
+-rw-r--r--   0        0        0     1376 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/integration_utils.py
+-rw-r--r--   0        0        0      622 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0     4498 2024-06-01 18:35:48.826479 hezar-0.38.1/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     2602 2024-06-01 18:35:48.826479 hezar-0.38.1/pyproject.toml
+-rw-r--r--   0        0        0    17052 1970-01-01 00:00:00.000000 hezar-0.38.1/PKG-INFO
```

### Comparing `hezar-0.38.0/LICENSE` & `hezar-0.38.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/README.md` & `hezar-0.38.1/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/__init__.py` & `hezar-0.38.1/hezar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.38.0"
+__version__ = "0.38.1"
```

### Comparing `hezar-0.38.0/hezar/builders.py` & `hezar-0.38.1/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/configs.py` & `hezar-0.38.1/hezar/configs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/constants.py` & `hezar-0.38.1/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/data_collators.py` & `hezar-0.38.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/data_samplers.py` & `hezar-0.38.1/hezar/data/data_samplers.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/__init__.py` & `hezar-0.38.1/hezar/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/dataset.py` & `hezar-0.38.1/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/image_captioning_dataset.py` & `hezar-0.38.1/hezar/data/datasets/image_captioning_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/ocr_dataset.py` & `hezar-0.38.1/hezar/data/datasets/ocr_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.38.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/speech_recognition_dataset.py` & `hezar-0.38.1/hezar/data/datasets/speech_recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.38.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.38.1/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/embeddings/embedding.py` & `hezar-0.38.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/embeddings/fasttext.py` & `hezar-0.38.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/embeddings/word2vec.py` & `hezar-0.38.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/accuracy.py` & `hezar-0.38.1/hezar/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/bleu.py` & `hezar-0.38.1/hezar/metrics/bleu.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/cer.py` & `hezar-0.38.1/hezar/metrics/cer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/f1.py` & `hezar-0.38.1/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/metric.py` & `hezar-0.38.1/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/precision.py` & `hezar-0.38.1/hezar/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/recall.py` & `hezar-0.38.1/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/rouge.py` & `hezar-0.38.1/hezar/metrics/rouge.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/seqeval.py` & `hezar-0.38.1/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/metrics/wer.py` & `hezar-0.38.1/hezar/metrics/wer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/bert/bert.py` & `hezar-0.38.1/hezar/models/backbone/bert/bert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/bert/bert_config.py` & `hezar-0.38.1/hezar/models/backbone/bert/bert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/distilbert/distilbert.py` & `hezar-0.38.1/hezar/models/backbone/distilbert/distilbert.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/distilbert/distilbert_config.py` & `hezar-0.38.1/hezar/models/backbone/distilbert/distilbert_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/roberta/roberta.py` & `hezar-0.38.1/hezar/models/backbone/roberta/roberta.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/roberta/roberta_config.py` & `hezar-0.38.1/hezar/models/backbone/roberta/roberta_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/vit/vit.py` & `hezar-0.38.1/hezar/models/backbone/vit/vit.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/backbone/vit/vit_config.py` & `hezar-0.38.1/hezar/models/backbone/vit/vit_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py` & `hezar-0.38.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py` & `hezar-0.38.1/hezar/models/image2text/beit_roberta/beit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/crnn/crnn_decode_utils.py` & `hezar-0.38.1/hezar/models/image2text/crnn/crnn_decode_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/crnn/crnn_image2text.py` & `hezar-0.38.1/hezar/models/image2text/crnn/crnn_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text.py` & `hezar-0.38.1/hezar/models/image2text/trocr/trocr_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/trocr/trocr_image2text_config.py` & `hezar-0.38.1/hezar/models/image2text/trocr/trocr_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py` & `hezar-0.38.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py` & `hezar-0.38.1/hezar/models/image2text/vit_gpt2/vit_gpt2_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py` & `hezar-0.38.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py` & `hezar-0.38.1/hezar/models/image2text/vit_roberta/vit_roberta_image2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling.py` & `hezar-0.38.1/hezar/models/mask_filling/bert/bert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/bert/bert_mask_filling_config.py` & `hezar-0.38.1/hezar/models/mask_filling/bert/bert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py` & `hezar-0.38.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py` & `hezar-0.38.1/hezar/models/mask_filling/distilbert/distilbert_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling.py` & `hezar-0.38.1/hezar/models/mask_filling/roberta/roberta_mask_filling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py` & `hezar-0.38.1/hezar/models/mask_filling/roberta/roberta_mask_filling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/model.py` & `hezar-0.38.1/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/model_outputs.py` & `hezar-0.38.1/hezar/models/model_outputs.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.38.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.38.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.38.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.38.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py` & `hezar-0.38.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py` & `hezar-0.38.1/hezar/models/sequence_labeling/roberta/roberta_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py` & `hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py` & `hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py` & `hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_speech_recognition_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/speech_recognition/whisper/whisper_tokenizer.py` & `hezar-0.38.1/hezar/models/speech_recognition/whisper/whisper_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.38.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.38.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.38.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.38.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.38.1/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.38.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation.py` & `hezar-0.38.1/hezar/models/text_generation/gpt2/gpt2_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py` & `hezar-0.38.1/hezar/models/text_generation/gpt2/gpt2_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation.py` & `hezar-0.38.1/hezar/models/text_generation/t5/t5_text_generation.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/models/text_generation/t5/t5_text_generation_config.py` & `hezar-0.38.1/hezar/models/text_generation/t5/t5_text_generation_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/audio_feature_extractor.py` & `hezar-0.38.1/hezar/preprocessors/audio_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/image_processor.py` & `hezar-0.38.1/hezar/preprocessors/image_processor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/preprocessor.py` & `hezar-0.38.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/text_normalizer.py` & `hezar-0.38.1/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.38.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.38.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.38.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.38.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.38.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/registry.py` & `hezar-0.38.1/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/trainer/metrics_handlers.py` & `hezar-0.38.1/hezar/trainer/metrics_handlers.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/trainer/trainer.py` & `hezar-0.38.1/hezar/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,16 @@
                 metric_for_best_checkpoint=self.config.metric_for_best_model,
                 logs_dir=resolve_logdir(os.path.join(self.config.output_dir, self.config.logs_dir)),
             )
         return state
 
     def _resolve_checkpoint_path(self, checkpoint: str | bool):
         if isinstance(checkpoint, bool) and checkpoint:
-            checkpoint_path = os.path.join(self.checkpoints_dir, str(self.state.global_step))
+            checkpoint_name = str(self.state.global_step).zfill(len(str(self.total_steps)))
+            checkpoint_path = os.path.join(self.checkpoints_dir, checkpoint_name)
         elif os.path.isdir(checkpoint):
             checkpoint_path = checkpoint
         else:
             raise ValueError(f"Checkpoint `{checkpoint}` is either invalid or does not exist!")
 
         return checkpoint_path
 
@@ -318,15 +319,15 @@
             optimizer = optimizers[optimizer_type](
                 self.model.parameters(),
                 lr=self.config.learning_rate,
                 weight_decay=self.config.weight_decay,
             )
             if self.config.resume_from_checkpoint is not None:
                 checkpoint_path = self._resolve_checkpoint_path(self.config.resume_from_checkpoint)
-                optimizer_path = os.path.join(checkpoint_path, self.optimizer_file)
+                optimizer_path = os.path.join(checkpoint_path, self.trainer_subfolder, self.optimizer_file)
                 if os.path.isdir(checkpoint_path) and os.path.isfile(optimizer_path):
                     optimizer.load_state_dict(torch.load(optimizer_path))
 
             if lr_scheduler is None:
                 scheduler_name = self.config.lr_scheduler or self.default_lr_scheduler
                 scheduler_kwargs = self.config.lr_scheduler_kwargs or {}
                 if scheduler_name is None:
@@ -717,15 +718,15 @@
         config_filename = config_filename or self.trainer_config_file
         subfolder = subfolder or self.trainer_subfolder
         dataset_config_file = dataset_config_file or self.dataset_config_file
         optimizer_file = optimizer_file or self.optimizer_file
 
         self.config.save(path, filename=config_filename, subfolder=subfolder)
         self.model.save(path, filename=model_filename, config_filename=model_config_filename)
-        torch.save(self.optimizer, os.path.join(path, subfolder, optimizer_file))
+        torch.save(self.optimizer.state_dict(), os.path.join(path, subfolder, optimizer_file))
         if isinstance(self.train_dataset, Dataset):
             self.train_dataset.config.save(path, filename=dataset_config_file, subfolder=subfolder)
         else:
             self.logger.warning(
                 "The dataset passed to the Trainer is not a `hezar.data.Dataset` instance so that no dataset config"
                 " will be saved!"
             )
```

### Comparing `hezar-0.38.0/hezar/trainer/trainer_utils.py` & `hezar-0.38.1/hezar/trainer/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/audio_utils.py` & `hezar-0.38.1/hezar/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/common_utils.py` & `hezar-0.38.1/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/data_utils.py` & `hezar-0.38.1/hezar/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/file_utils.py` & `hezar-0.38.1/hezar/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/hub_utils.py` & `hezar-0.38.1/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/image_utils.py` & `hezar-0.38.1/hezar/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/integration_utils.py` & `hezar-0.38.1/hezar/utils/integration_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/logging.py` & `hezar-0.38.1/hezar/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/hezar/utils/registry_utils.py` & `hezar-0.38.1/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.38.0/pyproject.toml` & `hezar-0.38.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.38.0"
+version = "0.38.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!"
 license = "Apache-2.0"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.38.0/PKG-INFO` & `hezar-0.38.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.38.0
+Version: 0.38.1
 Summary: Hezar: The all-in-one AI library for Persian, supporting a wide variety of tasks and modalities!
 Home-page: https://github.com/hezarai
 License: Apache-2.0
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

