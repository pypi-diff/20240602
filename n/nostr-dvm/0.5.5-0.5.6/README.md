# Comparing `tmp/nostr_dvm-0.5.5.tar.gz` & `tmp/nostr_dvm-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.5.5.tar", last modified: Sat Jun  1 17:31:28 2024, max compression
+gzip compressed data, was "nostr_dvm-0.5.6.tar", last modified: Sat Jun  1 21:47:23 2024, max compression
```

## Comparing `nostr_dvm-0.5.5.tar` & `nostr_dvm-0.5.6.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.634043 nostr_dvm-0.5.5/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    41554 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.646043 nostr_dvm-0.5.5/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.859486 nostr_dvm-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 21:47:23.859486 nostr_dvm-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.839486 nostr_dvm-0.5.6/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.839486 nostr_dvm-0.5.6/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.839486 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.839486 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.843486 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.843486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.843486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.843486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.843486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.847486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.847486 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41554 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.847486 nostr_dvm-0.5.6/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.851486 nostr_dvm-0.5.6/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.855486 nostr_dvm-0.5.6/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.855486 nostr_dvm-0.5.6/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.855486 nostr_dvm-0.5.6/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 21:47:23.000000 nostr_dvm-0.5.6/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 21:47:23.000000 nostr_dvm-0.5.6/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 21:47:23.000000 nostr_dvm-0.5.6/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 21:47:23.000000 nostr_dvm-0.5.6/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 21:47:23.000000 nostr_dvm-0.5.6/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 21:47:23.859486 nostr_dvm-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 21:47:23.855486 nostr_dvm-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-01 21:47:19.000000 nostr_dvm-0.5.6/tests/test_events.py
```

### Comparing `nostr_dvm-0.5.5/LICENSE` & `nostr_dvm-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/PKG-INFO` & `nostr_dvm-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.5
+Version: 0.5.6
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.5/README.md` & `nostr_dvm-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.5.6/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/bot.py` & `nostr_dvm-0.5.6/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/dvm.py` & `nostr_dvm-0.5.6/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.5.6/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/subscription.py` & `nostr_dvm-0.5.6/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,84 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
-    RelayOptions
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag, create_amount_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
-This File contains a Module to discover popular notes
+This File contains a Module to discover popular notes by topics
 Accepted Inputs: none
 Outputs: A list of events 
 Params:  None
 """
 
 
-class DicoverContentCurrentlyPopular(DVMTaskInterface):
+class DicoverContentCurrentlyPopularbyTopic(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
-    db_since = 3600
-    db_name = "db/nostr_recent_notes.db"
     min_reactions = 2
+    db_since = 10*3600
+    db_name = "db/nostr_default_recent_notes.db"
+    search_list = []
+    avoid_list = []
+    must_list = []
     personalized = False
     result = ""
-    logger = False
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        dvm_config.SCRIPT = os.path.abspath(__file__)
+
+
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
+        # Generate Generic request form for dvms that provide generic results (e.g only a calculation per update,
+        # not per call)
         self.request_form = {"jobID": "generic"}
         opts = {
             "max_results": 200,
         }
         self.request_form['options'] = json.dumps(opts)
 
-        self.last_schedule = Timestamp.now().as_secs()
-        if self.options is not None:
-            if self.options.get("db_name"):
-                self.db_name = self.options.get("db_name")
-            if self.options.get("db_since"):
-                self.db_since = int(self.options.get("db_since"))
-            if self.options.get("logger"):
-                self.logger = bool(self.options.get("logger"))
-
-            if self.logger:
-                init_logger(LogLevel.DEBUG)
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite(self.db_name)
-        self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
-
-        ropts = RelayOptions().ping(False)
-        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
-        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
-        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
-
-        self.client.connect()
-
+        dvm_config.SCRIPT = os.path.abspath(__file__)
 
+        if self.options.get("personalized"):
+            self.personalized = bool(self.options.get("personalized"))
+        self.last_schedule = Timestamp.now().as_secs()
+        if self.options.get("search_list"):
+            self.search_list = self.options.get("search_list")
+            #print(self.search_list)
+        if self.options.get("avoid_list"):
+            self.avoid_list = self.options.get("avoid_list")
+        if self.options.get("must_list"):
+            self.must_list = self.options.get("must_list")
+        if self.options.get("db_name"):
+            self.db_name = self.options.get("db_name")
+        if self.options.get("db_since"):
+            self.db_since = int(self.options.get("db_since"))
+
+
+        use_logger = False
+        if use_logger:
+            init_logger(LogLevel.DEBUG)
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
-
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
@@ -92,145 +89,175 @@
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
-        search = ""
-        max_results = 100
+        max_results = 200
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
             elif tag.as_vec()[0] == 'param':
                 param = tag.as_vec()[1]
                 if param == "max_results":  # check for param type
                     max_results = int(tag.as_vec()[2])
 
         options = {
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
+        self.request_form = request_form
         return request_form
 
     def process(self, request_form):
         # if the dvm supports individual results, recalculate it every time for the request
         if self.personalized:
             return self.calculate_result(request_form)
-        # else return the result that gets updated once every scheduled update. In this case on database update.
+        #else return the result that gets updated once every schenduled update. In this case on database update.
         else:
             return self.result
 
+
+    def post_process(self, result, event):
+        """Overwrite the interface function to return a social client readable format, if requested"""
+        for tag in event.tags():
+            if tag.as_vec()[0] == 'output':
+                format = tag.as_vec()[1]
+                if format == "text/plain":  # check for output type
+                    result = post_process_list_to_events(result)
+
+        # if not text/plain, don't post-process
+        return result
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = self.set_options(request_form)
 
-        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
-        since = Timestamp.from_secs(timestamp_hour_ago)
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
+
+        cli.connect()
+
+        # Negentropy reconciliation
+        # Query events from database
+        timestamp_since = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_since)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
-        events = self.client.database().query([filter1])
-        print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
 
+        events = cli.database().query([filter1])
+        print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
         ns.finallist = {}
-        for event in events:
-            if event.created_at().as_secs() > timestamp_hour_ago:
-                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
-                                       definitions.EventDefinitions.KIND_REACTION,
-                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
-                reactions = self.client.database().query([filt])
-                if len(reactions) >= self.min_reactions:
-                    ns.finallist[event.id().to_hex()] = len(reactions)
 
-        if len(ns.finallist) == 0:
-            return self.result
+        for event in events:
+            if all(ele in event.content().lower() for ele in self.must_list):
+                if any(ele in event.content().lower() for ele in self.search_list):
+                    if not any(ele in event.content().lower() for ele in self.avoid_list):
+
+                        filt = Filter().kinds(
+                            [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION,
+                             definitions.EventDefinitions.KIND_REPOST,
+                             definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
+                        reactions = cli.database().query([filt])
+                        if len(reactions) >= self.min_reactions:
+                            ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
+            # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
+        print(len(result_list))
 
+        cli.disconnect()
+        cli.shutdown()
         return json.dumps(result_list)
 
-    def post_process(self, result, event):
-        """Overwrite the interface function to return a social client readable format, if requested"""
-        for tag in event.tags():
-            if tag.as_vec()[0] == 'output':
-                format = tag.as_vec()[1]
-                if format == "text/plain":  # check for output type
-                    result = post_process_list_to_events(result)
-
-        # if not text/plain, don't post-process
-        return result
 
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
                 if self.dvm_config.UPDATE_DATABASE:
                     self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
-                if not self.personalized:
-                    try:
-                        self.result = self.calculate_result(self.request_form)
-                    except Exception as e:
-                        print("EXCEPTION: " + str(e))
+                self.result = self.calculate_result(self.request_form)
+                #print(self.result)
                 return 1
 
     def sync_db(self):
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
-        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
-        lasthour = Timestamp.from_secs(timestamp_hour_ago)
+        cli.add_relay("wss://relay.damus.io")
+        cli.add_relay("wss://nostr.oxtr.dev")
+        cli.add_relay("wss://relay.nostr.net")
+        cli.add_relay("wss://relay.nostr.bg")
+        cli.add_relay("wss://nostr.wine")
+        cli.add_relay("wss://nostr21.com")
+
+        #RELAY_LIST = [ "wss://nostr.wine",
+        #              , "wss://relay.nostr.bg",
+        #              , "wss://relay.nostr.net"
+        #              ]
+        cli.connect()
 
-        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
-                                  definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
+        timestamp_since = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_since)
+
+        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_ZAP]).since(since)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
-            self.db_since) + " seconds.. this might take a while..")
+        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
-        self.client.reconcile(filter1, dbopts)
-        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
-        self.client.database().delete(filter_delete)  # Clear old events so db doesn't get too full.
+        cli.reconcile(filter1, dbopts)
+        database.delete(Filter().until(Timestamp.from_secs(
+            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesn't get too full.
 
-        print(
-            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+        print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options, cost=0, update_rate=180, processing_msg=None,
-                  update_db=True):
+def build_example(name, identifier, admin_config, options, image, description, update_rate=600, cost=0, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 10 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = cost
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-    image = "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "picture": image,
-        "about": "I show notes that are currently popular",
+        "about": description,
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": False,
         "amount": create_amount_tag(cost),
         "nip90Params": {
             "max_results": {
@@ -241,41 +268,36 @@
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    # admin_config.UPDATE_PROFILE = False
-    # admin_config.REBROADCAST_NIP89 = False
-
-    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
+    return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None,
-                               update_db=True):
+def build_example_subscription(name, identifier, admin_config, options, image, description, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
-    dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 3 minutes
+    dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
-    # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
-    image = "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
+
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "picture": image,
-        "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
+        "about": description,
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
         "personalized": False,
         "nip90Params": {
             "max_results": {
@@ -299,22 +321,21 @@
     nip88config.AMOUNT_DAILY = 100
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
-    # admin_config.UPDATE_PROFILE = False
-    # admin_config.REBROADCAST_NIP89 = False
-    # admin_config.REBROADCAST_NIP88 = False
-
-    # admin_config.FETCH_NIP88 = True
-    # admin_config.EVENTID = ""
-    # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
-
-    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                          nip88config=nip88config, options=options,
-                                          admin_config=admin_config)
+
+   # admin_config.FETCH_NIP88 = True
+   # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
+   # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
+
+
+    return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                          nip88config=nip88config,
+                                          admin_config=admin_config,
+                                          options=options)
 
 
 if __name__ == '__main__':
-    process_venv(DicoverContentCurrentlyPopular)
+    process_venv(DicoverContentCurrentlyPopularbyTopic)
```

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,27 +56,14 @@
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
 
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite(self.db_name)
-        self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
-
-        ropts = RelayOptions().ping(False)
-        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
-        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
-        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
-
-        self.client.connect()
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
@@ -122,29 +109,38 @@
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = self.set_options(request_form)
 
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
+
+        cli.connect()
 
         # Negentropy reconciliation
         # Query events from database
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
-        events = self.client.database().query([filter1])
+        events = cli.database().query([filter1])
         print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
 
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
                 filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP]).event(event.id()).since(since)
-                reactions = self.client.database().query([filt])
+                reactions = cli.database().query([filt])
                 invoice_amount = 0
                 haspreimage = False
                 if len(reactions) >= self.min_reactions:
                     for reaction in reactions:
                         for tag in reaction.tags():
                             # print(tag.as_vec())
                             if tag.as_vec()[0] == 'bolt11':
@@ -161,14 +157,17 @@
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
             # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
 
+        cli.disconnect()
+        cli.shutdown()
+
         return json.dumps(result_list)
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
         for tag in event.tags():
             if tag.as_vec()[0] == 'output':
                 format = tag.as_vec()[1]
```

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,50 +27,31 @@
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
     db_since = 2 * 3600
     db_name = "db/nostr_recent_notes2.db"
     min_reactions = 2
-    logger = False
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
         self.last_schedule = Timestamp.now().as_secs()
-        if self.options is not None:
-            if self.options.get("db_name"):
-                self.db_name = self.options.get("db_name")
-            if self.options.get("db_since"):
-                self.db_since = int(self.options.get("db_since"))
-            if self.options.get("logger"):
-                self.logger = bool(self.options.get("logger"))
 
-            if self.logger:
-                init_logger(LogLevel.DEBUG)
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite(self.db_name)
-        self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
-
-        ropts = RelayOptions().ping(False)
-        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
-        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
-        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
-
-        #ropts = RelayOptions().ping(False)
-        #self.client.add_relay_with_opts("wss://nostr.band", ropts)
-
-        self.client.connect()
+        if self.options.get("db_name"):
+            self.db_name = self.options.get("db_name")
+        if self.options.get("db_since"):
+            self.db_since = int(self.options.get("db_since"))
+
+        use_logger = False
+        if use_logger:
+            init_logger(LogLevel.DEBUG)
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
@@ -85,88 +66,108 @@
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
         user = event.author().to_hex()
         max_results = 100
 
+
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
             elif tag.as_vec()[0] == 'param':
                 param = tag.as_vec()[1]
                 if param == "max_results":  # check for param type
                     max_results = int(tag.as_vec()[2])
                 elif param == "user":  # check for param type
                     user = tag.as_vec()[2]
 
+
+
         options = {
             "max_results": max_results,
             "user": user,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = self.set_options(request_form)
-
         relaylimits = RelayLimits.disable()
-        opts = (
-            Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)).relay_limits(
-                relaylimits))
+        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(relaylimits))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
+        cli.add_relay("wss://relay.damus.io")
+        cli.add_relay("wss://nostr.oxtr.dev")
+        cli.add_relay("wss://nostr.mom")
+
+        #ropts = RelayOptions().ping(False)
+        #cli.add_relay_with_opts("wss://nostr.band", ropts)
+
+        cli.connect()
 
         user = PublicKey.parse(options["user"])
         followers_filter = Filter().author(user).kinds([Kind(3)])
-        followers = self.client.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
+        followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
+        #print(followers)
 
         # Negentropy reconciliation
         # Query events from database
         timestamp_since = Timestamp.now().as_secs() - self.db_since
         since = Timestamp.from_secs(timestamp_since)
 
+
         result_list = []
 
         if len(followers) > 0:
             newest = 0
             best_entry = followers[0]
             for entry in followers:
                 if entry.created_at().as_secs() > newest:
                     newest = entry.created_at().as_secs()
                     best_entry = entry
 
-            # print(best_entry.as_json())
+            #print(best_entry.as_json())
             followings = []
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = PublicKey.parse(tag.as_vec()[1])
                     followings.append(following)
-            print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(followings)) + " Followers")
+
             filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(since)
-            events = self.client.database().query([filter1])
+            events = cli.database().query([filter1])
             print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
 
             ns.finallist = {}
             for event in events:
-                # if event.created_at().as_secs() > timestamp_since:
+                #if event.created_at().as_secs() > timestamp_since:
                 filt = Filter().kinds(
-                    [EventDefinitions.KIND_ZAP, EventDefinitions.KIND_REACTION, EventDefinitions.KIND_REPOST,
-                     EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
-                reactions = self.client.database().query([filt])
+                    [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_REPOST,
+                     definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
+                reactions = cli.database().query([filt])
                 if len(reactions) >= self.min_reactions:
                     ns.finallist[event.id().to_hex()] = len(reactions)
 
-            finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[
-                               :int(options["max_results"])]
+
+
+            finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
             for entry in finallist_sorted:
+                # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
                 e_tag = Tag.parse(["e", entry[0]])
                 result_list.append(e_tag.as_vec())
+            cli.connect()
+            cli.shutdown()
 
         return json.dumps(result_list)
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
         for tag in event.tags():
             if tag.as_vec()[0] == 'output':
@@ -183,42 +184,47 @@
         # We simply use the db from the other dvm that contains all notes
 
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
                 if self.dvm_config.UPDATE_DATABASE:
                     self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
-
                 return 1
 
     def sync_db(self):
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
+        cli.add_relay("wss://relay.damus.io")
+        cli.connect()
 
         timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
-                                  definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST]).since(lasthour)  # Notes, reactions, zaps
+                                  definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
-            self.db_since) + " seconds.. this might take a while..")
+        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
-        self.client.reconcile(filter1, dbopts)
-        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
-        self.client.database().delete(filter_delete)  # Clear old events so db doesn't get too full.
-        print(
-            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+        cli.reconcile(filter1, dbopts)
+        database.delete(Filter().until(Timestamp.from_secs(
+            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
+
+        print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options, cost=0, update_rate=300, processing_msg=None,
-                  update_db=True):
+def build_example(name, identifier, admin_config, options,  cost=0, update_rate=300, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every x seconds
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
@@ -251,16 +257,15 @@
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     # admin_config.UPDATE_PROFILE = False
     # admin_config.REBROADCAST_NIP89 = False
 
-    return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                                   options=options,
+    return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config, options=options,
                                                    admin_config=admin_config)
 
 
 def build_example_subscription(name, identifier, admin_config, options, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
@@ -315,8 +320,8 @@
 
     return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                                    nip88config=nip88config, options=options,
                                                    admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(DicoverContentCurrentlyPopularFollowers)
+    process_venv(DicoverContentCurrentlyPopularFollowers)
```

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,257 +1,239 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
     ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
-    RelayLimits, RelayOptions
+    RelayOptions
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag, create_amount_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
-This File contains a Module to discover popular notes by topic
+This File contains a Module to discover popular notes
 Accepted Inputs: none
 Outputs: A list of events 
 Params:  None
 """
 
 
