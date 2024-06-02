# Comparing `tmp/nusacrowd-0.1.3.tar.gz` & `tmp/nusacrowd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nusacrowd-0.1.3.tar", last modified: Sat Dec 16 02:49:50 2023, max compression
+gzip compressed data, was "nusacrowd-0.1.4.tar", last modified: Sun Jun  2 18:27:15 2024, max compression
```

## Comparing `nusacrowd-0.1.3.tar` & `nusacrowd-0.1.4.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.404088 nusacrowd-0.1.3/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    11357 2022-07-10 15:26:30.000000 nusacrowd-0.1.3/LICENSE
--rw-r--r--   0 samuel    (1020) samuel    (1020)     1072 2023-12-16 02:49:50.404088 nusacrowd-0.1.3/PKG-INFO
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7404 2023-09-07 12:26:06.000000 nusacrowd-0.1.3/README.md
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.864091 nusacrowd-0.1.3/nusacrowd/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      254 2023-12-16 02:47:42.000000 nusacrowd-0.1.3/nusacrowd/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    39273 2023-12-16 02:46:39.000000 nusacrowd-0.1.3/nusacrowd/config_helper.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.864091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/__init__.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.864091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/barasa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/barasa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7232 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/barasa/barasa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.872091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_en_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_en_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6804 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_en_id/bible_en_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.876091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_jv_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_jv_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6870 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_jv_id/bible_jv_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.888090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_su_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_su_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6646 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_su_id/bible_su_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.888090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/casa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/casa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5649 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/casa/casa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.896091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cc100/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cc100/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    10016 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cc100/cc100.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.900091 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cod/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cod/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6246 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cod/cod.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.908090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/code_mixed_jv_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/code_mixed_jv_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8788 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.916090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/covost2/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/covost2/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    10355 2023-03-20 12:04:07.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/covost2/covost2.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.920090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cvss/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cvss/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    11074 2022-12-08 05:10:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/cvss/cvss.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.932090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emot/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emot/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5536 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emot/emot.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.932090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotcmt/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotcmt/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4498 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotcmt/emotcmt.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.936090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotion_id_opinion/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotion_id_opinion/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7329 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.944090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5773 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/facqa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.944090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/utils/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/utils/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      815 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/utils/facqa_utils.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.948090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/hoasa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/hoasa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6315 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/hoasa/hoasa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.952090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6554 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive/id_abusive.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.952090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive_news_comment/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive_news_comment/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4307 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.960090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_am2ico/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-21 16:14:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_am2ico/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7442 2023-01-09 06:05:57.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_am2ico/id_am2ico.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.972090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_clickbait/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_clickbait/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5784 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_clickbait/id_clickbait.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.988090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_frog_story/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_frog_story/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4536 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_frog_story/id_frog_story.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.988090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_google_play_review/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_google_play_review/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6164 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_google_play_review/id_google_play_review.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.992090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hatespeech/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hatespeech/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4464 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hatespeech/id_hatespeech.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:49.996090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hoax_news/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hoax_news/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4569 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hoax_news/id_hoax_news.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.004090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hsd_nofaaulia/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hsd_nofaaulia/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7268 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.004090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_multilabel_hs/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_multilabel_hs/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6035 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.008090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_panl_bppt/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_panl_bppt/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5630 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_panl_bppt/id_panl_bppt.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.012090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_qqp/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_qqp/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4700 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_qqp/id_qqp.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.012090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9123 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.020090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/utils/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/utils/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     1826 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.020090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_stance/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_stance/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5126 2022-12-31 07:37:15.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_stance/id_stance.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.028090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_sts/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_sts/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4322 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_sts/id_sts.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.028090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_wiki_parallel/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_wiki_parallel/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6711 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.028090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/identic/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/identic/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    13392 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/identic/identic.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.032090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idk_mrc/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idk_mrc/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9514 2022-12-08 05:10:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idk_mrc/idk_mrc.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.036090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6208 2023-07-29 07:56:22.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.040090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/imdb_jv/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/imdb_jv/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4908 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/imdb_jv/imdb_jv.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.044090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7250 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b/indo4b.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.044090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b_plus/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b_plus/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7431 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b_plus/indo4b_plus.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.048090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_general_mt_en_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_general_mt_en_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6454 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.048090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_law/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_law/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5459 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_law/indo_law.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.048090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_puisi/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_puisi/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4033 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_puisi/indo_puisi.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.048090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_religious_mt_en_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_religious_mt_en_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8521 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.056090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocollex/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocollex/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6961 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocollex/indocollex.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.064090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    11626 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/indocoref.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.068090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9072 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/feature_utils.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     2091 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/file_utils.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4311 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/text_preprocess.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.072090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ner_ugm/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ner_ugm/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6417 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.072090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_nerui/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_nerui/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8210 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_nerui/indolem_nerui.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.072090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ntp/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ntp/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5899 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ntp/indolem_ntp.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.076090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_sentiment/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_sentiment/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    12718 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_sentiment/indolem_sentiment.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.076090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_tweet_ordering/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_tweet_ordering/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    12485 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.076090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_gsd/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_gsd/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8480 2023-07-29 07:50:25.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.080090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_pud/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_pud/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8849 2023-07-29 07:51:15.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.084090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonli/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonli/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8065 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonli/indonli.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.088090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonlu_nergrit/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonlu_nergrit/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5690 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.092090 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indosum/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indosum/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6886 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indosum/indosum.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.100089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indotacos/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indotacos/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5492 2023-01-09 06:47:34.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indotacos/indotacos.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.116089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indqner/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        1 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indqner/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6626 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indqner/indqner.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.116089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_digit_cdsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_digit_cdsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9870 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.128089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8453 2022-12-21 16:14:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.132089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_lvcsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_lvcsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9447 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.136089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_tts/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_tts/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8877 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.140089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    11631 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.140089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9945 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.148089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9832 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.156089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/inset_lexicon/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/inset_lexicon/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4843 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/inset_lexicon/inset_lexicon.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.168089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jadi_ide/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jadi_ide/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4418 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jadi_ide/jadi_ide.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.168089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_asr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_asr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6250 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_asr/jv_id_asr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.168089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_tts/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_tts/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7644 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_tts/jv_id_tts.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.168089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kamus_alay/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kamus_alay/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5300 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kamus_alay/kamus_alay.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.172089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/karonese_sentiment/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/karonese_sentiment/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4547 2022-12-22 02:15:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/karonese_sentiment/karonese_sentiment.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.176089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/keps/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/keps/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5081 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/keps/keps.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.184089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    10054 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc/kopi_cc.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.184089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc_news/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc_news/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5106 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc_news/kopi_cc_news.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.184089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_nllb/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_nllb/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5973 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_nllb/kopi_nllb.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.184089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/korpus_nusantara/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/korpus_nusantara/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8510 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/korpus_nusantara/korpus_nusantara.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.192089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/librivox_indonesia/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/librivox_indonesia/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8756 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/librivox_indonesia/librivox_indonesia.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.192089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/liputan6/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/liputan6/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7526 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/liputan6/liputan6.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.196089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/local_id_abusive/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/local_id_abusive/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7549 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/local_id_abusive/local_id_abusive.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.200089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/minangnlp_mt/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/minangnlp_mt/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6888 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/minangnlp_mt/minangnlp_mt.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.200089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/multilexnorm/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/multilexnorm/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6237 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/multilexnorm/multilexnorm.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.204089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nergrit/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nergrit/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6334 2023-07-29 08:29:58.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nergrit/nergrit.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.208089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nerp/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nerp/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4867 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nerp/nerp.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.208089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/netifier/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/netifier/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4852 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/netifier/netifier.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.208089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/news_en_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/news_en_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5017 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/news_en_id/news_en_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.208089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nllb_seed/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nllb_seed/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    15254 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nllb_seed/nllb_seed.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.220089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusa_kalimat/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-03-23 14:50:08.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusa_kalimat/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6530 2023-03-23 15:05:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusa_kalimat/nusa_kalimat.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.232089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_emot/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_emot/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8808 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.240089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8816 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.252089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_topic/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_topic/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8869 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.252089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_emot/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:53:23.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_emot/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8257 2023-07-30 06:53:23.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.252089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_mt/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-31 02:35:22.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_mt/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9176 2023-09-15 09:38:31.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.260089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_senti/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-31 02:35:22.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_senti/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8309 2023-07-31 02:35:22.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.264089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_mt/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_mt/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7601 2022-11-09 06:24:38.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_mt/nusax_mt.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.276089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_senti/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_senti/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7274 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_senti/nusax_senti.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.276089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ojw/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ojw/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5116 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ojw/ojw.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.276089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/paracotta_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/paracotta_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4782 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/paracotta_id/paracotta_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.280089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_id_nyo/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_id_nyo/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5485 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.288089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_su_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_su_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4796 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_su_id/parallel_su_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.300089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/posp/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/posp/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6005 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/posp/posp.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.300089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/postag_su/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/postag_su/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8047 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/postag_su/postag_su.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.300089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/sentiment_nathasa_review/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/sentiment_nathasa_review/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6016 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.312088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/singgalang/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/singgalang/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5445 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/singgalang/singgalang.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.312088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/smsa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/smsa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5589 2022-12-03 00:57:48.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/smsa/smsa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.312088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/squad_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/squad_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5283 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/squad_id/squad_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.312088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/stif_indonesia/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/stif_indonesia/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5149 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/stif_indonesia/stif_indonesia.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_emot/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_emot/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4585 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_emot/su_emot.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_asr/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_asr/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5616 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_asr/su_id_asr.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_tts/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_tts/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7652 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_tts/su_id_tts.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/talpco/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/talpco/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6891 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/talpco/talpco.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ted_en_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ted_en_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7119 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ted_en_id/ted_en_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.316089 nusacrowd-0.1.3/nusacrowd/nusa_datasets/term_a/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/term_a/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5373 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/term_a/term_a.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.320088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tico_19/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tico_19/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    12259 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tico_19/tico_19.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.320088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/titml_idn/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/titml_idn/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5915 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/titml_idn/titml_idn.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.324088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/toxicity_200/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/toxicity_200/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5986 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/toxicity_200/toxicity_200.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.324088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tydiqa_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tydiqa_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7019 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/tydiqa_id/tydiqa_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.328088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ud_id_csui/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ud_id_csui/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9214 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/ud_id_csui/ud_id_csui.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.336088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/unimorph_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/unimorph_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     7458 2022-12-03 00:57:24.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/unimorph_id/unimorph_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.340088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikiann/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikiann/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     8669 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikiann/wikiann.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.340088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikilingua/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikilingua/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4998 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikilingua/wikilingua.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.340088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wrete/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wrete/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6127 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/wrete/wrete.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.348088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/__init__.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.348088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/utils/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/utils/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      473 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/utils/x_fact_utils.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5909 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/x_fact.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.348088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xcopa/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xcopa/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6120 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xcopa/xcopa.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.348088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xl_sum/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xl_sum/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     5606 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xl_sum/xl_sum.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.348088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xpersona_id/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xpersona_id/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     6564 2023-07-29 08:29:41.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xpersona_id/xpersona_id.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.356088 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xsid/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xsid/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     9528 2023-07-19 06:09:59.000000 nusacrowd-0.1.3/nusacrowd/nusa_datasets/xsid/xsid.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.368088 nusacrowd-0.1.3/nusacrowd/utils/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-29 07:28:50.000000 nusacrowd-0.1.3/nusacrowd/utils/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4871 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/common_parser.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      286 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/configs.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     4895 2023-07-30 06:47:33.000000 nusacrowd-0.1.3/nusacrowd/utils/constants.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.400088 nusacrowd-0.1.3/nusacrowd/utils/schemas/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     1005 2022-10-23 02:39:37.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      506 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/image_text.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)     2283 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/kb.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      626 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/pairs.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      371 2022-10-22 07:33:32.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/pairs_multilabel.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      493 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/qa.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      206 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/self_supervised_pretraining.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      525 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/seq_label.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      454 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/speech_text.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      796 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/speech_to_speech.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      311 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/text.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      331 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/text_multilabel.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      444 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/nusacrowd/utils/schemas/text_to_text.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.400088 nusacrowd-0.1.3/nusacrowd.egg-info/
--rw-r--r--   0 samuel    (1020) samuel    (1020)     1072 2023-12-16 02:49:49.000000 nusacrowd-0.1.3/nusacrowd.egg-info/PKG-INFO
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    13971 2023-12-16 02:49:49.000000 nusacrowd-0.1.3/nusacrowd.egg-info/SOURCES.txt
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        1 2023-12-16 02:49:49.000000 nusacrowd-0.1.3/nusacrowd.egg-info/dependency_links.txt
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      409 2023-12-16 02:49:49.000000 nusacrowd-0.1.3/nusacrowd.egg-info/requires.txt
--rw-rw-r--   0 samuel    (1020) samuel    (1020)       16 2023-12-16 02:49:49.000000 nusacrowd-0.1.3/nusacrowd.egg-info/top_level.txt
--rw-rw-r--   0 samuel    (1020) samuel    (1020)      668 2023-12-16 02:49:50.404088 nusacrowd-0.1.3/setup.cfg
--rw-rw-r--   0 samuel    (1020) samuel    (1020)       68 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/setup.py
-drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2023-12-16 02:49:50.400088 nusacrowd-0.1.3/tests/
--rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-05-18 09:16:05.000000 nusacrowd-0.1.3/tests/__init__.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    23364 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/tests/test_nusantara.py
--rw-rw-r--   0 samuel    (1020) samuel    (1020)    20750 2022-09-26 14:15:09.000000 nusacrowd-0.1.3/tests/test_nusantara_source_only.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:15.044970 nusacrowd-0.1.4/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    11357 2022-07-10 15:26:30.000000 nusacrowd-0.1.4/LICENSE
+-rw-r--r--   0 samuel    (1020) samuel    (1020)     1072 2024-06-02 18:27:15.044970 nusacrowd-0.1.4/PKG-INFO
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7404 2023-09-07 12:26:06.000000 nusacrowd-0.1.4/README.md
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.484969 nusacrowd-0.1.4/nusacrowd/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      254 2024-06-02 18:24:19.000000 nusacrowd-0.1.4/nusacrowd/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    39273 2024-04-11 09:14:34.000000 nusacrowd-0.1.4/nusacrowd/config_helper.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.484969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/__init__.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.484969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/barasa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/barasa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7232 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/barasa/barasa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.492969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_en_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_en_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6804 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_en_id/bible_en_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.496969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_jv_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_jv_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6870 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_jv_id/bible_jv_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.500969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_su_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_su_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6646 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_su_id/bible_su_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.504969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/casa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/casa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5649 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/casa/casa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.512969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cc100/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cc100/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    10016 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cc100/cc100.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.520969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cod/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cod/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6246 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cod/cod.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.528969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/code_mixed_jv_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/code_mixed_jv_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8788 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.536969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/covost2/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/covost2/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    10355 2023-03-20 12:04:07.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/covost2/covost2.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.540969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cvss/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cvss/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    11074 2022-12-08 05:10:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/cvss/cvss.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.548969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emot/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emot/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5536 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emot/emot.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.552969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotcmt/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotcmt/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4498 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotcmt/emotcmt.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.560969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotion_id_opinion/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotion_id_opinion/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7329 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.564969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5773 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/facqa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.564969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/utils/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/utils/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      815 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/utils/facqa_utils.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.568969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/hoasa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/hoasa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6315 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/hoasa/hoasa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.572969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6554 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive/id_abusive.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.572969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive_news_comment/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive_news_comment/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4307 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.584969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_am2ico/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-21 16:14:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_am2ico/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7442 2023-01-09 06:05:57.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_am2ico/id_am2ico.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.596969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_clickbait/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_clickbait/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5784 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_clickbait/id_clickbait.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.612969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_frog_story/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_frog_story/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4536 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_frog_story/id_frog_story.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.612969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_google_play_review/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_google_play_review/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6164 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_google_play_review/id_google_play_review.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.612969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hatespeech/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hatespeech/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4464 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hatespeech/id_hatespeech.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.616969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hoax_news/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hoax_news/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4569 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hoax_news/id_hoax_news.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.620969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hsd_nofaaulia/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hsd_nofaaulia/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7268 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.632969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_multilabel_hs/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_multilabel_hs/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6035 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.632969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_panl_bppt/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_panl_bppt/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5630 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_panl_bppt/id_panl_bppt.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.636969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_qqp/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_qqp/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4700 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_qqp/id_qqp.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.636969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9123 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.640969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/utils/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/utils/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     1826 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.648970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_stance/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_stance/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5126 2022-12-31 07:37:15.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_stance/id_stance.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.656969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_sts/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_sts/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4322 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_sts/id_sts.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.660969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_wiki_parallel/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_wiki_parallel/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6711 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.660969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/identic/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/identic/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    13392 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/identic/identic.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.660969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idk_mrc/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idk_mrc/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9514 2022-12-08 05:10:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idk_mrc/idk_mrc.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.668969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6208 2023-07-29 07:56:22.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.676969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/imdb_jv/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/imdb_jv/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4908 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/imdb_jv/imdb_jv.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.680969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7250 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b/indo4b.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.684970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b_plus/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b_plus/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7431 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b_plus/indo4b_plus.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.684970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_general_mt_en_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_general_mt_en_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6454 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.688969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_law/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_law/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5459 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_law/indo_law.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.692969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_puisi/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_puisi/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4033 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_puisi/indo_puisi.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.692969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_religious_mt_en_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_religious_mt_en_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8521 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.696969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocollex/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocollex/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6961 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocollex/indocollex.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.704970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    11626 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/indocoref.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.708969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9072 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/feature_utils.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     2091 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/file_utils.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4311 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/text_preprocess.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.708969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ner_ugm/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ner_ugm/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6417 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.720970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_nerui/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_nerui/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8210 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_nerui/indolem_nerui.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.720970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ntp/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ntp/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5899 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ntp/indolem_ntp.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.720970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_sentiment/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_sentiment/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    12718 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_sentiment/indolem_sentiment.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.720970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_tweet_ordering/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_tweet_ordering/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    12485 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.728969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_gsd/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_gsd/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8480 2023-07-29 07:50:25.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.732969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_pud/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_pud/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8849 2023-07-29 07:51:15.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.740970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonli/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonli/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8065 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonli/indonli.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.740970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonlu_nergrit/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonlu_nergrit/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5690 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.748969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indosum/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indosum/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6886 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indosum/indosum.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.752970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indotacos/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indotacos/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5492 2023-01-09 06:47:34.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indotacos/indotacos.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.772970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indqner/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        1 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indqner/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6626 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indqner/indqner.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.772970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_digit_cdsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_digit_cdsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9870 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.776970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8453 2022-12-21 16:14:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.776970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_lvcsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_lvcsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9447 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.784969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_tts/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_tts/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8877 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.788970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    11631 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.788970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9945 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.788970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9832 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.796970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/inset_lexicon/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/inset_lexicon/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4843 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/inset_lexicon/inset_lexicon.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.796970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jadi_ide/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jadi_ide/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4418 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jadi_ide/jadi_ide.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.796970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_asr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_asr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6250 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_asr/jv_id_asr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.800969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_tts/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_tts/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7644 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_tts/jv_id_tts.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.800969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kamus_alay/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kamus_alay/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5300 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kamus_alay/kamus_alay.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.808970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/karonese_sentiment/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/karonese_sentiment/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4547 2022-12-22 02:15:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/karonese_sentiment/karonese_sentiment.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.816969 nusacrowd-0.1.4/nusacrowd/nusa_datasets/keps/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/keps/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5081 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/keps/keps.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.824970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    10054 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc/kopi_cc.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.824970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc_news/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc_news/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5106 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc_news/kopi_cc_news.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.824970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_nllb/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_nllb/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5973 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_nllb/kopi_nllb.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.824970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/korpus_nusantara/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/korpus_nusantara/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8510 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/korpus_nusantara/korpus_nusantara.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.832970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/librivox_indonesia/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/librivox_indonesia/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8756 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/librivox_indonesia/librivox_indonesia.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.832970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/liputan6/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/liputan6/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7526 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/liputan6/liputan6.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.844970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/local_id_abusive/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/local_id_abusive/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7549 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/local_id_abusive/local_id_abusive.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.848970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/minangnlp_mt/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/minangnlp_mt/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6888 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/minangnlp_mt/minangnlp_mt.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.848970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/multilexnorm/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/multilexnorm/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6237 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/multilexnorm/multilexnorm.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.856970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nergrit/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nergrit/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6334 2023-07-29 08:29:58.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nergrit/nergrit.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.860970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nerp/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nerp/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4867 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nerp/nerp.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.860970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/netifier/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/netifier/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4852 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/netifier/netifier.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.860970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/news_en_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/news_en_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5017 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/news_en_id/news_en_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.864970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nllb_seed/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nllb_seed/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    15254 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nllb_seed/nllb_seed.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.868970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusa_kalimat/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-03-23 14:50:08.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusa_kalimat/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6530 2023-03-23 15:05:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusa_kalimat/nusa_kalimat.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.872970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_emot/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_emot/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8808 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.880970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8816 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.884970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_topic/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_topic/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8869 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.884970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_emot/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-30 06:53:23.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_emot/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8257 2024-06-02 18:23:48.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.884970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_mt/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-31 02:35:22.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_mt/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9183 2024-06-02 18:23:48.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.884970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_senti/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-31 02:35:22.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_senti/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8316 2024-06-02 18:23:48.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.884970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_mt/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_mt/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7601 2022-11-09 06:24:38.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_mt/nusax_mt.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.888970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_senti/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_senti/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7274 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_senti/nusax_senti.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.896970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ojw/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ojw/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5116 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ojw/ojw.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.896970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/paracotta_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/paracotta_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4782 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/paracotta_id/paracotta_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.900970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_id_nyo/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_id_nyo/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5485 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.904970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_su_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_su_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4796 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_su_id/parallel_su_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.916970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/posp/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/posp/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6005 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/posp/posp.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.916970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/postag_su/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/postag_su/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8047 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/postag_su/postag_su.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.916970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/sentiment_nathasa_review/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/sentiment_nathasa_review/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6016 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.924970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/singgalang/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/singgalang/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5445 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/singgalang/singgalang.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.924970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/smsa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/smsa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5589 2022-12-03 00:57:48.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/smsa/smsa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.924970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/squad_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/squad_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5283 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/squad_id/squad_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.928970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/stif_indonesia/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/stif_indonesia/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5149 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/stif_indonesia/stif_indonesia.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.928970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_emot/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_emot/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4585 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_emot/su_emot.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.928970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_asr/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_asr/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5616 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_asr/su_id_asr.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.928970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_tts/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_tts/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7652 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_tts/su_id_tts.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.928970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/talpco/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/talpco/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6891 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/talpco/talpco.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.932970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ted_en_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ted_en_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7119 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ted_en_id/ted_en_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.932970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/term_a/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/term_a/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5373 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/term_a/term_a.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.940970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tico_19/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tico_19/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    12259 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tico_19/tico_19.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.940970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/titml_idn/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/titml_idn/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5915 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/titml_idn/titml_idn.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.948970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/toxicity_200/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/toxicity_200/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5986 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/toxicity_200/toxicity_200.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.948970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tydiqa_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tydiqa_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7019 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/tydiqa_id/tydiqa_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.948970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ud_id_csui/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ud_id_csui/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9214 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/ud_id_csui/ud_id_csui.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.956970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/unimorph_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/unimorph_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     7458 2022-12-03 00:57:24.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/unimorph_id/unimorph_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.964970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikiann/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikiann/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     8669 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikiann/wikiann.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.964970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikilingua/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikilingua/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4998 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikilingua/wikilingua.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.964970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wrete/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wrete/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6127 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/wrete/wrete.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.972970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/__init__.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.972970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/utils/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/utils/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      473 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/utils/x_fact_utils.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5909 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/x_fact.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.972970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xcopa/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xcopa/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6120 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xcopa/xcopa.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.972970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xl_sum/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xl_sum/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     5606 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xl_sum/xl_sum.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.972970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xpersona_id/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xpersona_id/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     6564 2023-07-29 08:29:41.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xpersona_id/xpersona_id.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.980970 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xsid/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xsid/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     9528 2023-07-19 06:09:59.000000 nusacrowd-0.1.4/nusacrowd/nusa_datasets/xsid/xsid.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:14.996970 nusacrowd-0.1.4/nusacrowd/utils/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2023-07-29 07:28:50.000000 nusacrowd-0.1.4/nusacrowd/utils/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4871 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/common_parser.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      286 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/configs.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     4895 2023-07-30 06:47:33.000000 nusacrowd-0.1.4/nusacrowd/utils/constants.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:15.040970 nusacrowd-0.1.4/nusacrowd/utils/schemas/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     1005 2022-10-23 02:39:37.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      506 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/image_text.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)     2283 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/kb.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      626 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/pairs.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      371 2022-10-22 07:33:32.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/pairs_multilabel.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      493 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/qa.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      206 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      525 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/seq_label.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      454 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/speech_text.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      796 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/speech_to_speech.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      311 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/text.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      331 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/text_multilabel.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      444 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/nusacrowd/utils/schemas/text_to_text.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:15.040970 nusacrowd-0.1.4/nusacrowd.egg-info/
+-rw-r--r--   0 samuel    (1020) samuel    (1020)     1072 2024-06-02 18:27:14.000000 nusacrowd-0.1.4/nusacrowd.egg-info/PKG-INFO
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    13971 2024-06-02 18:27:14.000000 nusacrowd-0.1.4/nusacrowd.egg-info/SOURCES.txt
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        1 2024-06-02 18:27:14.000000 nusacrowd-0.1.4/nusacrowd.egg-info/dependency_links.txt
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      409 2024-06-02 18:27:14.000000 nusacrowd-0.1.4/nusacrowd.egg-info/requires.txt
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)       16 2024-06-02 18:27:14.000000 nusacrowd-0.1.4/nusacrowd.egg-info/top_level.txt
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)      668 2024-06-02 18:27:15.044970 nusacrowd-0.1.4/setup.cfg
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)       68 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/setup.py
+drwxrwxr-x   0 samuel    (1020) samuel    (1020)        0 2024-06-02 18:27:15.040970 nusacrowd-0.1.4/tests/
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)        0 2022-05-18 09:16:05.000000 nusacrowd-0.1.4/tests/__init__.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    23364 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/tests/test_nusantara.py
+-rw-rw-r--   0 samuel    (1020) samuel    (1020)    20750 2022-09-26 14:15:09.000000 nusacrowd-0.1.4/tests/test_nusantara_source_only.py
```

### Comparing `nusacrowd-0.1.3/LICENSE` & `nusacrowd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/PKG-INFO` & `nusacrowd-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nusacrowd
-Version: 0.1.3
+Version: 0.1.4
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `nusacrowd-0.1.3/README.md` & `nusacrowd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/config_helper.py` & `nusacrowd-0.1.4/nusacrowd/config_helper.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/barasa/barasa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_en_id/bible_en_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_jv_id/bible_jv_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/bible_su_id/bible_su_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/casa/casa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/cc100/cc100.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/cod/cod.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/covost2/covost2.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/cvss/cvss.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/emot/emot.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotcmt/emotcmt.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/emotion_id_opinion/emotion_id_opinion.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/facqa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/facqa/utils/facqa_utils.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/hoasa/hoasa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive/id_abusive.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_am2ico/id_am2ico.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_clickbait/id_clickbait.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_frog_story/id_frog_story.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_google_play_review/id_google_play_review.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hatespeech/id_hatespeech.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hoax_news/id_hoax_news.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_multilabel_hs/id_multilabel_hs.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_panl_bppt/id_panl_bppt.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_qqp/id_qqp.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/id_short_answer_grading.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_stance/id_stance.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_sts/id_sts.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/id_wiki_parallel/id_wiki_parallel.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/identic/identic.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/idk_mrc/idk_mrc.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/imdb_jv/imdb_jv.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b/indo4b.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo4b_plus/indo4b_plus.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_law/indo_law.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_puisi/indo_puisi.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocollex/indocollex.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/indocoref.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/feature_utils.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/file_utils.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indocoref/utils/text_preprocess.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_nerui/indolem_nerui.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ntp/indolem_ntp.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_sentiment/indolem_sentiment.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonli/indonli.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indonlu_nergrit/indonlu_nergrit.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indosum/indosum.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indotacos/indotacos.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indqner/indqner.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_news_tts/indspeech_news_tts.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/inset_lexicon/inset_lexicon.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/jadi_ide/jadi_ide.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_asr/jv_id_asr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/jv_id_tts/jv_id_tts.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/kamus_alay/kamus_alay.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/karonese_sentiment/karonese_sentiment.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/keps/keps.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc/kopi_cc.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_cc_news/kopi_cc_news.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/kopi_nllb/kopi_nllb.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/korpus_nusantara/korpus_nusantara.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/librivox_indonesia/librivox_indonesia.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/liputan6/liputan6.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/local_id_abusive/local_id_abusive.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/minangnlp_mt/minangnlp_mt.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/multilexnorm/multilexnorm.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nergrit/nergrit.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nerp/nerp.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/netifier/netifier.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/news_en_id/news_en_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nllb_seed/nllb_seed.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusa_kalimat/nusa_kalimat.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusa_kalimat/nusa_kalimat.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_emot/nusatranslation_emot.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _LOCAL = False
 
 _DATASETNAME = "nusatranslation_emot"
 _SOURCE_VIEW_NAME = DEFAULT_SOURCE_VIEW_NAME
 _UNIFIED_VIEW_NAME = DEFAULT_NUSANTARA_VIEW_NAME
 
-_LANGUAGES = ["abs", "btk", "bew", "bug", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
+_LANGUAGES = ["abs", "btk", "bew", "bhp", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
 
 _CITATION = """\
     @unpublished{anonymous2023nusawrites:,
     title={NusaWrites: Constructing High-Quality Corpora for Underrepresented and Extremely Low-Resource Languages},
     author={Anonymous},
     journal={OpenReview Preprint},
     year={2023},
```

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_mt/nusatranslation_mt.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from nusacrowd.utils.configs import NusantaraConfig
 from nusacrowd.utils.constants import DEFAULT_NUSANTARA_VIEW_NAME, DEFAULT_SOURCE_VIEW_NAME, Tasks
 
 _DATASETNAME = "nusatranslation_mt"
 _SOURCE_VIEW_NAME = DEFAULT_SOURCE_VIEW_NAME
 _UNIFIED_VIEW_NAME = DEFAULT_NUSANTARA_VIEW_NAME
 
