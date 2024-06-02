# Comparing `tmp/monai_weekly-1.4.dev2421.tar.gz` & `tmp/monai_weekly-1.4.dev2422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai_weekly-1.4.dev2421.tar", last modified: Sun May 26 02:17:50 2024, max compression
+gzip compressed data, was "monai_weekly-1.4.dev2422.tar", last modified: Sun Jun  2 02:18:21 2024, max compression
```

## Comparing `monai_weekly-1.4.dev2421.tar` & `monai_weekly-1.4.dev2422.tar`

### file list

```diff
@@ -1,1187 +1,1187 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.626570 monai_weekly-1.4.dev2421/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-26 02:17:50.626570 monai_weekly-1.4.dev2421/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.626570 monai_weekly-1.4.dev2421/monai/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-26 02:16:23.000000 monai_weekly-1.4.dev2421/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.422570 monai_weekly-1.4.dev2421/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.422570 monai_weekly-1.4.dev2421/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-26 02:17:50.626570 monai_weekly-1.4.dev2421/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.426570 monai_weekly-1.4.dev2421/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.430570 monai_weekly-1.4.dev2421/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.430570 monai_weekly-1.4.dev2421/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.430570 monai_weekly-1.4.dev2421/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.430570 monai_weekly-1.4.dev2421/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.434570 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.438570 monai_weekly-1.4.dev2421/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.442570 monai_weekly-1.4.dev2421/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.442570 monai_weekly-1.4.dev2421/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.442570 monai_weekly-1.4.dev2421/monai/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.450570 monai_weekly-1.4.dev2421/monai/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    79098 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    61767 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/ultrasound_confidence_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.450570 monai_weekly-1.4.dev2421/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.450570 monai_weekly-1.4.dev2421/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.450570 monai_weekly-1.4.dev2421/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.454570 monai_weekly-1.4.dev2421/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.458570 monai_weekly-1.4.dev2421/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.458570 monai_weekly-1.4.dev2421/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.462570 monai_weekly-1.4.dev2421/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/cldice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/perceptual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.466570 monai_weekly-1.4.dev2421/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/fid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/mmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.466570 monai_weekly-1.4.dev2421/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.470570 monai_weekly-1.4.dev2421/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/pos_embed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.474570 monai_weekly-1.4.dev2421/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.482570 monai_weekly-1.4.dev2421/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/nets/voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)    49645 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.482570 monai_weekly-1.4.dev2421/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.482570 monai_weekly-1.4.dev2421/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/lazy/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/lazy/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.486570 monai_weekly-1.4.dev2421/monai/transforms/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/regularization/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/regularization/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.490570 monai_weekly-1.4.dev2421/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/signal/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/signal/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.490570 monai_weekly-1.4.dev2421/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.490570 monai_weekly-1.4.dev2421/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.490570 monai_weekly-1.4.dev2421/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)    94942 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.494570 monai_weekly-1.4.dev2421/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/tf32.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.494570 monai_weekly-1.4.dev2421/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.614570 monai_weekly-1.4.dev2421/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 02:17:50.000000 monai_weekly-1.4.dev2421/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-26 02:17:50.626570 monai_weekly-1.4.dev2421/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:17:50.614570 monai_weekly-1.4.dev2421/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_adversarial_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_auto3dseg_bundlegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_push_to_hf_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cldice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_clip_intensity_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_clip_intensity_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_component_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_fid_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_mmd_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_multiscalessim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_conjugate_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_daf3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_diffusion_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_distance_transform_edt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_download_url_yandex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_freeze_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gdsdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hausdorff_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_and_generate_sampling_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_perceptual_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_quicknat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity_fixed_meand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_simulate_low_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_simulate_low_resolutiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity_fixed_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_fillemptyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_soft_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_spectral_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_squeeze_unsqueeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_sure_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_text_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_ultrasound_confidence_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_voxelmorph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_wsi_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_zarr_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-05-26 02:16:17.000000 monai_weekly-1.4.dev2421/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.649576 monai_weekly-1.4.dev2422/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-06-02 02:18:21.649576 monai_weekly-1.4.dev2422/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.649576 monai_weekly-1.4.dev2422/monai/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-06-02 02:16:54.000000 monai_weekly-1.4.dev2422/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.453575 monai_weekly-1.4.dev2422/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.453575 monai_weekly-1.4.dev2422/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 02:18:21.649576 monai_weekly-1.4.dev2422/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.453575 monai_weekly-1.4.dev2422/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28994 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27277 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35085 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41884 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26618 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17161 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53640 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.457575 monai_weekly-1.4.dev2422/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24519 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69282 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18732 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48001 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24948 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.461575 monai_weekly-1.4.dev2422/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37258 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25928 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11377 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.465575 monai_weekly-1.4.dev2422/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14452 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.469575 monai_weekly-1.4.dev2422/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41323 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.469575 monai_weekly-1.4.dev2422/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16151 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22895 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15747 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80520 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.469575 monai_weekly-1.4.dev2422/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.473575 monai_weekly-1.4.dev2422/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50102 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78691 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19483 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61774 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39856 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/ultrasound_confidence_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66686 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49478 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.477575 monai_weekly-1.4.dev2422/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23793 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.477575 monai_weekly-1.4.dev2422/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.477575 monai_weekly-1.4.dev2422/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34061 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.477575 monai_weekly-1.4.dev2422/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.481575 monai_weekly-1.4.dev2422/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22501 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22615 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.481575 monai_weekly-1.4.dev2422/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34219 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15566 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20386 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.485575 monai_weekly-1.4.dev2422/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/cldice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51627 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15460 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/perceptual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.489575 monai_weekly-1.4.dev2422/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/fid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46947 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.489575 monai_weekly-1.4.dev2422/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.493575 monai_weekly-1.4.dev2422/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11686 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/pos_embed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.493575 monai_weekly-1.4.dev2422/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28472 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.501575 monai_weekly-1.4.dev2422/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23963 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44775 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18210 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40671 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14435 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28684 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18664 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28290 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19289 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44811 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/nets/voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49645 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.501575 monai_weekly-1.4.dev2422/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.505575 monai_weekly-1.4.dev2422/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.505575 monai_weekly-1.4.dev2422/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74745 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60722 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.505575 monai_weekly-1.4.dev2422/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120755 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85059 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.505575 monai_weekly-1.4.dev2422/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25636 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.505575 monai_weekly-1.4.dev2422/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/lazy/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/lazy/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44998 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43042 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/regularization/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/regularization/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/signal/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/signal/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17856 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   183231 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131672 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31249 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21532 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.509575 monai_weekly-1.4.dev2422/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70600 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73114 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94942 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31121 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.513575 monai_weekly-1.4.dev2422/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19674 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15651 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25008 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/tf32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.513575 monai_weekly-1.4.dev2422/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.637576 monai_weekly-1.4.dev2422/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35640 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 02:18:21.000000 monai_weekly-1.4.dev2422/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-06-02 02:18:21.649576 monai_weekly-1.4.dev2422/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 02:18:21.637576 monai_weekly-1.4.dev2422/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_adversarial_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_auto3dseg_bundlegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13774 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_push_to_hf_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cldice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_clip_intensity_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9018 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_clip_intensity_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_component_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_fid_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_mmd_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_multiscalessim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_conjugate_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18867 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19446 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_daf3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_diffusion_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_distance_transform_edt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_download_url_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10839 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17289 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_freeze_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gdsdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hausdorff_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13200 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14054 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18977 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20257 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12549 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_and_generate_sampling_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23741 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12021 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_perceptual_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_quicknat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity_fixed_meand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_simulate_low_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_simulate_low_resolutiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity_fixed_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_fillemptyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_soft_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_spectral_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_squeeze_unsqueeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_sure_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_ultrasound_confidence_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_voxelmorph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_wsi_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26108 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_zarr_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81097 2024-06-02 02:16:50.000000 monai_weekly-1.4.dev2422/versioneer.py
```

### Comparing `monai_weekly-1.4.dev2421/LICENSE` & `monai_weekly-1.4.dev2422/LICENSE`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/PKG-INFO` & `monai_weekly-1.4.dev2422/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2421
+Version: 1.4.dev2422
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai_weekly-1.4.dev2421/README.md` & `monai_weekly-1.4.dev2422/README.md`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/__init__.py` & `monai_weekly-1.4.dev2422/monai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,8 +89,8 @@
     if hasattr(torch.cuda.device_count, "cache_clear"):
         torch.cuda.device_count.cache_clear()
 except BaseException:
     from .utils.misc import MONAIEnvVars
 
     if MONAIEnvVars.debug():
         raise