-class DicoverContentCurrentlyPopularbyTopic(DVMTaskInterface):
+class DicoverContentCurrentlyPopular(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
+    db_since = 3600
+    db_name = "db/nostr_recent_notes.db"
     min_reactions = 2
-    db_since = 10 * 3600
-    db_name = "db/nostr_default_recent_notes.db"
-    search_list = []
-    avoid_list = []
-    must_list = []
     personalized = False
     result = ""
-    logger = False
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-
+        dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
-        # Generate Generic request form for dvms that provide generic results (e.g only a calculation per update,
-        # not per call)
         self.request_form = {"jobID": "generic"}
         opts = {
             "max_results": 200,
         }
         self.request_form['options'] = json.dumps(opts)
 
-        dvm_config.SCRIPT = os.path.abspath(__file__)
-        if self.options is not None:
-            if self.options.get("personalized"):
-                self.personalized = bool(self.options.get("personalized"))
-            self.last_schedule = Timestamp.now().as_secs()
-            if self.options.get("search_list"):
-                self.search_list = self.options.get("search_list")
-                # print(self.search_list)
-            if self.options.get("avoid_list"):
-                self.avoid_list = self.options.get("avoid_list")
-            if self.options.get("must_list"):
-                self.must_list = self.options.get("must_list")
-            if self.options.get("db_name"):
-                self.db_name = self.options.get("db_name")
-            if self.options.get("db_since"):
-                self.db_since = int(self.options.get("db_since"))
-            if self.options.get("logger"):
-                self.logger = bool(self.options.get("logger"))
-
-            if self.logger:
-                init_logger(LogLevel.DEBUG)
-
-        relaylimits = RelayLimits.disable()
-        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=dvm_config.RELAY_LONG_TIMEOUT))
-                .relay_limits(relaylimits))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite(self.db_name)
-        self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
+        self.last_schedule = Timestamp.now().as_secs()
 
