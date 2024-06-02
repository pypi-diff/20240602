# Comparing `tmp/naluconfigs-13.8.3.tar.gz` & `tmp/naluconfigs-13.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-13.8.3.tar", last modified: Wed May 22 20:34:20 2024, max compression
+gzip compressed data, was "naluconfigs-13.8.4.tar", last modified: Sun Jun  2 13:15:15 2024, max compression
```

## Comparing `naluconfigs-13.8.3.tar` & `naluconfigs-13.8.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.725114 naluconfigs-13.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.729114 naluconfigs-13.8.3/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.725114 naluconfigs-13.8.3/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.733114 naluconfigs-13.8.3/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.737114 naluconfigs-13.8.3/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3s.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 20:34:20.000000 naluconfigs-13.8.3/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:34:20.741114 naluconfigs-13.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-22 20:34:12.000000 naluconfigs-13.8.3/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.575210 naluconfigs-13.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-06-02 13:15:15.575210 naluconfigs-13.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 13:15:15.575210 naluconfigs-13.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.559210 naluconfigs-13.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.559210 naluconfigs-13.8.4/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.559210 naluconfigs-13.8.4/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.563210 naluconfigs-13.8.4/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.567210 naluconfigs-13.8.4/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.571210 naluconfigs-13.8.4/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv3s.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.575210 naluconfigs-13.8.4/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-06-02 13:15:15.000000 naluconfigs-13.8.4/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-06-02 13:15:15.000000 naluconfigs-13.8.4/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 13:15:15.000000 naluconfigs-13.8.4/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 13:15:15.000000 naluconfigs-13.8.4/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-02 13:15:15.000000 naluconfigs-13.8.4/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 13:15:15.575210 naluconfigs-13.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-06-02 13:15:06.000000 naluconfigs-13.8.4/tests/test_range_keys.py
```

### Comparing `naluconfigs-13.8.3/PKG-INFO` & `naluconfigs-13.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.3
+Version: 13.8.4
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.3/README.md` & `naluconfigs-13.8.4/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/pyproject.toml` & `naluconfigs-13.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/setup.py` & `naluconfigs-13.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/__init__.py` & `naluconfigs-13.8.4/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/_constructors.py` & `naluconfigs-13.8.4/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/hiper.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-13.8.4/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/asocv3s.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/asocv3s.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/hiper.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   channels: 56
   chanshift: 10
   chips:
     0..13:
       !include_chip
       from: hiper::params
   num_chips: 14
-  installed_chips: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]
+  installed_chips: []  # [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]
   clock_file: Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
   connections:
     - serial
     - d2xx
   si5341_address: 0xEE
   default_baud:
     3000000: 33
@@ -58,15 +58,18 @@
     channel_mapping: # asic channel: ext. dac channel
       0, 4, 8, 12, 16, 20, 24, 28, 32, 36, 40, 44, 48, 52: 0
       1, 5, 9, 13, 17, 21, 25, 29, 33, 37, 41, 45, 49, 53: 6
       2, 6, 10, 14, 18, 22, 26, 30, 34, 38, 42, 46, 50, 54: 3
       3, 7, 11, 15, 19, 23, 27, 31, 35, 39, 43, 47, 51, 55: 4
   headers: 3
   numregs: 64
-  pedestals_blocks: 16
+  pedestals_blocks: 8
+  pedestals:
+    trigger_limit: 3.0
+    
   peripherals:
     current:
       chan: 0
       addr: 0xD0
       bits: 16
       gain: 8
     vadjn:
@@ -827,14 +830,28 @@
     busy_locked:
       address: 0x5C
       bitposition: 0
       bitwidth: 16
       description: 'HIPeR RxOut Busy_Locked Status'
       readwrite: r
       value: 0
+    chip_sysrst:
+      address: 0x32
+      bitposition: 0
+      bitwidth: 14
+      description: 'Individual AARDVARC chip sysrst bitN=chipN'
+      readwrite: rw
+      value: 0
+    chip_regclr:
+      address: 0x33
+      bitposition: 0
+      bitwidth: 14
+      description: 'Individual AARDVARC chip regclr bitN=chipN'
+      readwrite: rw
+      value: 0
   i2c_registers:
     i2c_en:
       address: 0x0F
       bitposition: 14
       bitwidth: 1
       description: ''
       readwrite: rw
```

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-13.8.4/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/exceptions.py` & `naluconfigs-13.8.4/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/helpers.py` & `naluconfigs-13.8.4/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs/postprocess.py` & `naluconfigs-13.8.4/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-13.8.4/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.3
+Version: 13.8.4
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.3/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-13.8.4/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/tests/test_hex_addr_converter.py` & `naluconfigs-13.8.4/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/tests/test_i2c_registers.py` & `naluconfigs-13.8.4/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/tests/test_multichip.py` & `naluconfigs-13.8.4/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/tests/test_post_processing.py` & `naluconfigs-13.8.4/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.3/tests/test_range_keys.py` & `naluconfigs-13.8.4/tests/test_range_keys.py`

 * *Files identical despite different names*