-__commit_id__ = "e5afa4341b18149ca8d44f680f669b33ab423722"
+__commit_id__ = "4029c422f1da84cdf5e4ce546dbff33245cbe025"
```

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/__init__.py` & `monai_weekly-1.4.dev2422/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm.cpp` & `monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm.h` & `monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cpu.cpp` & `monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cuda.cu` & `monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai_weekly-1.4.dev2422/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/_extensions/loader.py` & `monai_weekly-1.4.dev2422/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/__main__.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/auto_runner.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/auto_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/bundle_gen.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/bundle_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/data_analyzer.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/ensemble_builder.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/ensemble_builder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/hpo_gen.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/hpo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/transforms.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/auto3dseg/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/datasets.py` & `monai_weekly-1.4.dev2422/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepedit/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepedit/interaction.py` & `monai_weekly-1.4.dev2422/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepedit/transforms.py` & `monai_weekly-1.4.dev2422/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepgrow/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepgrow/dataset.py` & `monai_weekly-1.4.dev2422/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepgrow/interaction.py` & `monai_weekly-1.4.dev2422/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/deepgrow/transforms.py` & `monai_weekly-1.4.dev2422/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/metrics/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/metrics/coco.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/metrics/matching.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/networks/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/networks/retinanet_detector.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/networks/retinanet_network.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/transforms/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/transforms/array.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/transforms/box_ops.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/transforms/dictionary.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/ATSS_matcher.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/anchor_utils.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/box_coder.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/box_selector.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/detector_utils.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/hard_negative_sampler.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/detection/utils/predict_utils.py` & `monai_weekly-1.4.dev2422/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/mmars/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/mmars/mmars.py` & `monai_weekly-1.4.dev2422/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/mmars/model_desc.py` & `monai_weekly-1.4.dev2422/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nnunet/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nnunet/__main__.py` & `monai_weekly-1.4.dev2422/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nnunet/nnunetv2_runner.py` & `monai_weekly-1.4.dev2422/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nnunet/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nuclick/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/nuclick/transforms.py` & `monai_weekly-1.4.dev2422/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/engines/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/engines/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/handlers/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/handlers/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/inferers/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/inferers/inferer.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/losses/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/losses/hovernet_loss.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/metrics/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/metrics/lesion_froc.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/array.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/array.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/transforms/stain/dictionary.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/pathology/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/complex_utils.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/fastmri_reader.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/mri_utils.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/networks/nets/varnet.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/array.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/reconstruction/transforms/dictionary.py` & `monai_weekly-1.4.dev2422/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/tcia/__init__.py` & `monai_weekly-1.4.dev2422/monai/apps/tcia/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/tcia/label_desc.py` & `monai_weekly-1.4.dev2422/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/tcia/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/apps/utils.py` & `monai_weekly-1.4.dev2422/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/__init__.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/algo_gen.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/analyzer.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/operations.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/seg_summarizer.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/auto3dseg/utils.py` & `monai_weekly-1.4.dev2422/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/__init__.py` & `monai_weekly-1.4.dev2422/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/__main__.py` & `monai_weekly-1.4.dev2422/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/config_item.py` & `monai_weekly-1.4.dev2422/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/config_parser.py` & `monai_weekly-1.4.dev2422/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/properties.py` & `monai_weekly-1.4.dev2422/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/reference_resolver.py` & `monai_weekly-1.4.dev2422/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/scripts.py` & `monai_weekly-1.4.dev2422/monai/bundle/scripts.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/utils.py` & `monai_weekly-1.4.dev2422/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/bundle/workflows.py` & `monai_weekly-1.4.dev2422/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/config/__init__.py` & `monai_weekly-1.4.dev2422/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/config/deviceconfig.py` & `monai_weekly-1.4.dev2422/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/config/type_definitions.py` & `monai_weekly-1.4.dev2422/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/__init__.py` & `monai_weekly-1.4.dev2422/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/box_utils.py` & `monai_weekly-1.4.dev2422/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/csv_saver.py` & `monai_weekly-1.4.dev2422/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/dataloader.py` & `monai_weekly-1.4.dev2422/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/dataset.py` & `monai_weekly-1.4.dev2422/monai/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,23 +32,15 @@
 from torch.multiprocessing import Manager
 from torch.serialization import DEFAULT_PROTOCOL
 from torch.utils.data import Dataset as _TorchDataset
 from torch.utils.data import Subset
 
 from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import SUPPORTED_PICKLE_MOD, convert_tables_to_dicts, pickle_hashing
-from monai.transforms import (
-    Compose,
-    Randomizable,
-    RandomizableTrait,
-    Transform,
-    apply_transform,
-    convert_to_contiguous,
-    reset_ops_id,
-)
+from monai.transforms import Compose, Randomizable, RandomizableTrait, Transform, convert_to_contiguous, reset_ops_id
 from monai.utils import MAX_SEED, convert_to_tensor, get_seed, look_up_option, min_version, optional_import
 from monai.utils.misc import first
 
 if TYPE_CHECKING:
     from tqdm import tqdm
 
     has_tqdm = True
@@ -73,33 +65,37 @@
         [{                            {                            {
              'img': 'image1.nii.gz',      'img': 'image2.nii.gz',      'img': 'image3.nii.gz',
              'seg': 'label1.nii.gz',      'seg': 'label2.nii.gz',      'seg': 'label3.nii.gz',
              'extra': 123                 'extra': 456                 'extra': 789
          },                           },                           }]
     """
 
-    def __init__(self, data: Sequence, transform: Callable | None = None) -> None:
+    def __init__(self, data: Sequence, transform: Sequence[Callable] | Callable | None = None) -> None:
         """
         Args:
             data: input data to load and transform to generate dataset for model.
-            transform: a callable data transform on input data.
-
+            transform: a callable, sequence of callables or None. If transform is not
+            a `Compose` instance, it will be wrapped in a `Compose` instance. Sequences
+            of callables are applied in order and if `None` is passed, the data is returned as is.
         """
         self.data = data
-        self.transform: Any = transform
+        try:
+            self.transform = Compose(transform) if not isinstance(transform, Compose) else transform
+        except Exception as e:
+            raise ValueError("`transform` must be a callable or a list of callables that is Composable") from e
 
     def __len__(self) -> int:
         return len(self.data)
 
     def _transform(self, index: int):
         """
         Fetch single data item from `self.data`.
         """
         data_i = self.data[index]
-        return apply_transform(self.transform, data_i) if self.transform is not None else data_i
+        return self.transform(data_i)
 
     def __getitem__(self, index: int | slice | Sequence[int]):
         """
         Returns a `Subset` if `index` is a slice or Sequence, a data item otherwise.
         """
         if isinstance(index, slice):
             # dataset[:42]
@@ -260,16 +256,14 @@
                 Other options are `pickle_hashing` and `json_hashing` functions from `monai.data.utils`.
             reset_ops_id: whether to set `TraceKeys.ID` to ``Tracekys.NONE``, defaults to ``True``.
                 When this is enabled, the traced transform instance IDs will be removed from the cached MetaTensors.
                 This is useful for skipping the transform instance checks when inverting applied operations
                 using the cached content and with re-created transform instances.
 
         """
-        if not isinstance(transform, Compose):
-            transform = Compose(transform)
         super().__init__(data=data, transform=transform)
         self.cache_dir = Path(cache_dir) if cache_dir is not None else None
         self.hash_func = hash_func
         self.pickle_module = pickle_module
         self.pickle_protocol = pickle_protocol
         if self.cache_dir is not None:
             if not self.cache_dir.exists():
@@ -319,17 +313,14 @@
             item_transformed: The data to be transformed
 
         Returns:
             the transformed element up to the first identified
             random transform object
 
         """
-        if not isinstance(self.transform, Compose):
-            raise ValueError("transform must be an instance of monai.transforms.Compose.")
-
         first_random = self.transform.get_index_of_first(
             lambda t: isinstance(t, RandomizableTrait) or not isinstance(t, Transform)
         )
         item_transformed = self.transform(item_transformed, end=first_random, threading=True)
 
         if self.reset_ops_id:
             reset_ops_id(item_transformed)
@@ -342,17 +333,14 @@
         Args:
             item_transformed: The data to be transformed (already processed up to the first random transform)
 
         Returns:
             the transformed element through the random transforms
 
         """
-        if not isinstance(self.transform, Compose):
-            raise ValueError("transform must be an instance of monai.transforms.Compose.")
-
         first_random = self.transform.get_index_of_first(
             lambda t: isinstance(t, RandomizableTrait) or not isinstance(t, Transform)
         )
         if first_random is not None:
             item_transformed = self.transform(item_transformed, start=first_random)
         return item_transformed
 
@@ -497,17 +485,14 @@
 
         Args:
             item_transformed: The data to be transformed
 
         Returns:
             the transformed element up to the N transform object
         """
-        if not isinstance(self.transform, Compose):
-            raise ValueError("transform must be an instance of monai.transforms.Compose.")
-
         item_transformed = self.transform(item_transformed, end=self.cache_n_trans, threading=True)
 
         reset_ops_id(item_transformed)
         return item_transformed
 
     def _post_transform(self, item_transformed):
         """
@@ -515,17 +500,14 @@
 
         Args:
             item_transformed: The data to be transformed (already processed up to the first N transform)
 
         Returns:
             the final transformed result
         """
-        if not isinstance(self.transform, Compose):
-            raise ValueError("transform must be an instance of monai.transforms.Compose.")
-
         return self.transform(item_transformed, start=self.cache_n_trans)
 
 
 class LMDBDataset(PersistentDataset):
     """
     Extension of `PersistentDataset` using LMDB as the backend.
 
@@ -805,16 +787,14 @@
                 For single process workflows with multiprocessing data loading, option 2 is recommended.
                 For multiprocessing workflows (typically for distributed training),
                 where this class is initialized in subprocesses, option 3 is recommended,
                 and the list-like object should be prepared in the main process and passed to all subprocesses.
                 Not following these recommendations may lead to runtime errors or duplicated cache across processes.
 
         """
-        if not isinstance(transform, Compose):
-            transform = Compose(transform)
         super().__init__(data=data, transform=transform)
         self.set_num = cache_num  # tracking the user-provided `cache_num` option
         self.set_rate = cache_rate  # tracking the user-provided `cache_rate` option
         self.progress = progress
         self.copy_cache = copy_cache
         self.as_contiguous = as_contiguous
         self.hash_as_key = hash_as_key
@@ -1278,16 +1258,18 @@
 
         def to_list(x):
             return list(x) if isinstance(x, (tuple, list)) else [x]
 
         data = []
         for dataset in self.data:
             data.extend(to_list(dataset[index]))
+
         if self.transform is not None:
-            data = apply_transform(self.transform, data, map_items=False)  # transform the list data
+            self.transform.map_items = False  # Compose object map_items to false so transform is applied to list
+            data = self.transform(data)
         # use tuple instead of list as the default collate_fn callback of MONAI DataLoader flattens nested lists
         return tuple(data)
 
 
 class ArrayDataset(Randomizable, _TorchDataset):
     """
     Dataset for segmentation and classification tasks based on array format input data and transforms.
@@ -1428,23 +1410,19 @@
         super().__init__([], transform)
 
     def __len__(self):
         return self.length
 
     def _transform(self, index: int):
         data = {k: v[index] for k, v in self.arrays.items()}
-
-        if not self.transform:
-            return data
-
-        result = apply_transform(self.transform, data)
+        result = self.transform(data) if self.transform is not None else data
 
         if isinstance(result, dict) or (isinstance(result, list) and isinstance(result[0], dict)):
             return result
-        raise AssertionError("With a dict supplied to apply_transform, should return a dict or a list of dicts.")
+        raise AssertionError("With a dict supplied to Compose, should return a dict or a list of dicts.")
 
 
 class CSVDataset(Dataset):
     """
     Dataset to load data from CSV files and generate a list of dictionaries,
     every dictionary maps to a row of the CSV file, and the keys of dictionary
     map to the column names of the CSV file.
```

### Comparing `monai_weekly-1.4.dev2421/monai/data/dataset_summary.py` & `monai_weekly-1.4.dev2422/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/decathlon_datalist.py` & `monai_weekly-1.4.dev2422/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/fft_utils.py` & `monai_weekly-1.4.dev2422/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/folder_layout.py` & `monai_weekly-1.4.dev2422/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/grid_dataset.py` & `monai_weekly-1.4.dev2422/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/image_dataset.py` & `monai_weekly-1.4.dev2422/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/image_reader.py` & `monai_weekly-1.4.dev2422/monai/data/image_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,15 +1327,15 @@
 
             if self.affine_lps_to_ras:
                 header = self._switch_lps_ras(header)
             if header.get(MetaKeys.SPACE, "left-posterior-superior") == "left-posterior-superior":
                 header[MetaKeys.SPACE] = SpaceKeys.LPS  # assuming LPS if not specified
 
             header[MetaKeys.AFFINE] = header[MetaKeys.ORIGINAL_AFFINE].copy()
-            header[MetaKeys.SPATIAL_SHAPE] = header["sizes"]
+            header[MetaKeys.SPATIAL_SHAPE] = header["sizes"].copy()
             [header.pop(k) for k in ("sizes", "space origin", "space directions")]  # rm duplicated data in header
 
             if self.channel_dim is None:  # default to "no_channel" or -1
                 header[MetaKeys.ORIGINAL_CHANNEL_DIM] = (
                     float("nan") if len(data.shape) == len(header[MetaKeys.SPATIAL_SHAPE]) else 0
                 )
             else:
```

### Comparing `monai_weekly-1.4.dev2421/monai/data/image_writer.py` & `monai_weekly-1.4.dev2422/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/iterable_dataset.py` & `monai_weekly-1.4.dev2422/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/itk_torch_bridge.py` & `monai_weekly-1.4.dev2422/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/meta_obj.py` & `monai_weekly-1.4.dev2422/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/meta_tensor.py` & `monai_weekly-1.4.dev2422/monai/data/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/samplers.py` & `monai_weekly-1.4.dev2422/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/synthetic.py` & `monai_weekly-1.4.dev2422/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/test_time_augmentation.py` & `monai_weekly-1.4.dev2422/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/thread_buffer.py` & `monai_weekly-1.4.dev2422/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/torchscript_utils.py` & `monai_weekly-1.4.dev2422/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/ultrasound_confidence_map.py` & `monai_weekly-1.4.dev2422/monai/data/ultrasound_confidence_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/utils.py` & `monai_weekly-1.4.dev2422/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/video_dataset.py` & `monai_weekly-1.4.dev2422/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/wsi_datasets.py` & `monai_weekly-1.4.dev2422/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/data/wsi_reader.py` & `monai_weekly-1.4.dev2422/monai/data/wsi_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/engines/__init__.py` & `monai_weekly-1.4.dev2422/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/engines/evaluator.py` & `monai_weekly-1.4.dev2422/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/engines/trainer.py` & `monai_weekly-1.4.dev2422/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/engines/utils.py` & `monai_weekly-1.4.dev2422/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/engines/workflow.py` & `monai_weekly-1.4.dev2422/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/__init__.py` & `monai_weekly-1.4.dev2422/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/client/__init__.py` & `monai_weekly-1.4.dev2422/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/client/client_algo.py` & `monai_weekly-1.4.dev2422/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/client/monai_algo.py` & `monai_weekly-1.4.dev2422/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/utils/__init__.py` & `monai_weekly-1.4.dev2422/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/utils/constants.py` & `monai_weekly-1.4.dev2422/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/utils/exchange_object.py` & `monai_weekly-1.4.dev2422/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/fl/utils/filters.py` & `monai_weekly-1.4.dev2422/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/__init__.py` & `monai_weekly-1.4.dev2422/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/checkpoint_loader.py` & `monai_weekly-1.4.dev2422/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/checkpoint_saver.py` & `monai_weekly-1.4.dev2422/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/classification_saver.py` & `monai_weekly-1.4.dev2422/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/clearml_handlers.py` & `monai_weekly-1.4.dev2422/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/confusion_matrix.py` & `monai_weekly-1.4.dev2422/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/decollate_batch.py` & `monai_weekly-1.4.dev2422/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/earlystop_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/garbage_collector.py` & `monai_weekly-1.4.dev2422/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/hausdorff_distance.py` & `monai_weekly-1.4.dev2422/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/ignite_metric.py` & `monai_weekly-1.4.dev2422/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/logfile_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/lr_schedule_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/mean_dice.py` & `monai_weekly-1.4.dev2422/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/mean_iou.py` & `monai_weekly-1.4.dev2422/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/metric_logger.py` & `monai_weekly-1.4.dev2422/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/metrics_reloaded_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/metrics_saver.py` & `monai_weekly-1.4.dev2422/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/mlflow_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/nvtx_handlers.py` & `monai_weekly-1.4.dev2422/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/panoptic_quality.py` & `monai_weekly-1.4.dev2422/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/parameter_scheduler.py` & `monai_weekly-1.4.dev2422/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/postprocessing.py` & `monai_weekly-1.4.dev2422/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/probability_maps.py` & `monai_weekly-1.4.dev2422/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/regression_metrics.py` & `monai_weekly-1.4.dev2422/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/roc_auc.py` & `monai_weekly-1.4.dev2422/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/smartcache_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/stats_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/surface_distance.py` & `monai_weekly-1.4.dev2422/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/tensorboard_handlers.py` & `monai_weekly-1.4.dev2422/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/utils.py` & `monai_weekly-1.4.dev2422/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/handlers/validation_handler.py` & `monai_weekly-1.4.dev2422/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/inferers/__init__.py` & `monai_weekly-1.4.dev2422/monai/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/inferers/inferer.py` & `monai_weekly-1.4.dev2422/monai/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/inferers/merger.py` & `monai_weekly-1.4.dev2422/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/inferers/splitter.py` & `monai_weekly-1.4.dev2422/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/inferers/utils.py` & `monai_weekly-1.4.dev2422/monai/inferers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/__init__.py` & `monai_weekly-1.4.dev2422/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/adversarial_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/barlow_twins.py` & `monai_weekly-1.4.dev2422/monai/losses/barlow_twins.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/cldice.py` & `monai_weekly-1.4.dev2422/monai/losses/cldice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/contrastive.py` & `monai_weekly-1.4.dev2422/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/deform.py` & `monai_weekly-1.4.dev2422/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/dice.py` & `monai_weekly-1.4.dev2422/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/ds_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/focal_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/giou_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/hausdorff_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/hausdorff_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/image_dissimilarity.py` & `monai_weekly-1.4.dev2422/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/multi_scale.py` & `monai_weekly-1.4.dev2422/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/perceptual.py` & `monai_weekly-1.4.dev2422/monai/losses/perceptual.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/spatial_mask.py` & `monai_weekly-1.4.dev2422/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/spectral_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/ssim_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/sure_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/tversky.py` & `monai_weekly-1.4.dev2422/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/losses/unified_focal_loss.py` & `monai_weekly-1.4.dev2422/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/__init__.py` & `monai_weekly-1.4.dev2422/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/active_learning_metrics.py` & `monai_weekly-1.4.dev2422/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/confusion_matrix.py` & `monai_weekly-1.4.dev2422/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/cumulative_average.py` & `monai_weekly-1.4.dev2422/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/f_beta_score.py` & `monai_weekly-1.4.dev2422/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/fid.py` & `monai_weekly-1.4.dev2422/monai/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/froc.py` & `monai_weekly-1.4.dev2422/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/generalized_dice.py` & `monai_weekly-1.4.dev2422/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/hausdorff_distance.py` & `monai_weekly-1.4.dev2422/monai/metrics/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/loss_metric.py` & `monai_weekly-1.4.dev2422/monai/metrics/loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/meandice.py` & `monai_weekly-1.4.dev2422/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/meaniou.py` & `monai_weekly-1.4.dev2422/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/metric.py` & `monai_weekly-1.4.dev2422/monai/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/mmd.py` & `monai_weekly-1.4.dev2422/monai/metrics/mmd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/panoptic_quality.py` & `monai_weekly-1.4.dev2422/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/regression.py` & `monai_weekly-1.4.dev2422/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/rocauc.py` & `monai_weekly-1.4.dev2422/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/surface_dice.py` & `monai_weekly-1.4.dev2422/monai/metrics/surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/surface_distance.py` & `monai_weekly-1.4.dev2422/monai/metrics/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/utils.py` & `monai_weekly-1.4.dev2422/monai/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/metrics/wrapper.py` & `monai_weekly-1.4.dev2422/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/__init__.py` & `monai_weekly-1.4.dev2422/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/__init__.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/acti_norm.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/activation.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/aspp.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/backbone_fpn_utils.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/convolutions.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/crf.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/denseblock.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/dints_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/downsample.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/dynunet_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/encoder.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/fcn.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/feature_pyramid_network.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/fft_utils_t.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/localnet_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/mlp.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/patchembedding.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/pos_embed_utils.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/pos_embed_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/regunet_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/segresnet_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/selfattention.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/selfattention.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/squeeze_and_excitation.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/text_embedding.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/text_embedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/transformerblock.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/unetr_block.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/upsample.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/blocks/warp.py` & `monai_weekly-1.4.dev2422/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/__init__.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/conjugate_gradient.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/convutils.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/drop_path.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/factories.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/filtering.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/gmm.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/simplelayers.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/spatial_transforms.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/utils.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/layers/weight_init.py` & `monai_weekly-1.4.dev2422/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/__init__.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/ahnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/attentionunet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/autoencoder.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/basic_unet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/basic_unetplusplus.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/classifier.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/daf3d.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/densenet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/dints.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/dynunet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/efficientnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/flexible_unet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/fullyconnectednet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/generator.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/highresnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/hovernet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/milmodel.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/netadapter.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/quicknat.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/regressor.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/regunet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/resnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,21 +90,20 @@
             downsample: which downsample layer to use.
             act: activation type and arguments. Defaults to relu.
             norm: feature normalization type and arguments. Defaults to batch norm.
         """
         super().__init__()
 
         conv_type: Callable = Conv[Conv.CONV, spatial_dims]
-        norm_layer = get_norm_layer(name=norm, spatial_dims=spatial_dims, channels=planes)
 
         self.conv1 = conv_type(in_planes, planes, kernel_size=3, padding=1, stride=stride, bias=False)
-        self.bn1 = norm_layer
+        self.bn1 = get_norm_layer(name=norm, spatial_dims=spatial_dims, channels=planes)
         self.act = get_act_layer(name=act)
         self.conv2 = conv_type(planes, planes, kernel_size=3, padding=1, bias=False)
-        self.bn2 = norm_layer
+        self.bn2 = get_norm_layer(name=norm, spatial_dims=spatial_dims, channels=planes)
         self.downsample = downsample
         self.stride = stride
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         residual = x
 
         out: torch.Tensor = self.conv1(x)
```

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/segresnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/segresnet_ds.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/senet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/swin_unetr.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/torchvision_fc.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/transchex.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/unet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/unetr.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/varautoencoder.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/vit.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/vit.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/vitautoenc.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/vnet.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/nets/voxelmorph.py` & `monai_weekly-1.4.dev2422/monai/networks/nets/voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/networks/utils.py` & `monai_weekly-1.4.dev2422/monai/networks/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/optimizers/__init__.py` & `monai_weekly-1.4.dev2422/monai/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/optimizers/lr_finder.py` & `monai_weekly-1.4.dev2422/monai/optimizers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/optimizers/lr_scheduler.py` & `monai_weekly-1.4.dev2422/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/optimizers/novograd.py` & `monai_weekly-1.4.dev2422/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/optimizers/utils.py` & `monai_weekly-1.4.dev2422/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/adaptors.py` & `monai_weekly-1.4.dev2422/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/compose.py` & `monai_weekly-1.4.dev2422/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/croppad/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/croppad/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/croppad/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/croppad/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/croppad/batch.py` & `monai_weekly-1.4.dev2422/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/croppad/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/croppad/functional.py` & `monai_weekly-1.4.dev2422/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/intensity/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/intensity/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/intensity/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/inverse.py` & `monai_weekly-1.4.dev2422/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/inverse_batch_transform.py` & `monai_weekly-1.4.dev2422/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/io/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/io/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/io/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/lazy/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/lazy/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/lazy/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/lazy/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/lazy/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/lazy/functional.py` & `monai_weekly-1.4.dev2422/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/lazy/utils.py` & `monai_weekly-1.4.dev2422/monai/transforms/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/meta_utility/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/meta_utility/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/nvtx.py` & `monai_weekly-1.4.dev2422/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/post/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/post/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/post/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/regularization/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/regularization/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/regularization/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/regularization/array.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from math import ceil, sqrt
 
 import torch
 
+from monai.data.meta_obj import get_track_meta
+from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
+
 from ..transform import RandomizableTransform
 
 __all__ = ["MixUp", "CutMix", "CutOut", "Mixer"]
 
 
 class Mixer(RandomizableTransform):
 
@@ -49,46 +52,55 @@
     def randomize(self, data=None) -> None:
         """
         Sometimes you need may to apply the same transform to different tensors.
         The idea is to get a sample and then apply it with apply() as often
         as needed. You need to call this method everytime you apply the transform to a new
         batch.
         """
+        super().randomize(None)
         self._params = (
             torch.from_numpy(self.R.beta(self.alpha, self.alpha, self.batch_size)).type(torch.float32),
             self.R.permutation(self.batch_size),
+            [torch.from_numpy(self.R.randint(0, d, size=(1,))) for d in data.shape[2:]] if data is not None else [],
         )
 
 
 class MixUp(Mixer):
     """MixUp as described in:
     Hongyi Zhang, Moustapha Cisse, Yann N. Dauphin, David Lopez-Paz.
     mixup: Beyond Empirical Risk Minimization, ICLR 2018
 
     Class derived from :py:class:`monai.transforms.Mixer`. See corresponding
     documentation for details on the constructor parameters.
     """
 
     def apply(self, data: torch.Tensor):
-        weight, perm = self._params
+        weight, perm, _ = self._params
         nsamples, *dims = data.shape
         if len(weight) != nsamples:
             raise ValueError(f"Expected batch of size: {len(weight)}, but got {nsamples}")
 
         if len(dims) not in [3, 4]:
             raise ValueError("Unexpected number of dimensions")
 
         mixweight = weight[(Ellipsis,) + (None,) * len(dims)]
         return mixweight * data + (1 - mixweight) * data[perm, ...]
 
-    def __call__(self, data: torch.Tensor, labels: torch.Tensor | None = None):
-        self.randomize()
+    def __call__(self, data: torch.Tensor, labels: torch.Tensor | None = None, randomize=True):
+        data_t = convert_to_tensor(data, track_meta=get_track_meta())
+        if labels is not None:
+            labels_t = convert_to_tensor(labels, track_meta=get_track_meta())
+        if randomize:
+            self.randomize()
         if labels is None:
-            return self.apply(data)
-        return self.apply(data), self.apply(labels)
+            return convert_to_dst_type(self.apply(data_t), dst=data)[0]
+        return (
+            convert_to_dst_type(self.apply(data_t), dst=data)[0],
+            convert_to_dst_type(self.apply(labels_t), dst=labels)[0],
+        )
 
 
 class CutMix(Mixer):
     """CutMix augmentation as described in:
         Sangdoo Yun, Dongyoon Han, Seong Joon Oh, Sanghyuk Chun, Junsuk Choe, Youngjoon Yoo.
         CutMix: Regularization Strategy to Train Strong Classifiers with Localizable Features,
         ICCV 2019
@@ -109,41 +121,46 @@
             output = model(augimg)
             loss = loss_function(output, auglabels)
             ...
 
     """
 
     def apply(self, data: torch.Tensor):
-        weights, perm = self._params
+        weights, perm, coords = self._params
         nsamples, _, *dims = data.shape
         if len(weights) != nsamples:
             raise ValueError(f"Expected batch of size: {len(weights)}, but got {nsamples}")
 
         mask = torch.ones_like(data)
         for s, weight in enumerate(weights):
-            coords = [torch.randint(0, d, size=(1,)) for d in dims]
             lengths = [d * sqrt(1 - weight) for d in dims]
             idx = [slice(None)] + [slice(c, min(ceil(c + ln), d)) for c, ln, d in zip(coords, lengths, dims)]
             mask[s][idx] = 0
 
         return mask * data + (1 - mask) * data[perm, ...]
 
     def apply_on_labels(self, labels: torch.Tensor):
-        weights, perm = self._params
+        weights, perm, _ = self._params
         nsamples, *dims = labels.shape
         if len(weights) != nsamples:
             raise ValueError(f"Expected batch of size: {len(weights)}, but got {nsamples}")
 
         mixweight = weights[(Ellipsis,) + (None,) * len(dims)]
         return mixweight * labels + (1 - mixweight) * labels[perm, ...]
 
-    def __call__(self, data: torch.Tensor, labels: torch.Tensor | None = None):
-        self.randomize()
-        augmented = self.apply(data)
-        return (augmented, self.apply_on_labels(labels)) if labels is not None else augmented
+    def __call__(self, data: torch.Tensor, labels: torch.Tensor | None = None, randomize=True):
+        data_t = convert_to_tensor(data, track_meta=get_track_meta())
+        if labels is not None:
+            labels_t = convert_to_tensor(labels, track_meta=get_track_meta())
+        if randomize:
+            self.randomize(data)
+        augmented = convert_to_dst_type(self.apply(data_t), dst=data)[0]
+        if labels is not None:
+            augmented_label = convert_to_dst_type(self.apply(labels_t), dst=labels)[0]
+        return (augmented, augmented_label) if labels is not None else augmented
 
 
 class CutOut(Mixer):
     """Cutout as described in the paper:
     Terrance DeVries, Graham W. Taylor.
     Improved Regularization of Convolutional Neural Networks with Cutout,
     arXiv:1708.04552