-        #self.client.add_relay("wss://relay.damus.io")
-        #self.client.add_relay("wss://nostr.oxtr.dev")
+        if self.options.get("db_name"):
+            self.db_name = self.options.get("db_name")
+        if self.options.get("db_since"):
+            self.db_since = int(self.options.get("db_since"))
 
-        ropts = RelayOptions().ping(False)
-        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
-        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
-        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
 
-        self.client.connect()
+        use_logger = False
+        if use_logger:
+            init_logger(LogLevel.DEBUG)
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
+
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
+
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
+        search = ""
         max_results = 200
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
             elif tag.as_vec()[0] == 'param':
                 param = tag.as_vec()[1]
                 if param == "max_results":  # check for param type
                     max_results = int(tag.as_vec()[2])
 
         options = {
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
-        self.request_form = request_form
         return request_form
 
     def process(self, request_form):
         # if the dvm supports individual results, recalculate it every time for the request
         if self.personalized:
             return self.calculate_result(request_form)
-        # else return the result that gets updated once every schenduled update. In this case on database update.
+        # else return the result that gets updated once every scheduled update. In this case on database update.
         else:
             return self.result
 
-    def post_process(self, result, event):
-        """Overwrite the interface function to return a social client readable format, if requested"""
-        for tag in event.tags():
-            if tag.as_vec()[0] == 'output':
-                format = tag.as_vec()[1]
-                if format == "text/plain":  # check for output type
-                    result = post_process_list_to_events(result)
-
-        # if not text/plain, don't post-process
-        return result
-
     def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = self.set_options(request_form)
 
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
+        cli.connect()
 
-        timestamp_since = Timestamp.now().as_secs() - self.db_since
-        since = Timestamp.from_secs(timestamp_since)
+        # Negentropy reconciliation
+        # Query events from database
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
+        since = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(since)
-
-        events = self.client.database().query([filter1])
+        events = cli.database().query([filter1])
         print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
-
-        ns.final_list = {}
-
+        ns.finallist = {}
         for event in events:
-            if all(ele in event.content().lower() for ele in self.must_list):
-                if any(ele in event.content().lower() for ele in self.search_list):
-                    if not any(ele in event.content().lower() for ele in self.avoid_list):
-
-                        filt = Filter().kinds(
-                            [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION,
-                             definitions.EventDefinitions.KIND_REPOST,
-                             definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
-                        reactions = self.client.database().query([filt])
-                        if len(reactions) >= self.min_reactions:
-                            ns.final_list[event.id().to_hex()] = len(reactions)
+            if event.created_at().as_secs() > timestamp_hour_ago:
+                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
+                                       definitions.EventDefinitions.KIND_REACTION,
+                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
+                reactions = cli.database().query([filt])
+                if len(reactions) >= self.min_reactions:
+                    ns.finallist[event.id().to_hex()] = len(reactions)
+        if len(ns.finallist) == 0:
+            cli.disconnect()
+            cli.shutdown()
+            return self.result
 
         result_list = []
-        finallist_sorted = sorted(ns.final_list.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
+        finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
             # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
-
+        cli.disconnect()
+        cli.shutdown()
         return json.dumps(result_list)
 
+    def post_process(self, result, event):
+        """Overwrite the interface function to return a social client readable format, if requested"""
+        for tag in event.tags():
+            if tag.as_vec()[0] == 'output':
+                format = tag.as_vec()[1]
+                if format == "text/plain":  # check for output type
+                    result = post_process_list_to_events(result)
+
+        # if not text/plain, don't post-process
+        return result
+
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
-                try:
-                    if self.dvm_config.UPDATE_DATABASE:
-                        self.sync_db()
-                    self.last_schedule = Timestamp.now().as_secs()
-                    if not self.personalized:
-                        self.result = self.calculate_result(self.request_form)
-                except Exception as e:
-                    print(e)
+                if self.dvm_config.UPDATE_DATABASE:
+                    self.sync_db()
+                self.last_schedule = Timestamp.now().as_secs()
+                self.result = self.calculate_result(self.request_form)
                 return 1
 
     def sync_db(self):
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
+        keys = Keys.parse(sk.to_hex())
+        signer = NostrSigner.keys(keys)
+        database = NostrDatabase.sqlite(self.db_name)
+        cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
+        ropts = RelayOptions().ping(True)
+        cli.add_relay_with_opts("wss://relay.damus.io", ropts)
+        cli.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
+        cli.add_relay_with_opts("wss://nostr21.com", ropts)
+        cli.connect()
 
-        timestamp_since = Timestamp.now().as_secs() - self.db_since
-        since = Timestamp.from_secs(timestamp_since)
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
+        lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
-        filter1 = Filter().kinds([EventDefinitions.KIND_NOTE, EventDefinitions.KIND_REACTION, EventDefinitions.KIND_ZAP,
-                                  definitions.EventDefinitions.KIND_REPOST
-                                  ]).since(since)  # Notes, reactions, zaps
+        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
+                                  definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("[" + self.dvm_config.NIP89.NAME + "] Syncing notes of the last " + str(
+        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
             self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
-        self.client.reconcile(filter1, dbopts)
-        filter_delete = Filter().until(Timestamp.from_secs(Timestamp.now().as_secs() - self.db_since))
-        self.client.database().delete(filter_delete)  # Clear old events so db doesn't get too full.
+        cli.reconcile(filter1, dbopts)
+        database.delete(Filter().until(Timestamp.from_secs(
+            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
 
         print(
-            "[" + self.dvm_config.NIP89.NAME + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
+            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options, image, description, update_rate=600, cost=0,
-                  processing_msg=None, update_db=True):
+def build_example(name, identifier, admin_config, options,  cost=0, update_rate=180,  processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 10 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = cost
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
+    image = "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
+
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "picture": image,
-        "about": description,
+        "about": "I show notes that are currently popular",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "personalized": False,
         "amount": create_amount_tag(cost),
         "nip90Params": {
             "max_results": {
@@ -262,36 +244,40 @@
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                                 admin_config=admin_config, options=options)
+    #admin_config.UPDATE_PROFILE = False
+    #admin_config.REBROADCAST_NIP89 = False
+
+    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                          admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, image, description, processing_msg=None,
-                               update_db=True):
+def build_example_subscription(name, identifier, admin_config, options, update_rate=180, processing_msg=None, update_db=True):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
-    dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
+    dvm_config.SCHEDULE_UPDATES_SECONDS = update_rate  # Every 3 minutes
     dvm_config.UPDATE_DATABASE = update_db
     # Activate these to use a subscription based model instead
+    # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
     dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
+    image = "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "picture": image,
-        "about": description,
+        "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
         "personalized": False,
         "nip90Params": {
             "max_results": {
@@ -315,15 +301,22 @@
     nip88config.AMOUNT_DAILY = 100
     nip88config.AMOUNT_MONTHLY = 2000
     nip88config.CONTENT = "Subscribe to the DVM for unlimited use during your subscription"
     nip88config.PERK1DESC = "Unlimited requests"
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
-    return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                                 nip88config=nip88config,
-                                                 admin_config=admin_config,
-                                                 options=options)
+    #admin_config.UPDATE_PROFILE = False
+    #admin_config.REBROADCAST_NIP89 = False
+    #admin_config.REBROADCAST_NIP88 = False
+
+    # admin_config.FETCH_NIP88 = True
+    # admin_config.EVENTID = ""
+    # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
+
+    return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                          nip88config=nip88config, options=options,
+                                          admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(DicoverContentCurrentlyPopularbyTopic)
+    process_venv(DicoverContentCurrentlyPopular)
```

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.5.6/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.5.6/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.5.6/nostr_dvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.5
+Version: 0.5.6
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.5/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.5.6/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/setup.py` & `nostr_dvm-0.5.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.5'
+VERSION = '0.5.6'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.5.5/tests/test_dvm_client.py` & `nostr_dvm-0.5.6/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.5/tests/test_events.py` & `nostr_dvm-0.5.6/tests/test_events.py`

 * *Files identical despite different names*