-_LANGUAGES = ["ind", "btk", "bew", "bug", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
+_LANGUAGES = ["ind", "abs", "btk", "bew", "bhp", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
 _LOCAL = False
 
 _CITATION = """\
     @unpublished{anonymous2023nusawrites:,
     title={NusaWrites: Constructing High-Quality Corpora for Underrepresented and Extremely Low-Resource Languages},
     author={Anonymous},
     journal={OpenReview Preprint},
```

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusatranslation_senti/nusatranslation_senti.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _LOCAL = False
 
 _DATASETNAME = "nusatranslation_senti"
 _SOURCE_VIEW_NAME = DEFAULT_SOURCE_VIEW_NAME
 _UNIFIED_VIEW_NAME = DEFAULT_NUSANTARA_VIEW_NAME
 
-_LANGUAGES = ["btk", "bew", "bug", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
+_LANGUAGES = ["abs", "btk", "bew", "bhp", "jav", "mad", "mak", "min", "mui", "rej", "sun"]  # We follow ISO639-3 language code (https://iso639-3.sil.org/code_tables/639/data)
 
 _CITATION = """\
     @unpublished{anonymous2023nusawrites:,
     title={NusaWrites: Constructing High-Quality Corpora for Underrepresented and Extremely Low-Resource Languages},
     author={Anonymous},
     journal={OpenReview Preprint},
     year={2023},
```

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_mt/nusax_mt.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/nusax_senti/nusax_senti.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/ojw/ojw.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/paracotta_id/paracotta_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_id_nyo/parallel_id_nyo.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/parallel_su_id/parallel_su_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/posp/posp.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/postag_su/postag_su.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/singgalang/singgalang.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/smsa/smsa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/squad_id/squad_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/stif_indonesia/stif_indonesia.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_emot/su_emot.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_asr/su_id_asr.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/su_id_tts/su_id_tts.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/talpco/talpco.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/ted_en_id/ted_en_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/term_a/term_a.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/tico_19/tico_19.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/titml_idn/titml_idn.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/toxicity_200/toxicity_200.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/tydiqa_id/tydiqa_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/tydiqa_id/tydiqa_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/ud_id_csui/ud_id_csui.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/unimorph_id/unimorph_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikiann/wikiann.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/wikilingua/wikilingua.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/wrete/wrete.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/x_fact/x_fact.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/xcopa/xcopa.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/xl_sum/xl_sum.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/xpersona_id/xpersona_id.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/nusa_datasets/xsid/xsid.py` & `nusacrowd-0.1.4/nusacrowd/nusa_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/common_parser.py` & `nusacrowd-0.1.4/nusacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/constants.py` & `nusacrowd-0.1.4/nusacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/schemas/__init__.py` & `nusacrowd-0.1.4/nusacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/schemas/kb.py` & `nusacrowd-0.1.4/nusacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/schemas/pairs.py` & `nusacrowd-0.1.4/nusacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/schemas/seq_label.py` & `nusacrowd-0.1.4/nusacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd/utils/schemas/speech_to_speech.py` & `nusacrowd-0.1.4/nusacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/nusacrowd.egg-info/PKG-INFO` & `nusacrowd-0.1.4/nusacrowd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nusacrowd
-Version: 0.1.3
+Version: 0.1.4
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `nusacrowd-0.1.3/nusacrowd.egg-info/SOURCES.txt` & `nusacrowd-0.1.4/nusacrowd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/setup.cfg` & `nusacrowd-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/tests/test_nusantara.py` & `nusacrowd-0.1.4/tests/test_nusantara.py`

 * *Files identical despite different names*

### Comparing `nusacrowd-0.1.3/tests/test_nusantara_source_only.py` & `nusacrowd-0.1.4/tests/test_nusantara_source_only.py`

 * *Files identical despite different names*