@@ -151,24 +168,25 @@
     Class derived from :py:class:`monai.transforms.Mixer`. See corresponding
     documentation for details on the constructor parameters. Here, alpha not only determines
     the mixing weight but also the size of the random rectangles being cut put.
     Please refer to the paper for details.
     """
 
     def apply(self, data: torch.Tensor):
-        weights, _ = self._params
+        weights, _, coords = self._params
         nsamples, _, *dims = data.shape
         if len(weights) != nsamples:
             raise ValueError(f"Expected batch of size: {len(weights)}, but got {nsamples}")
 
         mask = torch.ones_like(data)
         for s, weight in enumerate(weights):
-            coords = [torch.randint(0, d, size=(1,)) for d in dims]
             lengths = [d * sqrt(1 - weight) for d in dims]
             idx = [slice(None)] + [slice(c, min(ceil(c + ln), d)) for c, ln, d in zip(coords, lengths, dims)]
             mask[s][idx] = 0
 
         return mask * data
 
-    def __call__(self, data: torch.Tensor):
-        self.randomize()
-        return self.apply(data)
+    def __call__(self, data: torch.Tensor, randomize=True):
+        data_t = convert_to_tensor(data, track_meta=get_track_meta())
+        if randomize:
+            self.randomize(data)
+        return convert_to_dst_type(self.apply(data_t), dst=data)[0]
```

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/regularization/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/regularization/dictionary.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,46 +7,59 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from collections.abc import Hashable
+
+import numpy as np
+
 from monai.config import KeysCollection
+from monai.config.type_definitions import NdarrayOrTensor
+from monai.data.meta_obj import get_track_meta
+from monai.utils import convert_to_tensor
 from monai.utils.misc import ensure_tuple
 
-from ..transform import MapTransform
+from ..transform import MapTransform, RandomizableTransform
 from .array import CutMix, CutOut, MixUp
 
 __all__ = ["MixUpd", "MixUpD", "MixUpDict", "CutMixd", "CutMixD", "CutMixDict", "CutOutd", "CutOutD", "CutOutDict"]
 
 
-class MixUpd(MapTransform):
+class MixUpd(MapTransform, RandomizableTransform):
     """
     Dictionary-based version :py:class:`monai.transforms.MixUp`.
 
     Notice that the mixup transformation will be the same for all entries
     for consistency, i.e. images and labels must be applied the same augmenation.
     """
 
     def __init__(
         self, keys: KeysCollection, batch_size: int, alpha: float = 1.0, allow_missing_keys: bool = False
     ) -> None:
-        super().__init__(keys, allow_missing_keys)
+        MapTransform.__init__(self, keys, allow_missing_keys)
         self.mixup = MixUp(batch_size, alpha)
 
+    def set_random_state(self, seed: int | None = None, state: np.random.RandomState | None = None) -> MixUpd:
+        super().set_random_state(seed, state)
+        self.mixup.set_random_state(seed, state)
+        return self
+
     def __call__(self, data):
-        self.mixup.randomize()
-        result = dict(data)
-        for k in self.keys:
-            result[k] = self.mixup.apply(data[k])
-        return result
+        d = dict(data)
+        # all the keys share the same random state
+        self.mixup.randomize(None)
+        for k in self.key_iterator(d):
+            d[k] = self.mixup(data[k], randomize=False)
+        return d
 
 
-class CutMixd(MapTransform):
+class CutMixd(MapTransform, RandomizableTransform):
     """
     Dictionary-based version :py:class:`monai.transforms.CutMix`.
 
     Notice that the mixture weights will be the same for all entries
     for consistency, i.e. images and labels must be aggregated with the same weights,
     but the random crops are not.
     """
@@ -59,39 +72,58 @@
         alpha: float = 1.0,
         allow_missing_keys: bool = False,
     ) -> None:
         super().__init__(keys, allow_missing_keys)
         self.mixer = CutMix(batch_size, alpha)
         self.label_keys = ensure_tuple(label_keys) if label_keys is not None else []
 
+    def set_random_state(self, seed: int | None = None, state: np.random.RandomState | None = None) -> CutMixd:
+        super().set_random_state(seed, state)
+        self.mixer.set_random_state(seed, state)
+        return self
+
     def __call__(self, data):
-        self.mixer.randomize()
-        result = dict(data)
-        for k in self.keys:
-            result[k] = self.mixer.apply(data[k])
-        for k in self.label_keys:
-            result[k] = self.mixer.apply_on_labels(data[k])
-        return result
+        d = dict(data)
+        first_key: Hashable = self.first_key(d)
+        if first_key == ():
+            out: dict[Hashable, NdarrayOrTensor] = convert_to_tensor(d, track_meta=get_track_meta())
+            return out
+        self.mixer.randomize(d[first_key])
+        for key, label_key in self.key_iterator(d, self.label_keys):
+            ret = self.mixer(data[key], data.get(label_key, None), randomize=False)
+            d[key] = ret[0]
+            if label_key in d:
+                d[label_key] = ret[1]
+        return d
 
 
-class CutOutd(MapTransform):
+class CutOutd(MapTransform, RandomizableTransform):
     """
     Dictionary-based version :py:class:`monai.transforms.CutOut`.
 
     Notice that the cutout is different for every entry in the dictionary.
     """
 
     def __init__(self, keys: KeysCollection, batch_size: int, allow_missing_keys: bool = False) -> None:
         super().__init__(keys, allow_missing_keys)
         self.cutout = CutOut(batch_size)
 
+    def set_random_state(self, seed: int | None = None, state: np.random.RandomState | None = None) -> CutOutd:
+        super().set_random_state(seed, state)
+        self.cutout.set_random_state(seed, state)
+        return self
+
     def __call__(self, data):
-        result = dict(data)
-        self.cutout.randomize()
-        for k in self.keys:
-            result[k] = self.cutout(data[k])
-        return result
+        d = dict(data)
+        first_key: Hashable = self.first_key(d)
+        if first_key == ():
+            out: dict[Hashable, NdarrayOrTensor] = convert_to_tensor(d, track_meta=get_track_meta())
+            return out
+        self.cutout.randomize(d[first_key])
+        for k in self.key_iterator(d):
+            d[k] = self.cutout(data[k], randomize=False)
+        return d
 
 
 MixUpD = MixUpDict = MixUpd
 CutMixD = CutMixDict = CutMixd
 CutOutD = CutOutDict = CutOutd
```

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/signal/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/signal/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/signal/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/signal/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/smooth_field/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/smooth_field/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/smooth_field/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/spatial/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/spatial/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/spatial/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/spatial/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/spatial/functional.py` & `monai_weekly-1.4.dev2422/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/traits.py` & `monai_weekly-1.4.dev2422/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/transform.py` & `monai_weekly-1.4.dev2422/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utility/__init__.py` & `monai_weekly-1.4.dev2422/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utility/array.py` & `monai_weekly-1.4.dev2422/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utility/dictionary.py` & `monai_weekly-1.4.dev2422/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utils.py` & `monai_weekly-1.4.dev2422/monai/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utils_create_transform_ims.py` & `monai_weekly-1.4.dev2422/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/transforms/utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2422/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/__init__.py` & `monai_weekly-1.4.dev2422/monai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/aliases.py` & `monai_weekly-1.4.dev2422/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/component_store.py` & `monai_weekly-1.4.dev2422/monai/utils/component_store.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/decorators.py` & `monai_weekly-1.4.dev2422/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/deprecate_utils.py` & `monai_weekly-1.4.dev2422/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/dist.py` & `monai_weekly-1.4.dev2422/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/enums.py` & `monai_weekly-1.4.dev2422/monai/utils/enums.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/jupyter_utils.py` & `monai_weekly-1.4.dev2422/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/misc.py` & `monai_weekly-1.4.dev2422/monai/utils/misc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/module.py` & `monai_weekly-1.4.dev2422/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/nvtx.py` & `monai_weekly-1.4.dev2422/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/profiling.py` & `monai_weekly-1.4.dev2422/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/state_cacher.py` & `monai_weekly-1.4.dev2422/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/tf32.py` & `monai_weekly-1.4.dev2422/monai/utils/tf32.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/utils/type_conversion.py` & `monai_weekly-1.4.dev2422/monai/utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/__init__.py` & `monai_weekly-1.4.dev2422/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/class_activation_maps.py` & `monai_weekly-1.4.dev2422/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/gradient_based.py` & `monai_weekly-1.4.dev2422/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/img2tensorboard.py` & `monai_weekly-1.4.dev2422/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/occlusion_sensitivity.py` & `monai_weekly-1.4.dev2422/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/utils.py` & `monai_weekly-1.4.dev2422/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai/visualize/visualizer.py` & `monai_weekly-1.4.dev2422/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai_weekly.egg-info/PKG-INFO` & `monai_weekly-1.4.dev2422/monai_weekly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.4.dev2421
+Version: 1.4.dev2422
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai_weekly-1.4.dev2421/monai_weekly.egg-info/SOURCES.txt` & `monai_weekly-1.4.dev2422/monai_weekly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/monai_weekly.egg-info/requires.txt` & `monai_weekly-1.4.dev2422/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/pyproject.toml` & `monai_weekly-1.4.dev2422/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/setup.cfg` & `monai_weekly-1.4.dev2422/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/setup.py` & `monai_weekly-1.4.dev2422/setup.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_acn_block.py` & `monai_weekly-1.4.dev2422/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_activations.py` & `monai_weekly-1.4.dev2422/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_activationsd.py` & `monai_weekly-1.4.dev2422/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_adaptors.py` & `monai_weekly-1.4.dev2422/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_add_coordinate_channels.py` & `monai_weekly-1.4.dev2422/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_add_coordinate_channelsd.py` & `monai_weekly-1.4.dev2422/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_add_extreme_points_channel.py` & `monai_weekly-1.4.dev2422/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_add_extreme_points_channeld.py` & `monai_weekly-1.4.dev2422/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_adjust_contrast.py` & `monai_weekly-1.4.dev2422/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_adjust_contrastd.py` & `monai_weekly-1.4.dev2422/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_adn.py` & `monai_weekly-1.4.dev2422/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_adversarial_loss.py` & `monai_weekly-1.4.dev2422/tests/test_adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_affine.py` & `monai_weekly-1.4.dev2422/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_affine_grid.py` & `monai_weekly-1.4.dev2422/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_affine_transform.py` & `monai_weekly-1.4.dev2422/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_affined.py` & `monai_weekly-1.4.dev2422/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ahnet.py` & `monai_weekly-1.4.dev2422/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_alias.py` & `monai_weekly-1.4.dev2422/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_anchor_box.py` & `monai_weekly-1.4.dev2422/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_apply.py` & `monai_weekly-1.4.dev2422/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_apply_filter.py` & `monai_weekly-1.4.dev2422/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_arraydataset.py` & `monai_weekly-1.4.dev2422/tests/test_arraydataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     (0, 1),
     (1, 128, 128, 128),
 ]
 
 
 class TestCompose(Compose):
 
-    def __call__(self, input_, lazy):
+    def __call__(self, input_, lazy=False):
         img = self.transforms[0](input_)
         metadata = img.meta
         img = self.transforms[1](img)
         img = self.transforms[2](img, lazy=lazy)
         metadata = img.meta
         return self.transforms[3](img), metadata
```

### Comparing `monai_weekly-1.4.dev2421/tests/test_as_channel_last.py` & `monai_weekly-1.4.dev2422/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_as_channel_lastd.py` & `monai_weekly-1.4.dev2422/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_as_discrete.py` & `monai_weekly-1.4.dev2422/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_as_discreted.py` & `monai_weekly-1.4.dev2422/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_atss_box_matcher.py` & `monai_weekly-1.4.dev2422/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_attentionunet.py` & `monai_weekly-1.4.dev2422/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_auto3dseg.py` & `monai_weekly-1.4.dev2422/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_auto3dseg_bundlegen.py` & `monai_weekly-1.4.dev2422/tests/test_auto3dseg_bundlegen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_auto3dseg_ensemble.py` & `monai_weekly-1.4.dev2422/tests/test_auto3dseg_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_auto3dseg_hpo.py` & `monai_weekly-1.4.dev2422/tests/test_auto3dseg_hpo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_autoencoder.py` & `monai_weekly-1.4.dev2422/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_avg_merger.py` & `monai_weekly-1.4.dev2422/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_barlow_twins_loss.py` & `monai_weekly-1.4.dev2422/tests/test_barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_basic_unet.py` & `monai_weekly-1.4.dev2422/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_basic_unetplusplus.py` & `monai_weekly-1.4.dev2422/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bending_energy.py` & `monai_weekly-1.4.dev2422/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bilateral_approx_cpu.py` & `monai_weekly-1.4.dev2422/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bilateral_approx_cuda.py` & `monai_weekly-1.4.dev2422/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bilateral_precise.py` & `monai_weekly-1.4.dev2422/tests/test_bilateral_precise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_blend_images.py` & `monai_weekly-1.4.dev2422/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_border_pad.py` & `monai_weekly-1.4.dev2422/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_border_padd.py` & `monai_weekly-1.4.dev2422/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bounding_rect.py` & `monai_weekly-1.4.dev2422/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bounding_rectd.py` & `monai_weekly-1.4.dev2422/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_box_coder.py` & `monai_weekly-1.4.dev2422/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_box_transform.py` & `monai_weekly-1.4.dev2422/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_box_utils.py` & `monai_weekly-1.4.dev2422/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_ckpt_export.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_download.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_get_data.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_init_bundle.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_onnx_export.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_push_to_hf_hub.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_trt_export.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_trt_export.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_utils.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_verify_metadata.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_verify_net.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_bundle_workflow.py` & `monai_weekly-1.4.dev2422/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cachedataset.py` & `monai_weekly-1.4.dev2422/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cachedataset_parallel.py` & `monai_weekly-1.4.dev2422/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cachedataset_persistent_workers.py` & `monai_weekly-1.4.dev2422/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cachentransdataset.py` & `monai_weekly-1.4.dev2422/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_call_dist.py` & `monai_weekly-1.4.dev2422/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cast_to_type.py` & `monai_weekly-1.4.dev2422/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cast_to_typed.py` & `monai_weekly-1.4.dev2422/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_center_scale_crop.py` & `monai_weekly-1.4.dev2422/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_center_scale_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_center_spatial_crop.py` & `monai_weekly-1.4.dev2422/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_center_spatial_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_channel_pad.py` & `monai_weekly-1.4.dev2422/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_check_hash.py` & `monai_weekly-1.4.dev2422/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_check_missing_files.py` & `monai_weekly-1.4.dev2422/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_classes_to_indices.py` & `monai_weekly-1.4.dev2422/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_classes_to_indicesd.py` & `monai_weekly-1.4.dev2422/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cldice_loss.py` & `monai_weekly-1.4.dev2422/tests/test_cldice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_clip_intensity_percentiles.py` & `monai_weekly-1.4.dev2422/tests/test_clip_intensity_percentiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,81 +14,100 @@
 
 import torch
 from parameterized import parameterized
 
 from monai.transforms import ClipIntensityPercentiles
 from monai.transforms.utils import soft_clip
 from monai.transforms.utils_pytorch_numpy_unification import clip, percentile
+from monai.utils.type_conversion import convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, NumpyImageTestCase3D, assert_allclose
 
 
+def test_hard_clip_func(im, lower, upper):
+    im_t = convert_to_tensor(im)
+    if lower is None:
+        upper = percentile(im_t, upper)
+    elif upper is None:
+        lower = percentile(im_t, lower)
+    else:
+        lower, upper = percentile(im_t, (lower, upper))
+    return clip(im_t, lower, upper)
+
+
+def test_soft_clip_func(im, lower, upper):
+    im_t = convert_to_tensor(im)
+    if lower is None:
+        upper = percentile(im_t, upper)
+    elif upper is None:
+        lower = percentile(im_t, lower)
+    else:
+        lower, upper = percentile(im_t, (lower, upper))
+    return soft_clip(im_t, minv=lower, maxv=upper, sharpness_factor=1.0, dtype=torch.float32)
+
+
 class TestClipIntensityPercentiles2D(NumpyImageTestCase2D):
+
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (5, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 95)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (0, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 0, 95)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (5, 100))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 100)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        lower, upper = percentile(im, (5, 95))
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, 5, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_high(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=None, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        upper = percentile(im, 95)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=None, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 5e-5 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, None, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_low(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=None, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        lower = percentile(im, 5)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=None, dtype=torch.float32)
-        # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, 5, None)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_channel_wise(self, p):
         clipper = ClipIntensityPercentiles(upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper(im)
-        for i, c in enumerate(im):
+        im_t = convert_to_tensor(self.imt)
+        for i, c in enumerate(im_t):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
             assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     def test_ill_sharpness_factor(self):
         with self.assertRaises(ValueError):
             ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=0.0)
@@ -113,72 +132,67 @@
 class TestClipIntensityPercentiles3D(NumpyImageTestCase3D):
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (5, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 95)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (0, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 0, 95)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         hard_clipper = ClipIntensityPercentiles(upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper(im)
-        lower, upper = percentile(im, (5, 100))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 100)
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        lower, upper = percentile(im, (5, 95))
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=upper, dtype=torch.float32)
+        expected = test_soft_clip_func(im, 5, 95)
         # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_high(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=95, lower=None, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        upper = percentile(im, 95)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=None, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 5e-5 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, None, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_low(self, p):
         soft_clipper = ClipIntensityPercentiles(upper=None, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper(im)
-        lower = percentile(im, 5)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=None, dtype=torch.float32)
-        # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, 5, None)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result, p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_channel_wise(self, p):
         clipper = ClipIntensityPercentiles(upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper(im)
-        for i, c in enumerate(im):
+        im_t = convert_to_tensor(self.imt)
+        for i, c in enumerate(im_t):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
             assert_allclose(result[i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2421/tests/test_clip_intensity_percentilesd.py` & `monai_weekly-1.4.dev2422/tests/test_clip_intensity_percentilesd.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,95 +9,91 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import unittest
 
-import torch
 from parameterized import parameterized
 
 from monai.transforms import ClipIntensityPercentilesd
-from monai.transforms.utils import soft_clip
 from monai.transforms.utils_pytorch_numpy_unification import clip, percentile
+from monai.utils.type_conversion import convert_to_tensor
 from tests.utils import TEST_NDARRAYS, NumpyImageTestCase2D, NumpyImageTestCase3D, assert_allclose
 
+from .test_clip_intensity_percentiles import test_hard_clip_func, test_soft_clip_func
+
 
 class TestClipIntensityPercentilesd2D(NumpyImageTestCase2D):
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (5, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 95)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (0, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 0, 95)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (5, 100))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 100)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        lower, upper = percentile(im, (5, 95))
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, 5, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_high(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        upper = percentile(im, 95)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=None, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 5e-5 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, None, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_low(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        lower = percentile(im, 5)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=None, dtype=torch.float32)
-        # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, 5, None)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_channel_wise(self, p):
         key = "img"
         clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper({key: im})
-        for i, c in enumerate(im):
+        im_t = convert_to_tensor(self.imt)
+        for i, c in enumerate(im_t):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
             assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-3, atol=0)
 
     def test_ill_sharpness_factor(self):
         key = "img"
         with self.assertRaises(ValueError):
@@ -128,78 +124,73 @@
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_two_sided(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (5, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 95)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_high(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (0, 95))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 0, 95)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_hard_clipping_one_sided_low(self, p):
         key = "img"
         hard_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5)
         im = p(self.imt)
         result = hard_clipper({key: im})
-        lower, upper = percentile(im, (5, 100))
-        expected = clip(im, lower, upper)
+        expected = test_hard_clip_func(im, 5, 100)
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_two_sided(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        lower, upper = percentile(im, (5, 95))
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=upper, dtype=torch.float32)
+        expected = test_soft_clip_func(im, 5, 95)
         # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_high(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=None, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        upper = percentile(im, 95)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=None, maxv=upper, dtype=torch.float32)
-        # the rtol is set to 5e-5 because the logaddexp function used in softplus is not stable accross torch and numpy
+        expected = test_soft_clip_func(im, None, 95)
+        # the rtol is set to 1e-4 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_soft_clipping_one_sided_low(self, p):
         key = "img"
         soft_clipper = ClipIntensityPercentilesd(keys=[key], upper=None, lower=5, sharpness_factor=1.0)
         im = p(self.imt)
         result = soft_clipper({key: im})
-        lower = percentile(im, 5)
-        expected = soft_clip(im, sharpness_factor=1.0, minv=lower, maxv=None, dtype=torch.float32)
+        expected = test_soft_clip_func(im, 5, None)
         # the rtol is set to 1e-6 because the logaddexp function used in softplus is not stable accross torch and numpy
         assert_allclose(result[key], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
     @parameterized.expand([[p] for p in TEST_NDARRAYS])
     def test_channel_wise(self, p):
         key = "img"
         clipper = ClipIntensityPercentilesd(keys=[key], upper=95, lower=5, channel_wise=True)
         im = p(self.imt)
         result = clipper({key: im})
-        for i, c in enumerate(im):
+        im_t = convert_to_tensor(im)
+        for i, c in enumerate(im_t):
             lower, upper = percentile(c, (5, 95))
             expected = clip(c, lower, upper)
             assert_allclose(result[key][i], p(expected), type_test="tensor", rtol=1e-4, atol=0)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai_weekly-1.4.dev2421/tests/test_complex_utils.py` & `monai_weekly-1.4.dev2422/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_component_locator.py` & `monai_weekly-1.4.dev2422/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_component_store.py` & `monai_weekly-1.4.dev2422/tests/test_component_store.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compose.py` & `monai_weekly-1.4.dev2422/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compose_get_number_conversions.py` & `monai_weekly-1.4.dev2422/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_confusion_matrix.py` & `monai_weekly-1.4.dev2422/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_f_beta.py` & `monai_weekly-1.4.dev2422/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_fid_metric.py` & `monai_weekly-1.4.dev2422/tests/test_compute_fid_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_froc.py` & `monai_weekly-1.4.dev2422/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_generalized_dice.py` & `monai_weekly-1.4.dev2422/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_ho_ver_maps.py` & `monai_weekly-1.4.dev2422/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_ho_ver_maps_d.py` & `monai_weekly-1.4.dev2422/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_meandice.py` & `monai_weekly-1.4.dev2422/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_meaniou.py` & `monai_weekly-1.4.dev2422/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_mmd_metric.py` & `monai_weekly-1.4.dev2422/tests/test_compute_mmd_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_multiscalessim_metric.py` & `monai_weekly-1.4.dev2422/tests/test_compute_multiscalessim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_panoptic_quality.py` & `monai_weekly-1.4.dev2422/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_regression_metrics.py` & `monai_weekly-1.4.dev2422/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_roc_auc.py` & `monai_weekly-1.4.dev2422/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_compute_variance.py` & `monai_weekly-1.4.dev2422/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_concat_itemsd.py` & `monai_weekly-1.4.dev2422/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_config_item.py` & `monai_weekly-1.4.dev2422/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_config_parser.py` & `monai_weekly-1.4.dev2422/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_conjugate_gradient.py` & `monai_weekly-1.4.dev2422/tests/test_conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_contrastive_loss.py` & `monai_weekly-1.4.dev2422/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_data_type.py` & `monai_weekly-1.4.dev2422/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_to_multi_channel.py` & `monai_weekly-1.4.dev2422/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_to_multi_channeld.py` & `monai_weekly-1.4.dev2422/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_to_onnx.py` & `monai_weekly-1.4.dev2422/tests/test_convert_to_onnx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_to_torchscript.py` & `monai_weekly-1.4.dev2422/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convert_to_trt.py` & `monai_weekly-1.4.dev2422/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_convolutions.py` & `monai_weekly-1.4.dev2422/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_copy_itemsd.py` & `monai_weekly-1.4.dev2422/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_copy_model_state.py` & `monai_weekly-1.4.dev2422/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_correct_crop_centers.py` & `monai_weekly-1.4.dev2422/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_create_cross_validation_datalist.py` & `monai_weekly-1.4.dev2422/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_create_grid_and_affine.py` & `monai_weekly-1.4.dev2422/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_crf_cpu.py` & `monai_weekly-1.4.dev2422/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_crf_cuda.py` & `monai_weekly-1.4.dev2422/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_crop_foreground.py` & `monai_weekly-1.4.dev2422/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_crop_foregroundd.py` & `monai_weekly-1.4.dev2422/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cross_validation.py` & `monai_weekly-1.4.dev2422/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_csv_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_csv_iterable_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_csv_saver.py` & `monai_weekly-1.4.dev2422/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cucim_dict_transform.py` & `monai_weekly-1.4.dev2422/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cucim_transform.py` & `monai_weekly-1.4.dev2422/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cumulative.py` & `monai_weekly-1.4.dev2422/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cumulative_average.py` & `monai_weekly-1.4.dev2422/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cumulative_average_dist.py` & `monai_weekly-1.4.dev2422/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_cv2_dist.py` & `monai_weekly-1.4.dev2422/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_daf3d.py` & `monai_weekly-1.4.dev2422/tests/test_daf3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_data_stats.py` & `monai_weekly-1.4.dev2422/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_data_statsd.py` & `monai_weekly-1.4.dev2422/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dataloader.py` & `monai_weekly-1.4.dev2422/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from io import StringIO
 
 import nibabel as nib
 import numpy as np
 from parameterized import parameterized
 
 from monai.data import Dataset
-from monai.transforms import Compose, LoadImaged, SimulateDelayd
+from monai.transforms import Compose, Lambda, LoadImage, LoadImaged, SimulateDelay, SimulateDelayd
 from tests.test_compose import TEST_COMPOSE_LAZY_ON_CALL_LOGGING_TEST_CASES, data_from_keys
 
 TEST_CASE_1 = [(128, 128, 128)]
 
 
 class TestDataset(unittest.TestCase):
 
@@ -95,14 +95,80 @@
                 self.assertTupleEqual(d["image"].shape, expected_shape)
 
     def test_dataset_lazy_on_call(self):
         data = np.zeros((1, 5, 5))
         data[0, 0:2, 0:2] = 1
 
 
+class TestTupleDataset(unittest.TestCase):
+
+    @parameterized.expand([TEST_CASE_1])
+    def test_shape(self, expected_shape):
+        test_image = nib.Nifti1Image(np.random.randint(0, 2, size=[128, 128, 128]).astype(float), np.eye(4))
+        with tempfile.TemporaryDirectory() as tempdir:
+            nib.save(test_image, os.path.join(tempdir, "test_image1.nii.gz"))
+            nib.save(test_image, os.path.join(tempdir, "test_label1.nii.gz"))
+            nib.save(test_image, os.path.join(tempdir, "test_image2.nii.gz"))
+            nib.save(test_image, os.path.join(tempdir, "test_label2.nii.gz"))
+            test_data = [
+                (os.path.join(tempdir, "test_image1.nii.gz"), os.path.join(tempdir, "test_label1.nii.gz")),
+                (os.path.join(tempdir, "test_image2.nii.gz"), os.path.join(tempdir, "test_label2.nii.gz")),
+            ]
+
+            test_transform = Compose([LoadImage(), SimulateDelay(delay_time=1e-5)])
+
+            # Here test_transform is applied element by element for the tuple.
+            dataset = Dataset(data=test_data, transform=test_transform)
+            data1 = dataset[0]
+            data2 = dataset[1]
+
+            # Output is a list/tuple
+            self.assertTrue(isinstance(data1, (list, tuple)))
+            self.assertTrue(isinstance(data2, (list, tuple)))
+
+            # Number of elements are 2
+            self.assertEqual(len(data1), 2)
+            self.assertEqual(len(data2), 2)
+
+            # Output shapes are as expected
+            self.assertTupleEqual(data1[0].shape, expected_shape)
+            self.assertTupleEqual(data1[1].shape, expected_shape)
+            self.assertTupleEqual(data2[0].shape, expected_shape)
+            self.assertTupleEqual(data2[1].shape, expected_shape)
+
+            # Here test_transform is applied to the tuple as a whole.
+            test_transform = Compose(
+                [
+                    # LoadImage creates a channel-stacked image when applied to a tuple
+                    LoadImage(),
+                    # Get the channel-stacked image and the label
+                    Lambda(func=lambda x: (x[0].permute(2, 1, 0), x[1])),
+                ],
+                map_items=False,
+            )
+
+            dataset = Dataset(data=test_data, transform=test_transform)
+            data1 = dataset[0]
+            data2 = dataset[1]
+
+            # Output is a list/tuple
+            self.assertTrue(isinstance(data1, (list, tuple)))
+            self.assertTrue(isinstance(data2, (list, tuple)))
+
+            # Number of elements are 2
+            self.assertEqual(len(data1), 2)
+            self.assertEqual(len(data2), 2)
+
+            # Output shapes are as expected
+            self.assertTupleEqual(data1[0].shape, expected_shape)
+            self.assertTupleEqual(data1[1].shape, expected_shape)
+            self.assertTupleEqual(data2[0].shape, expected_shape)
+            self.assertTupleEqual(data2[1].shape, expected_shape)
+
+
 class TestDatsesetWithLazy(unittest.TestCase):
     LOGGER_NAME = "a_logger_name"
 
     def init_logger(self, name=LOGGER_NAME):
         stream = StringIO()
         handler = logging.StreamHandler(stream)
         formatter = logging.Formatter("%(levelname)s - %(message)s")
```

### Comparing `monai_weekly-1.4.dev2421/tests/test_dataset_func.py` & `monai_weekly-1.4.dev2422/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dataset_summary.py` & `monai_weekly-1.4.dev2422/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_decathlondataset.py` & `monai_weekly-1.4.dev2422/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_decollate.py` & `monai_weekly-1.4.dev2422/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deepedit_interaction.py` & `monai_weekly-1.4.dev2422/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deepedit_transforms.py` & `monai_weekly-1.4.dev2422/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deepgrow_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deepgrow_interaction.py` & `monai_weekly-1.4.dev2422/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deepgrow_transforms.py` & `monai_weekly-1.4.dev2422/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_delete_itemsd.py` & `monai_weekly-1.4.dev2422/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_denseblock.py` & `monai_weekly-1.4.dev2422/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_densenet.py` & `monai_weekly-1.4.dev2422/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_deprecated.py` & `monai_weekly-1.4.dev2422/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_detect_envelope.py` & `monai_weekly-1.4.dev2422/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_detection_coco_metrics.py` & `monai_weekly-1.4.dev2422/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_detector_boxselector.py` & `monai_weekly-1.4.dev2422/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_detector_utils.py` & `monai_weekly-1.4.dev2422/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dev_collate.py` & `monai_weekly-1.4.dev2422/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dice_ce_loss.py` & `monai_weekly-1.4.dev2422/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dice_focal_loss.py` & `monai_weekly-1.4.dev2422/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dice_loss.py` & `monai_weekly-1.4.dev2422/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_diffusion_loss.py` & `monai_weekly-1.4.dev2422/tests/test_diffusion_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dints_cell.py` & `monai_weekly-1.4.dev2422/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dints_mixop.py` & `monai_weekly-1.4.dev2422/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dints_network.py` & `monai_weekly-1.4.dev2422/tests/test_dints_network.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_discriminator.py` & `monai_weekly-1.4.dev2422/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_distance_transform_edt.py` & `monai_weekly-1.4.dev2422/tests/test_distance_transform_edt.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_divisible_pad.py` & `monai_weekly-1.4.dev2422/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_divisible_padd.py` & `monai_weekly-1.4.dev2422/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_download_and_extract.py` & `monai_weekly-1.4.dev2422/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_download_url_yandex.py` & `monai_weekly-1.4.dev2422/tests/test_download_url_yandex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_downsample_block.py` & `monai_weekly-1.4.dev2422/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_drop_path.py` & `monai_weekly-1.4.dev2422/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ds_loss.py` & `monai_weekly-1.4.dev2422/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dvf2ddf.py` & `monai_weekly-1.4.dev2422/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dynunet.py` & `monai_weekly-1.4.dev2422/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_dynunet_block.py` & `monai_weekly-1.4.dev2422/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_efficientnet.py` & `monai_weekly-1.4.dev2422/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensemble_evaluator.py` & `monai_weekly-1.4.dev2422/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensure_channel_first.py` & `monai_weekly-1.4.dev2422/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensure_channel_firstd.py` & `monai_weekly-1.4.dev2422/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensure_tuple.py` & `monai_weekly-1.4.dev2422/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensure_type.py` & `monai_weekly-1.4.dev2422/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ensure_typed.py` & `monai_weekly-1.4.dev2422/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_enum_bound_interp.py` & `monai_weekly-1.4.dev2422/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_eval_mode.py` & `monai_weekly-1.4.dev2422/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_evenly_divisible_all_gather_dist.py` & `monai_weekly-1.4.dev2422/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_factorized_increase.py` & `monai_weekly-1.4.dev2422/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_factorized_reduce.py` & `monai_weekly-1.4.dev2422/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fastmri_reader.py` & `monai_weekly-1.4.dev2422/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fft_utils.py` & `monai_weekly-1.4.dev2422/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fg_bg_to_indices.py` & `monai_weekly-1.4.dev2422/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fg_bg_to_indicesd.py` & `monai_weekly-1.4.dev2422/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_file_basename.py` & `monai_weekly-1.4.dev2422/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fill_holes.py` & `monai_weekly-1.4.dev2422/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fill_holesd.py` & `monai_weekly-1.4.dev2422/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fl_exchange_object.py` & `monai_weekly-1.4.dev2422/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fl_monai_algo.py` & `monai_weekly-1.4.dev2422/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fl_monai_algo_dist.py` & `monai_weekly-1.4.dev2422/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fl_monai_algo_stats.py` & `monai_weekly-1.4.dev2422/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_flatten_sub_keysd.py` & `monai_weekly-1.4.dev2422/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_flexible_unet.py` & `monai_weekly-1.4.dev2422/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_flip.py` & `monai_weekly-1.4.dev2422/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_flipd.py` & `monai_weekly-1.4.dev2422/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_focal_loss.py` & `monai_weekly-1.4.dev2422/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_folder_layout.py` & `monai_weekly-1.4.dev2422/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_foreground_mask.py` & `monai_weekly-1.4.dev2422/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_foreground_maskd.py` & `monai_weekly-1.4.dev2422/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fourier.py` & `monai_weekly-1.4.dev2422/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fpn_block.py` & `monai_weekly-1.4.dev2422/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_freeze_layers.py` & `monai_weekly-1.4.dev2422/tests/test_freeze_layers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_from_engine_hovernet.py` & `monai_weekly-1.4.dev2422/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_fullyconnectednet.py` & `monai_weekly-1.4.dev2422/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian_filter.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian_sharpen.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian_sharpend.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian_smooth.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gaussian_smoothd.py` & `monai_weekly-1.4.dev2422/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gdsdataset.py` & `monai_weekly-1.4.dev2422/tests/test_gdsdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generalized_dice_focal_loss.py` & `monai_weekly-1.4.dev2422/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generalized_dice_loss.py` & `monai_weekly-1.4.dev2422/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generalized_wasserstein_dice_loss.py` & `monai_weekly-1.4.dev2422/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_distance_map.py` & `monai_weekly-1.4.dev2422/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_distance_mapd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_border.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_borderd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_centroid.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_centroidd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_contour.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_contourd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_type.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_instance_typed.py` & `monai_weekly-1.4.dev2422/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_label_classes_crop_centers.py` & `monai_weekly-1.4.dev2422/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_param_groups.py` & `monai_weekly-1.4.dev2422/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_pos_neg_label_crop_centers.py` & `monai_weekly-1.4.dev2422/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_spatial_bounding_box.py` & `monai_weekly-1.4.dev2422/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_succinct_contour.py` & `monai_weekly-1.4.dev2422/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_succinct_contourd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_watershed_markers.py` & `monai_weekly-1.4.dev2422/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_watershed_markersd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_watershed_mask.py` & `monai_weekly-1.4.dev2422/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generate_watershed_maskd.py` & `monai_weekly-1.4.dev2422/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_generator.py` & `monai_weekly-1.4.dev2422/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_get_equivalent_dtype.py` & `monai_weekly-1.4.dev2422/tests/test_get_equivalent_dtype.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_get_extreme_points.py` & `monai_weekly-1.4.dev2422/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_get_layers.py` & `monai_weekly-1.4.dev2422/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_get_package_version.py` & `monai_weekly-1.4.dev2422/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_get_unique_labels.py` & `monai_weekly-1.4.dev2422/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gibbs_noise.py` & `monai_weekly-1.4.dev2422/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gibbs_noised.py` & `monai_weekly-1.4.dev2422/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_giou_loss.py` & `monai_weekly-1.4.dev2422/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_global_mutual_information_loss.py` & `monai_weekly-1.4.dev2422/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_globalnet.py` & `monai_weekly-1.4.dev2422/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_gmm.py` & `monai_weekly-1.4.dev2422/tests/test_gmm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_distortion.py` & `monai_weekly-1.4.dev2422/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_distortiond.py` & `monai_weekly-1.4.dev2422/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_patch.py` & `monai_weekly-1.4.dev2422/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_patchd.py` & `monai_weekly-1.4.dev2422/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_pull.py` & `monai_weekly-1.4.dev2422/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_split.py` & `monai_weekly-1.4.dev2422/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_grid_splitd.py` & `monai_weekly-1.4.dev2422/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_checkpoint_loader.py` & `monai_weekly-1.4.dev2422/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_checkpoint_saver.py` & `monai_weekly-1.4.dev2422/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_classification_saver.py` & `monai_weekly-1.4.dev2422/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_classification_saver_dist.py` & `monai_weekly-1.4.dev2422/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_clearml_image.py` & `monai_weekly-1.4.dev2422/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_clearml_stats.py` & `monai_weekly-1.4.dev2422/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_confusion_matrix.py` & `monai_weekly-1.4.dev2422/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_confusion_matrix_dist.py` & `monai_weekly-1.4.dev2422/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_decollate_batch.py` & `monai_weekly-1.4.dev2422/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_early_stop.py` & `monai_weekly-1.4.dev2422/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_garbage_collector.py` & `monai_weekly-1.4.dev2422/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_hausdorff_distance.py` & `monai_weekly-1.4.dev2422/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_ignite_metric.py` & `monai_weekly-1.4.dev2422/tests/test_handler_ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_logfile.py` & `monai_weekly-1.4.dev2422/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_lr_scheduler.py` & `monai_weekly-1.4.dev2422/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_mean_dice.py` & `monai_weekly-1.4.dev2422/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_mean_iou.py` & `monai_weekly-1.4.dev2422/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_metric_logger.py` & `monai_weekly-1.4.dev2422/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_metrics_reloaded.py` & `monai_weekly-1.4.dev2422/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_metrics_saver.py` & `monai_weekly-1.4.dev2422/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_metrics_saver_dist.py` & `monai_weekly-1.4.dev2422/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_mlflow.py` & `monai_weekly-1.4.dev2422/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_nvtx.py` & `monai_weekly-1.4.dev2422/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_panoptic_quality.py` & `monai_weekly-1.4.dev2422/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_parameter_scheduler.py` & `monai_weekly-1.4.dev2422/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_post_processing.py` & `monai_weekly-1.4.dev2422/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_prob_map_producer.py` & `monai_weekly-1.4.dev2422/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_regression_metrics.py` & `monai_weekly-1.4.dev2422/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_regression_metrics_dist.py` & `monai_weekly-1.4.dev2422/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_rocauc.py` & `monai_weekly-1.4.dev2422/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_rocauc_dist.py` & `monai_weekly-1.4.dev2422/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_smartcache.py` & `monai_weekly-1.4.dev2422/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_stats.py` & `monai_weekly-1.4.dev2422/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_surface_distance.py` & `monai_weekly-1.4.dev2422/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_tb_image.py` & `monai_weekly-1.4.dev2422/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_tb_stats.py` & `monai_weekly-1.4.dev2422/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_handler_validation.py` & `monai_weekly-1.4.dev2422/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hardnegsampler.py` & `monai_weekly-1.4.dev2422/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hashing.py` & `monai_weekly-1.4.dev2422/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hausdorff_distance.py` & `monai_weekly-1.4.dev2422/tests/test_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hausdorff_loss.py` & `monai_weekly-1.4.dev2422/tests/test_hausdorff_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_header_correct.py` & `monai_weekly-1.4.dev2422/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_highresnet.py` & `monai_weekly-1.4.dev2422/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hilbert_transform.py` & `monai_weekly-1.4.dev2422/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_histogram_normalize.py` & `monai_weekly-1.4.dev2422/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_histogram_normalized.py` & `monai_weekly-1.4.dev2422/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet_instance_map_post_processing.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet_instance_map_post_processingd.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet_loss.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet_nuclear_type_post_processing.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai_weekly-1.4.dev2422/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_identity.py` & `monai_weekly-1.4.dev2422/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_identityd.py` & `monai_weekly-1.4.dev2422/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_image_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_image_filter.py` & `monai_weekly-1.4.dev2422/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_image_rw.py` & `monai_weekly-1.4.dev2422/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_img2tensorboard.py` & `monai_weekly-1.4.dev2422/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_init_reader.py` & `monai_weekly-1.4.dev2422/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_autorunner.py` & `monai_weekly-1.4.dev2422/tests/test_integration_autorunner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_bundle_run.py` & `monai_weekly-1.4.dev2422/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_classification_2d.py` & `monai_weekly-1.4.dev2422/tests/test_integration_classification_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_determinism.py` & `monai_weekly-1.4.dev2422/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_fast_train.py` & `monai_weekly-1.4.dev2422/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_gpu_customization.py` & `monai_weekly-1.4.dev2422/tests/test_integration_gpu_customization.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_lazy_samples.py` & `monai_weekly-1.4.dev2422/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_nnunetv2_runner.py` & `monai_weekly-1.4.dev2422/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_segmentation_3d.py` & `monai_weekly-1.4.dev2422/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_sliding_window.py` & `monai_weekly-1.4.dev2422/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_stn.py` & `monai_weekly-1.4.dev2422/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_unet_2d.py` & `monai_weekly-1.4.dev2422/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_workers.py` & `monai_weekly-1.4.dev2422/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_workflows.py` & `monai_weekly-1.4.dev2422/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_integration_workflows_gan.py` & `monai_weekly-1.4.dev2422/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_intensity_stats.py` & `monai_weekly-1.4.dev2422/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_intensity_statsd.py` & `monai_weekly-1.4.dev2422/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_inverse.py` & `monai_weekly-1.4.dev2422/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_inverse_array.py` & `monai_weekly-1.4.dev2422/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_inverse_collation.py` & `monai_weekly-1.4.dev2422/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_invert.py` & `monai_weekly-1.4.dev2422/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_invertd.py` & `monai_weekly-1.4.dev2422/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_is_supported_format.py` & `monai_weekly-1.4.dev2422/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_iterable_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_itk_torch_bridge.py` & `monai_weekly-1.4.dev2422/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_itk_writer.py` & `monai_weekly-1.4.dev2422/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_k_space_spike_noise.py` & `monai_weekly-1.4.dev2422/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_k_space_spike_noised.py` & `monai_weekly-1.4.dev2422/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_keep_largest_connected_component.py` & `monai_weekly-1.4.dev2422/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_keep_largest_connected_componentd.py` & `monai_weekly-1.4.dev2422/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_kspace_mask.py` & `monai_weekly-1.4.dev2422/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_filter.py` & `monai_weekly-1.4.dev2422/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_filterd.py` & `monai_weekly-1.4.dev2422/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_quality_score.py` & `monai_weekly-1.4.dev2422/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_to_contour.py` & `monai_weekly-1.4.dev2422/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_to_contourd.py` & `monai_weekly-1.4.dev2422/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_to_mask.py` & `monai_weekly-1.4.dev2422/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_label_to_maskd.py` & `monai_weekly-1.4.dev2422/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lambda.py` & `monai_weekly-1.4.dev2422/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lambdad.py` & `monai_weekly-1.4.dev2422/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lesion_froc.py` & `monai_weekly-1.4.dev2422/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_list_data_collate.py` & `monai_weekly-1.4.dev2422/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_list_to_dict.py` & `monai_weekly-1.4.dev2422/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lltm.py` & `monai_weekly-1.4.dev2422/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lmdbdataset.py` & `monai_weekly-1.4.dev2422/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lmdbdataset_dist.py` & `monai_weekly-1.4.dev2422/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_load_decathlon_datalist.py` & `monai_weekly-1.4.dev2422/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_load_image.py` & `monai_weekly-1.4.dev2422/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_load_imaged.py` & `monai_weekly-1.4.dev2422/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_load_spacing_orientation.py` & `monai_weekly-1.4.dev2422/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_loader_semaphore.py` & `monai_weekly-1.4.dev2422/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_local_normalized_cross_correlation_loss.py` & `monai_weekly-1.4.dev2422/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_localnet.py` & `monai_weekly-1.4.dev2422/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_localnet_block.py` & `monai_weekly-1.4.dev2422/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_look_up_option.py` & `monai_weekly-1.4.dev2422/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_loss_metric.py` & `monai_weekly-1.4.dev2422/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lr_finder.py` & `monai_weekly-1.4.dev2422/tests/test_lr_finder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_lr_scheduler.py` & `monai_weekly-1.4.dev2422/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_make_nifti.py` & `monai_weekly-1.4.dev2422/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_and_generate_sampling_centers.py` & `monai_weekly-1.4.dev2422/tests/test_map_and_generate_sampling_centers.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_binary_to_indices.py` & `monai_weekly-1.4.dev2422/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_classes_to_indices.py` & `monai_weekly-1.4.dev2422/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_label_value.py` & `monai_weekly-1.4.dev2422/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_label_valued.py` & `monai_weekly-1.4.dev2422/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_map_transform.py` & `monai_weekly-1.4.dev2422/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mask_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mask_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_masked_dice_loss.py` & `monai_weekly-1.4.dev2422/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_masked_loss.py` & `monai_weekly-1.4.dev2422/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_masked_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_masked_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_matshow3d.py` & `monai_weekly-1.4.dev2422/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mean_ensemble.py` & `monai_weekly-1.4.dev2422/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mean_ensembled.py` & `monai_weekly-1.4.dev2422/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_median_filter.py` & `monai_weekly-1.4.dev2422/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_median_smooth.py` & `monai_weekly-1.4.dev2422/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_median_smoothd.py` & `monai_weekly-1.4.dev2422/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mednistdataset.py` & `monai_weekly-1.4.dev2422/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_meta_affine.py` & `monai_weekly-1.4.dev2422/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_meta_tensor.py` & `monai_weekly-1.4.dev2422/tests/test_meta_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_metatensor_integration.py` & `monai_weekly-1.4.dev2422/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_metrics_reloaded.py` & `monai_weekly-1.4.dev2422/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_milmodel.py` & `monai_weekly-1.4.dev2422/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mlp.py` & `monai_weekly-1.4.dev2422/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mmar_download.py` & `monai_weekly-1.4.dev2422/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_module_list.py` & `monai_weekly-1.4.dev2422/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_monai_env_vars.py` & `monai_weekly-1.4.dev2422/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_monai_utils_misc.py` & `monai_weekly-1.4.dev2422/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_mri_utils.py` & `monai_weekly-1.4.dev2422/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_multi_scale.py` & `monai_weekly-1.4.dev2422/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_net_adapter.py` & `monai_weekly-1.4.dev2422/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_network_consistency.py` & `monai_weekly-1.4.dev2422/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nifti_endianness.py` & `monai_weekly-1.4.dev2422/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nifti_header_revise.py` & `monai_weekly-1.4.dev2422/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nifti_rw.py` & `monai_weekly-1.4.dev2422/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_normalize_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_normalize_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_npzdictitemdataset.py` & `monai_weekly-1.4.dev2422/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nrrd_reader.py` & `monai_weekly-1.4.dev2422/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nuclick_transforms.py` & `monai_weekly-1.4.dev2422/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_numpy_reader.py` & `monai_weekly-1.4.dev2422/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nvtx_decorator.py` & `monai_weekly-1.4.dev2422/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_nvtx_transform.py` & `monai_weekly-1.4.dev2422/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_occlusion_sensitivity.py` & `monai_weekly-1.4.dev2422/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_one_of.py` & `monai_weekly-1.4.dev2422/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_optim_novograd.py` & `monai_weekly-1.4.dev2422/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_optional_import.py` & `monai_weekly-1.4.dev2422/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ori_ras_lps.py` & `monai_weekly-1.4.dev2422/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_orientation.py` & `monai_weekly-1.4.dev2422/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_orientationd.py` & `monai_weekly-1.4.dev2422/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_p3d_block.py` & `monai_weekly-1.4.dev2422/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pad_collation.py` & `monai_weekly-1.4.dev2422/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pad_mode.py` & `monai_weekly-1.4.dev2422/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_partition_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_partition_dataset_classes.py` & `monai_weekly-1.4.dev2422/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_patch_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_patch_inferer.py` & `monai_weekly-1.4.dev2422/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_patchembedding.py` & `monai_weekly-1.4.dev2422/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pathology_he_stain.py` & `monai_weekly-1.4.dev2422/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pathology_he_stain_dict.py` & `monai_weekly-1.4.dev2422/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pathology_prob_nms.py` & `monai_weekly-1.4.dev2422/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_perceptual_loss.py` & `monai_weekly-1.4.dev2422/tests/test_perceptual_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_persistentdataset.py` & `monai_weekly-1.4.dev2422/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_persistentdataset_dist.py` & `monai_weekly-1.4.dev2422/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_phl_cpu.py` & `monai_weekly-1.4.dev2422/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_phl_cuda.py` & `monai_weekly-1.4.dev2422/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_pil_reader.py` & `monai_weekly-1.4.dev2422/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_plot_2d_or_3d_image.py` & `monai_weekly-1.4.dev2422/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_png_rw.py` & `monai_weekly-1.4.dev2422/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_polyval.py` & `monai_weekly-1.4.dev2422/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_prepare_batch_default.py` & `monai_weekly-1.4.dev2422/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_prepare_batch_default_dist.py` & `monai_weekly-1.4.dev2422/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_prepare_batch_extra_input.py` & `monai_weekly-1.4.dev2422/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_prepare_batch_hovernet.py` & `monai_weekly-1.4.dev2422/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_preset_filters.py` & `monai_weekly-1.4.dev2422/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_print_info.py` & `monai_weekly-1.4.dev2422/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_print_transform_backends.py` & `monai_weekly-1.4.dev2422/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_probnms.py` & `monai_weekly-1.4.dev2422/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_probnmsd.py` & `monai_weekly-1.4.dev2422/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_profiling.py` & `monai_weekly-1.4.dev2422/tests/test_profiling.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class TestWorkflowProfiler(unittest.TestCase):
 
     def setUp(self):
         super().setUp()
 
         self.scale = mt.ScaleIntensity()
         self.scale_call_name = "ScaleIntensity.__call__"
+        self.compose_call_name = "Compose.__call__"
         self.test_comp = mt.Compose([mt.ScaleIntensity(), mt.RandAxisFlip(0.5)])
         self.test_image = torch.rand(1, 16, 16, 16)
         self.pid = os.getpid()
 
     def test_empty(self):
         """Test that the profiler correctly produces an empty result when nothing happens in a context."""
         wp = WorkflowProfiler()
@@ -78,15 +79,15 @@
 
         with WorkflowProfiler() as wp:
             batch = first(dl)
 
         self.assertSequenceEqual(batch.shape, (4, 1, 16, 16, 16))
 
         results = wp.get_results()
-        self.assertSequenceEqual(list(results), [self.scale_call_name])
+        self.assertSequenceEqual(list(results), [self.scale_call_name, self.compose_call_name])
 
         prs = results[self.scale_call_name]
 
         self.assertEqual(len(prs), 4)
 
     def test_profile_context(self):
         """Test results from profiling contexts with the same name accumulate correctly."""
@@ -94,14 +95,15 @@
             with wp.profile_ctx("context"):
                 self.scale(self.test_image)
 
             with wp.profile_ctx("context"):
                 self.scale(self.test_image)
 
         results = wp.get_results()
+
         self.assertSequenceEqual(set(results), {"ScaleIntensity.__call__", "context"})
 
         prs = results["context"]
 
         self.assertEqual(len(prs), 2)
 
     def test_profile_callable(self):
```

### Comparing `monai_weekly-1.4.dev2421/tests/test_pytorch_version_after.py` & `monai_weekly-1.4.dev2422/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_query_memory.py` & `monai_weekly-1.4.dev2422/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_quicknat.py` & `monai_weekly-1.4.dev2422/tests/test_quicknat.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_adjust_contrast.py` & `monai_weekly-1.4.dev2422/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_adjust_contrastd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_affine.py` & `monai_weekly-1.4.dev2422/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_affine_grid.py` & `monai_weekly-1.4.dev2422/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_affined.py` & `monai_weekly-1.4.dev2422/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_axis_flip.py` & `monai_weekly-1.4.dev2422/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_axis_flipd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_bias_field.py` & `monai_weekly-1.4.dev2422/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_bias_fieldd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_coarse_dropout.py` & `monai_weekly-1.4.dev2422/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_coarse_dropoutd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_coarse_shuffle.py` & `monai_weekly-1.4.dev2422/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_coarse_shuffled.py` & `monai_weekly-1.4.dev2422/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_crop_by_label_classes.py` & `monai_weekly-1.4.dev2422/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_crop_by_label_classesd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_crop_by_pos_neg_label.py` & `monai_weekly-1.4.dev2422/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai_weekly-1.4.dev2422/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_cucim_dict_transform.py` & `monai_weekly-1.4.dev2422/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_cucim_transform.py` & `monai_weekly-1.4.dev2422/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_deform_grid.py` & `monai_weekly-1.4.dev2422/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_elastic_2d.py` & `monai_weekly-1.4.dev2422/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_elastic_3d.py` & `monai_weekly-1.4.dev2422/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_elasticd_2d.py` & `monai_weekly-1.4.dev2422/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_elasticd_3d.py` & `monai_weekly-1.4.dev2422/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_flip.py` & `monai_weekly-1.4.dev2422/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_flipd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_noise.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_noised.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_sharpen.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_sharpend.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_smooth.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gaussian_smoothd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gibbs_noise.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_gibbs_noised.py` & `monai_weekly-1.4.dev2422/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_grid_distortion.py` & `monai_weekly-1.4.dev2422/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_grid_distortiond.py` & `monai_weekly-1.4.dev2422/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_grid_patch.py` & `monai_weekly-1.4.dev2422/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_grid_patchd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_histogram_shift.py` & `monai_weekly-1.4.dev2422/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_histogram_shiftd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_k_space_spike_noise.py` & `monai_weekly-1.4.dev2422/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_k_space_spike_noised.py` & `monai_weekly-1.4.dev2422/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_lambda.py` & `monai_weekly-1.4.dev2422/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_lambdad.py` & `monai_weekly-1.4.dev2422/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rician_noise.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rician_noised.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rotate.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rotate90.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rotate90d.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_rotated.py` & `monai_weekly-1.4.dev2422/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_crop.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_intensity_fixed_meand.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_intensity_fixed_meand.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_scale_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_shift_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_shift_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_simulate_low_resolution.py` & `monai_weekly-1.4.dev2422/tests/test_rand_simulate_low_resolution.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_simulate_low_resolutiond.py` & `monai_weekly-1.4.dev2422/tests/test_rand_simulate_low_resolutiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop.py` & `monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop_samples.py` & `monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_spatial_crop_samplesd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_spatial_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_std_shift_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_std_shift_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_weighted_crop.py` & `monai_weekly-1.4.dev2422/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_weighted_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_zoom.py` & `monai_weekly-1.4.dev2422/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rand_zoomd.py` & `monai_weekly-1.4.dev2422/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_randidentity.py` & `monai_weekly-1.4.dev2422/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_random_order.py` & `monai_weekly-1.4.dev2422/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_randomizable.py` & `monai_weekly-1.4.dev2422/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_randomizable_transform_type.py` & `monai_weekly-1.4.dev2422/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_randtorchvisiond.py` & `monai_weekly-1.4.dev2422/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rankfilter_dist.py` & `monai_weekly-1.4.dev2422/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_recon_net_utils.py` & `monai_weekly-1.4.dev2422/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_reference_based_normalize_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_reference_based_spatial_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_reference_resolver.py` & `monai_weekly-1.4.dev2422/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_reg_loss_integration.py` & `monai_weekly-1.4.dev2422/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_regunet.py` & `monai_weekly-1.4.dev2422/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_regunet_block.py` & `monai_weekly-1.4.dev2422/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_remove_repeated_channel.py` & `monai_weekly-1.4.dev2422/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_remove_repeated_channeld.py` & `monai_weekly-1.4.dev2422/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_remove_small_objects.py` & `monai_weekly-1.4.dev2422/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_repeat_channel.py` & `monai_weekly-1.4.dev2422/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_repeat_channeld.py` & `monai_weekly-1.4.dev2422/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_replace_module.py` & `monai_weekly-1.4.dev2422/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_require_pkg.py` & `monai_weekly-1.4.dev2422/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resample.py` & `monai_weekly-1.4.dev2422/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resample_backends.py` & `monai_weekly-1.4.dev2422/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resample_datalist.py` & `monai_weekly-1.4.dev2422/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resample_to_match.py` & `monai_weekly-1.4.dev2422/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resample_to_matchd.py` & `monai_weekly-1.4.dev2422/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resampler.py` & `monai_weekly-1.4.dev2422/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resize.py` & `monai_weekly-1.4.dev2422/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resize_with_pad_or_crop.py` & `monai_weekly-1.4.dev2422/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resize_with_pad_or_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resized.py` & `monai_weekly-1.4.dev2422/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_resnet.py` & `monai_weekly-1.4.dev2422/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_retinanet.py` & `monai_weekly-1.4.dev2422/tests/test_retinanet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_retinanet_detector.py` & `monai_weekly-1.4.dev2422/tests/test_retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_retinanet_predict_utils.py` & `monai_weekly-1.4.dev2422/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rotate.py` & `monai_weekly-1.4.dev2422/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rotate90.py` & `monai_weekly-1.4.dev2422/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rotate90d.py` & `monai_weekly-1.4.dev2422/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_rotated.py` & `monai_weekly-1.4.dev2422/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_safe_dtype_range.py` & `monai_weekly-1.4.dev2422/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_saliency_inferer.py` & `monai_weekly-1.4.dev2422/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sample_slices.py` & `monai_weekly-1.4.dev2422/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sampler_dist.py` & `monai_weekly-1.4.dev2422/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_save_classificationd.py` & `monai_weekly-1.4.dev2422/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_save_image.py` & `monai_weekly-1.4.dev2422/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_save_imaged.py` & `monai_weekly-1.4.dev2422/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_save_state.py` & `monai_weekly-1.4.dev2422/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_savitzky_golay_filter.py` & `monai_weekly-1.4.dev2422/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_savitzky_golay_smooth.py` & `monai_weekly-1.4.dev2422/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_savitzky_golay_smoothd.py` & `monai_weekly-1.4.dev2422/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity_fixed_mean.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity_fixed_mean.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity_range.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity_range_percentiles.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity_range_percentilesd.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensity_ranged.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_scale_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_se_block.py` & `monai_weekly-1.4.dev2422/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_se_blocks.py` & `monai_weekly-1.4.dev2422/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_seg_loss_integration.py` & `monai_weekly-1.4.dev2422/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_segresnet.py` & `monai_weekly-1.4.dev2422/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_segresnet_block.py` & `monai_weekly-1.4.dev2422/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_segresnet_ds.py` & `monai_weekly-1.4.dev2422/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_select_cross_validation_folds.py` & `monai_weekly-1.4.dev2422/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_select_itemsd.py` & `monai_weekly-1.4.dev2422/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_selfattention.py` & `monai_weekly-1.4.dev2422/tests/test_selfattention.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_senet.py` & `monai_weekly-1.4.dev2422/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_separable_filter.py` & `monai_weekly-1.4.dev2422/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_set_determinism.py` & `monai_weekly-1.4.dev2422/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_set_visible_devices.py` & `monai_weekly-1.4.dev2422/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_shift_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_shift_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_shuffle_buffer.py` & `monai_weekly-1.4.dev2422/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_continuouswavelet.py` & `monai_weekly-1.4.dev2422/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_fillempty.py` & `monai_weekly-1.4.dev2422/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_fillemptyd.py` & `monai_weekly-1.4.dev2422/tests/test_signal_fillemptyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_add_gaussiannoise.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_add_sine.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_add_sine_partial.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_add_squarepulse.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_add_squarepulse_partial.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_drop.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_scale.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_rand_shift.py` & `monai_weekly-1.4.dev2422/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_signal_remove_frequency.py` & `monai_weekly-1.4.dev2422/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_simple_aspp.py` & `monai_weekly-1.4.dev2422/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_simulatedelay.py` & `monai_weekly-1.4.dev2422/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_simulatedelayd.py` & `monai_weekly-1.4.dev2422/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_skip_connection.py` & `monai_weekly-1.4.dev2422/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_slice_inferer.py` & `monai_weekly-1.4.dev2422/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sliding_patch_wsi_dataset.py` & `monai_weekly-1.4.dev2422/tests/test_sliding_patch_wsi_dataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sliding_window_hovernet_inference.py` & `monai_weekly-1.4.dev2422/tests/test_sliding_window_hovernet_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sliding_window_inference.py` & `monai_weekly-1.4.dev2422/tests/test_sliding_window_inference.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sliding_window_splitter.py` & `monai_weekly-1.4.dev2422/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_smartcachedataset.py` & `monai_weekly-1.4.dev2422/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_smooth_field.py` & `monai_weekly-1.4.dev2422/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sobel_gradient.py` & `monai_weekly-1.4.dev2422/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sobel_gradientd.py` & `monai_weekly-1.4.dev2422/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_soft_clip.py` & `monai_weekly-1.4.dev2422/tests/test_soft_clip.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_some_of.py` & `monai_weekly-1.4.dev2422/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spacing.py` & `monai_weekly-1.4.dev2422/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spacingd.py` & `monai_weekly-1.4.dev2422/tests/test_spacingd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_combine_transforms.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_crop.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_cropd.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_pad.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_padd.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_resample.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spatial_resampled.py` & `monai_weekly-1.4.dev2422/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_spectral_loss.py` & `monai_weekly-1.4.dev2422/tests/test_spectral_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_splitdim.py` & `monai_weekly-1.4.dev2422/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_splitdimd.py` & `monai_weekly-1.4.dev2422/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_squeeze_unsqueeze.py` & `monai_weekly-1.4.dev2422/tests/test_squeeze_unsqueeze.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_squeezedim.py` & `monai_weekly-1.4.dev2422/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_squeezedimd.py` & `monai_weekly-1.4.dev2422/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ssim_loss.py` & `monai_weekly-1.4.dev2422/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ssim_metric.py` & `monai_weekly-1.4.dev2422/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_state_cacher.py` & `monai_weekly-1.4.dev2422/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_std_shift_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_std_shift_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_str2bool.py` & `monai_weekly-1.4.dev2422/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_str2list.py` & `monai_weekly-1.4.dev2422/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_subpixel_upsample.py` & `monai_weekly-1.4.dev2422/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_sure_loss.py` & `monai_weekly-1.4.dev2422/tests/test_sure_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_surface_dice.py` & `monai_weekly-1.4.dev2422/tests/test_surface_dice.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_surface_distance.py` & `monai_weekly-1.4.dev2422/tests/test_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_swin_unetr.py` & `monai_weekly-1.4.dev2422/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_synthetic.py` & `monai_weekly-1.4.dev2422/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_tciadataset.py` & `monai_weekly-1.4.dev2422/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_testtimeaugmentation.py` & `monai_weekly-1.4.dev2422/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_text_encoding.py` & `monai_weekly-1.4.dev2422/tests/test_text_encoding.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_thread_buffer.py` & `monai_weekly-1.4.dev2422/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_threadcontainer.py` & `monai_weekly-1.4.dev2422/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_threshold_intensity.py` & `monai_weekly-1.4.dev2422/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_threshold_intensityd.py` & `monai_weekly-1.4.dev2422/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_timedcall_dist.py` & `monai_weekly-1.4.dev2422/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_contiguous.py` & `monai_weekly-1.4.dev2422/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_cupy.py` & `monai_weekly-1.4.dev2422/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_cupyd.py` & `monai_weekly-1.4.dev2422/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_device.py` & `monai_weekly-1.4.dev2422/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_deviced.py` & `monai_weekly-1.4.dev2422/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_from_meta_tensord.py` & `monai_weekly-1.4.dev2422/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_numpy.py` & `monai_weekly-1.4.dev2422/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_numpyd.py` & `monai_weekly-1.4.dev2422/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_onehot.py` & `monai_weekly-1.4.dev2422/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_pil.py` & `monai_weekly-1.4.dev2422/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_pild.py` & `monai_weekly-1.4.dev2422/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_tensor.py` & `monai_weekly-1.4.dev2422/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_to_tensord.py` & `monai_weekly-1.4.dev2422/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_torchscript_utils.py` & `monai_weekly-1.4.dev2422/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_torchvision.py` & `monai_weekly-1.4.dev2422/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_torchvision_fc_model.py` & `monai_weekly-1.4.dev2422/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_torchvisiond.py` & `monai_weekly-1.4.dev2422/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_traceable_transform.py` & `monai_weekly-1.4.dev2422/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_train_mode.py` & `monai_weekly-1.4.dev2422/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_trainable_bilateral.py` & `monai_weekly-1.4.dev2422/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_trainable_joint_bilateral.py` & `monai_weekly-1.4.dev2422/tests/test_trainable_joint_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_transchex.py` & `monai_weekly-1.4.dev2422/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_transform.py` & `monai_weekly-1.4.dev2422/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_transformerblock.py` & `monai_weekly-1.4.dev2422/tests/test_transformerblock.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_transpose.py` & `monai_weekly-1.4.dev2422/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_transposed.py` & `monai_weekly-1.4.dev2422/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_tversky_loss.py` & `monai_weekly-1.4.dev2422/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_ultrasound_confidence_map_transform.py` & `monai_weekly-1.4.dev2422/tests/test_ultrasound_confidence_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_unet.py` & `monai_weekly-1.4.dev2422/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_unetr.py` & `monai_weekly-1.4.dev2422/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_unetr_block.py` & `monai_weekly-1.4.dev2422/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_unified_focal_loss.py` & `monai_weekly-1.4.dev2422/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_upsample_block.py` & `monai_weekly-1.4.dev2422/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_utils_pytorch_numpy_unification.py` & `monai_weekly-1.4.dev2422/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_varautoencoder.py` & `monai_weekly-1.4.dev2422/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_varnet.py` & `monai_weekly-1.4.dev2422/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_version.py` & `monai_weekly-1.4.dev2422/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_video_datasets.py` & `monai_weekly-1.4.dev2422/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vis_cam.py` & `monai_weekly-1.4.dev2422/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vis_gradbased.py` & `monai_weekly-1.4.dev2422/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vis_gradcam.py` & `monai_weekly-1.4.dev2422/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vit.py` & `monai_weekly-1.4.dev2422/tests/test_vit.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vitautoenc.py` & `monai_weekly-1.4.dev2422/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vnet.py` & `monai_weekly-1.4.dev2422/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vote_ensemble.py` & `monai_weekly-1.4.dev2422/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_vote_ensembled.py` & `monai_weekly-1.4.dev2422/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_voxelmorph.py` & `monai_weekly-1.4.dev2422/tests/test_voxelmorph.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_warp.py` & `monai_weekly-1.4.dev2422/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_watershed.py` & `monai_weekly-1.4.dev2422/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_watershedd.py` & `monai_weekly-1.4.dev2422/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_weight_init.py` & `monai_weekly-1.4.dev2422/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_weighted_random_sampler_dist.py` & `monai_weekly-1.4.dev2422/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_with_allow_missing_keys.py` & `monai_weekly-1.4.dev2422/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_write_metrics_reports.py` & `monai_weekly-1.4.dev2422/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_wsi_sliding_window_splitter.py` & `monai_weekly-1.4.dev2422/tests/test_wsi_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_wsireader.py` & `monai_weekly-1.4.dev2422/tests/test_wsireader.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_zarr_avg_merger.py` & `monai_weekly-1.4.dev2422/tests/test_zarr_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_zipdataset.py` & `monai_weekly-1.4.dev2422/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_zoom.py` & `monai_weekly-1.4.dev2422/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_zoom_affine.py` & `monai_weekly-1.4.dev2422/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/tests/test_zoomd.py` & `monai_weekly-1.4.dev2422/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai_weekly-1.4.dev2421/versioneer.py` & `monai_weekly-1.4.dev2422/versioneer.py`

 * *Files identical despite different names*

