# Comparing `tmp/epyt_flow-0.1.1.tar.gz` & `tmp/epyt_flow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyt_flow-0.1.1.tar", last modified: Mon May 13 08:55:45 2024, max compression
+gzip compressed data, was "epyt_flow-0.2.0.tar", last modified: Sun Jun  2 14:39:28 2024, max compression
```

## Comparing `epyt_flow-0.1.1.tar` & `epyt_flow-0.2.0.tar`

### file list

```diff
@@ -1,159 +1,168 @@
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5202 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1076 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/LICENSE
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      316 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/MANIFEST.in
--rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5815 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/PKG-INFO
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4361 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/README.md
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      174 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/REQUIREMENTS.txt
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/EPANET/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.804516 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      925 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1070 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1005 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4351 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   171230 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25173 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7782 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2786 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5991 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32936 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4018 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      838 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33821 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32358 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23669 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13947 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13955 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    69518 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19874 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24745 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24278 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input1.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25371 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    67160 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input3.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2563 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/main.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3600 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      654 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    26660 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/output.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    41722 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/project.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19500 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/quality.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21691 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21516 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    43451 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/report.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    36206 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/rules.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25997 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17375 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/text.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    30772 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/types.h
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.808516 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1536 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.812517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      941 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2848 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      412 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.h
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.812517 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3429 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1054 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23189 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4283 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      455 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    35046 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2147 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14274 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3055 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7068 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4364 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1337 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    38985 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    57734 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11505 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12126 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33854 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24060 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12104 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1811 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4387 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1090 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9778 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1280 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8542 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1249 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    28375 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1567 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      911 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/readme.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      453 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/EPANET/compile.sh
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        6 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/VERSION
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1230 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/data/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/data/benchmarks/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      754 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11175 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      880 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    20167 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3373 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10985 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/gecco_water_quality.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25445 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   507058 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4778 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/benchmarks/water_usage.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24343 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/data/networks.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/gym/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      115 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1281 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/control_gyms.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2950 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/gym/scenario_control_env.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12883 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/metrics.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.816517 epyt_flow-0.1.1/epyt_flow/models/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       75 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      789 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/event_detector.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3624 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/models/sensor_interpolation_detector.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/rest_api/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      126 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1886 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/base_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2342 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/res_manager.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    16115 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/scada_data_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11471 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/scenario_handler.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4928 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/rest_api/server.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12893 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/serialization.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      164 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/__init__.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/events/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      185 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7903 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/actuator_events.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2603 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14569 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/leakages.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8447 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_faults.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7538 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_attack.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6785 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2396 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/events/system_event.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6508 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/parallel_simulation.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/simulation/scada/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       90 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4489 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/advanced_control.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    76694 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9860 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data_export.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    27168 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_config.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    81432 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_simulator.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2186 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/simulation/scenario_visualizer.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    58161 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/epyt_flow/simulation/sensor_config.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9795 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/topology.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow/uncertainty/
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       89 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/__init__.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13592 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/model_uncertainty.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2324 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/sensor_noise.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17669 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/uncertainties.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5315 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/uncertainty/utils.py
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9817 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/epyt_flow/utils.py
-drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-05-13 08:55:45.820518 epyt_flow-0.1.1/epyt_flow.egg-info/
--rw-r--r--   0 aartelt   (1000) aartelt   (1000)     5815 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/PKG-INFO
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5471 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/SOURCES.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        1 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/dependency_links.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      175 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/requires.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       41 2024-05-13 08:55:45.000000 epyt_flow-0.1.1/epyt_flow.egg-info/top_level.txt
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1446 2024-05-13 08:42:00.000000 epyt_flow-0.1.1/pyproject.toml
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-13 08:55:45.824519 epyt_flow-0.1.1/setup.cfg
--rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-05-08 14:44:26.000000 epyt_flow-0.1.1/setup.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5202 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1076 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/LICENSE
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      316 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/MANIFEST.in
+-rw-r--r--   0 aartelt   (1000) aartelt   (1000)     6609 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/PKG-INFO
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5155 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/README.md
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      174 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/REQUIREMENTS.txt
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.197155 epyt_flow-0.2.0/epyt_flow/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.197155 epyt_flow-0.2.0/epyt_flow/EPANET/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.193155 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.201156 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      925 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1070 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1005 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4351 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   171230 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25173 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7782 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2786 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5991 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32936 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4018 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      838 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33821 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    32358 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23669 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13947 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13955 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    69518 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19874 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24745 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24278 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input1.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25371 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    67160 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input3.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2563 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/main.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3600 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      654 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    26660 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/output.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    41722 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/project.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    19500 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/quality.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21691 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21516 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    43451 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/report.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    36206 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/rules.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25997 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17375 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/text.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    30772 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/types.h
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.197155 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1536 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.201156 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      941 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2848 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      412 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.h
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.201156 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/include/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3429 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1054 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    23189 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1342 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4283 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      455 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    35046 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10817 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2147 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14274 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3055 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7068 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4364 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1337 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    38985 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11342 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    21817 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    57734 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11505 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12126 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    33854 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24060 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12104 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1811 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4387 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1090 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9778 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1280 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8542 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1249 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    28375 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1567 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      911 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/readme.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      489 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/EPANET/compile_linux.sh
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        6 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/VERSION
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1456 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/data/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/data/benchmarks/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      754 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11175 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/batadal.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      880 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/batadal_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    20167 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/battledim.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3373 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/battledim_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10985 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/gecco_water_quality.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    25445 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/leakdb.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)   507058 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/leakdb_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4778 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/benchmarks/water_usage.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    24343 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/data/networks.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/gym/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      115 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/gym/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1281 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/gym/control_gyms.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2950 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/gym/scenario_control_env.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12883 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/metrics.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/models/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       75 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/models/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      789 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/models/event_detector.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3624 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/models/sensor_interpolation_detector.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/rest_api/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      126 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/rest_api/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1886 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/rest_api/base_handler.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2342 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/rest_api/res_manager.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10938 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/data_handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4450 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/export_handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5391 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/handlers.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     3842 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/event_handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12353 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5905 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/simulation_handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4048 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/scenario/uncertainty_handlers.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7589 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/rest_api/server.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    12893 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/serialization.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.205155 epyt_flow-0.2.0/epyt_flow/simulation/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      164 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/__init__.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/epyt_flow/simulation/events/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      185 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7903 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/actuator_events.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2603 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    14569 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/leakages.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     8447 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_faults.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     7538 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_reading_attack.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6785 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_reading_event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2396 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/events/system_event.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     6508 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/parallel_simulation.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/epyt_flow/simulation/scada/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       90 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/scada/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     4489 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/scada/advanced_control.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    76710 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/simulation/scada/scada_data.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     9431 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/simulation/scada/scada_data_export.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    26531 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/simulation/scenario_config.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    91659 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/simulation/scenario_simulator.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2186 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/simulation/scenario_visualizer.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    71015 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/simulation/sensor_config.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    10961 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/topology.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/epyt_flow/uncertainty/
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       89 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/uncertainty/__init__.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    13592 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/uncertainty/model_uncertainty.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     2324 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/uncertainty/sensor_noise.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    17669 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/uncertainty/uncertainties.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5315 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/epyt_flow/uncertainty/utils.py
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)    11507 2024-06-02 14:29:19.000000 epyt_flow-0.2.0/epyt_flow/utils.py
+drwxrwxr-x   0 aartelt   (1000) aartelt   (1000)        0 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/epyt_flow.egg-info/
+-rw-r--r--   0 aartelt   (1000) aartelt   (1000)     6609 2024-06-02 14:39:28.000000 epyt_flow-0.2.0/epyt_flow.egg-info/PKG-INFO
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     5806 2024-06-02 14:39:28.000000 epyt_flow-0.2.0/epyt_flow.egg-info/SOURCES.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)        1 2024-06-02 14:39:28.000000 epyt_flow-0.2.0/epyt_flow.egg-info/dependency_links.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)      175 2024-06-02 14:39:28.000000 epyt_flow-0.2.0/epyt_flow.egg-info/requires.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       41 2024-06-02 14:39:28.000000 epyt_flow-0.2.0/epyt_flow.egg-info/top_level.txt
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)     1446 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/pyproject.toml
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-06-02 14:39:28.209155 epyt_flow-0.2.0/setup.cfg
+-rw-rw-r--   0 aartelt   (1000) aartelt   (1000)       38 2024-06-02 14:20:34.000000 epyt_flow-0.2.0/setup.py
```

### Comparing `epyt_flow-0.1.1/CODE_OF_CONDUCT.md` & `epyt_flow-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/LICENSE` & `epyt_flow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/PKG-INFO` & `epyt_flow-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyt-flow
-Version: 0.1.1
+Version: 0.2.0
 Summary: EPyT-Flow -- EPANET Python Toolkit - Flow
 Author-email: André Artelt <aartelt@techfak.uni-bielefeld.de>, "Marios S. Kyriakou" <kiriakou.marios@ucy.ac.cy>, "Stelios G. Vrachimis" <vrachimis.stelios@ucy.ac.cy>
 License: MIT License
 Project-URL: Homepage, https://github.com/WaterFutures/EPyT-Flow
 Project-URL: Documentation, https://epyt-flow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/WaterFutures/EPyT-Flow.git
 Project-URL: Issues, https://github.com/WaterFutures/EPyT-Flow/issues
@@ -48,14 +48,31 @@
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
 
 EPyT-Flow provides easy access to popular benchmark data sets for event detection and localization.
 Furthermore, it also provides an environment for developing and testing control algorithms.
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
+
+## Unique Features
+
+Unique features of EPyT-Flow that make it superior to other (Python) toolboxes are the following:
+
+- High-performance hydraulic and (advanced) water quality simulation
+- High- and low-level interface
+- Object-orientated design that is easy to extend and customize
+- Sensor configurations
+- Wide variety of pre-defined events (e.g. leakages, sensor faults, actuator events, cyber-attacks, etc.)
+- Wide variety of pre-defined types of uncertainties (e.g. model uncertainties)
+- Step-wise simulation and environment for training and evaluating control strategies
+- Serialization module for easy exchange of data and (scenario) configurations
+- REST API to make EPyT-Flow accessible in other applications
+- Access to many WDNs and popular benchmarks (incl. their evaluation)
+
+
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
 Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
```

### Comparing `epyt_flow-0.1.1/README.md` & `epyt_flow-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,31 @@
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
 
 EPyT-Flow provides easy access to popular benchmark data sets for event detection and localization.
 Furthermore, it also provides an environment for developing and testing control algorithms.
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
+
+## Unique Features
+
+Unique features of EPyT-Flow that make it superior to other (Python) toolboxes are the following:
+
+- High-performance hydraulic and (advanced) water quality simulation
+- High- and low-level interface
+- Object-orientated design that is easy to extend and customize
+- Sensor configurations
+- Wide variety of pre-defined events (e.g. leakages, sensor faults, actuator events, cyber-attacks, etc.)
+- Wide variety of pre-defined types of uncertainties (e.g. model uncertainties)
+- Step-wise simulation and environment for training and evaluating control strategies
+- Serialization module for easy exchange of data and (scenario) configurations
+- REST API to make EPyT-Flow accessible in other applications
+- Access to many WDNs and popular benchmarks (incl. their evaluation)
+
+
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
 Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
```

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/AUTHORS`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/LICENSE`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/Readme_SRC_Engines.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/enumstxt.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/epanet2.def`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/errors.dat`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/funcs.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/genmmd.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hash.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hash.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydcoeffs.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydraul.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydsolver.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/hydstatus.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/include/epanet2_enums.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/inpfile.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input1.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input1.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input2.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/input3.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/input3.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/main.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/main.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/mempool.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/output.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/output.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/project.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/project.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/quality.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/quality.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/qualreact.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/qualroute.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/report.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/report.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/rules.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/rules.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/smatrix.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/text.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/text.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET/SRC_engines/types.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET/SRC_engines/types.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/hash.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/hash.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/include/epanetmsx_export.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/mempool.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxchem.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxcompiler.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdict.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxdispersion.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxerr.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfile.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxfuncs.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxinp.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxout.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxproj.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxqual.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxrpt.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtank.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtoolkit.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxtypes.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/msxutils.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/newton.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/newton.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/rk5.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/ros2.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.c`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/Src/smatrix.h`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/EPANET/EPANET-MSX/readme.txt` & `epyt_flow-0.2.0/epyt_flow/EPANET/EPANET-MSX/readme.txt`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/__init__.py` & `epyt_flow-0.2.0/epyt_flow/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 import shutil
 import sys
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'VERSION'), encoding="utf-8") as f:
     VERSION = f.read().strip()
 
-if sys.platform.startswith("linux"):
-    def compile_libraries():
-        """Compile EPANET and EPANET-MSX libraries if needed."""
-        path_to_custom_libs = os.path.join(os.path.dirname(__file__), "customlibs")
-        path_to_lib_epanet = os.path.join(path_to_custom_libs, "libepanet2_2.so")
-        path_to_epanet = os.path.join(os.path.dirname(__file__), "EPANET")
-
-        update = False
-        if os.path.isfile(path_to_lib_epanet):
-            if os.path.getmtime(__file__) > os.path.getmtime(path_to_lib_epanet):
-                update = True
-
-        if not os.path.isfile(path_to_lib_epanet) or update:
-            if shutil.which("gcc") is not None:
-                print("Compiling EPANET and EPANET-MSX...")
-                subprocess.check_call(f"cd \"{path_to_epanet}\"; bash compile.sh", shell=True)
-            else:
-                warnings.warn("GCC is not available to compile the required libraries.\n" +
-                              "Falling back to pre-compiled library shipped by EPyT.")
 
-    compile_libraries()
+def compile_libraries_unix(lib_epanet_name, compile_script_name):
+    """Compile EPANET and EPANET-MSX libraries if needed."""
+    path_to_custom_libs = os.path.join(os.path.dirname(__file__), "customlibs")
+    path_to_lib_epanet = os.path.join(path_to_custom_libs, lib_epanet_name)
+    path_to_epanet = os.path.join(os.path.dirname(__file__), "EPANET")
+
+    update = False
+    if os.path.isfile(path_to_lib_epanet):
+        if os.path.getmtime(__file__) > os.path.getmtime(path_to_lib_epanet):
+            update = True
+
+    if not os.path.isfile(path_to_lib_epanet) or update:
+        if shutil.which("gcc") is not None:
+            print("Compiling EPANET and EPANET-MSX...")
+            try:
+                subprocess.check_call(f"cd \"{path_to_epanet}\"; bash {compile_script_name}",
+                                      shell=True)
+                print("Done")
+            except subprocess.CalledProcessError as ex:
+                print(f"Compilation failed\n{ex}")
+        else:
+            warnings.warn("GCC is not available to compile the required libraries.\n" +
+                          "Falling back to pre-compiled library shipped by EPyT.")
+
+
+if sys.platform.startswith("linux"):
+    compile_libraries_unix("libepanet2_2.so", "compile_linux.sh")
```

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/__init__.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/batadal.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/batadal_data.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/batadal_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/battledim.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/battledim_data.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/battledim_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/gecco_water_quality.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/gecco_water_quality.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/leakdb.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/leakdb_data.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/leakdb_data.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/benchmarks/water_usage.py` & `epyt_flow-0.2.0/epyt_flow/data/benchmarks/water_usage.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/data/networks.py` & `epyt_flow-0.2.0/epyt_flow/data/networks.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/gym/control_gyms.py` & `epyt_flow-0.2.0/epyt_flow/gym/control_gyms.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/gym/scenario_control_env.py` & `epyt_flow-0.2.0/epyt_flow/gym/scenario_control_env.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/metrics.py` & `epyt_flow-0.2.0/epyt_flow/metrics.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/models/event_detector.py` & `epyt_flow-0.2.0/epyt_flow/models/event_detector.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/models/sensor_interpolation_detector.py` & `epyt_flow-0.2.0/epyt_flow/models/sensor_interpolation_detector.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/rest_api/base_handler.py` & `epyt_flow-0.2.0/epyt_flow/rest_api/base_handler.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/rest_api/res_manager.py` & `epyt_flow-0.2.0/epyt_flow/rest_api/res_manager.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/rest_api/scada_data_handler.py` & `epyt_flow-0.2.0/epyt_flow/rest_api/scada_data/data_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,15 @@
 """
-The module provides all handlers for SCADA data requests.
+This module provides REST API handlers for accessing the final sensor readings
+(e.g. pressure, flow rate, etc.).
 """
 import warnings
 import falcon
 
-from .base_handler import BaseHandler
-from .res_manager import ResourceManager
-from ..simulation import SensorConfig, SensorFault
-
-
-class ScadaDataManager(ResourceManager):
-    """
-    Class for managing SCADA data.
-    """
-
-
-class ScadaDataBaseHandler(BaseHandler):
-    """
-    Base class for all handlers concerning SCADA data.
-
-    Parameters
-    ----------
-    scada_data_mgr : `~epyt_flow.rest_api.scenario_handler.ScadaDataBaseHandler`
-        SCADA data manager.
-    """
-    def __init__(self, scada_data_mgr: ScadaDataManager):
-        self.scada_data_mgr = scada_data_mgr
-
-
-class ScadaDataRemoveHandler(ScadaDataBaseHandler):
-    """
-    Class for handling a DELETE request for a given SCADA data instance.
-    """
-    def on_delete(self, _, resp: falcon.Response, data_id: str) -> None:
-        """
-        Deletes a given SCADA data instance.
-
-        Parameters
-        ----------
-        resp : `falcon.Response`
-            Response instance.
-        data_id : `str`
-            UUID of the SCADA data instance.
-        """
-        try:
-            if self.scada_data_mgr.validate_uuid(data_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            self.scada_data_mgr.remove(data_id)
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
-
-
-class ScadaDataSensorConfigHandler(ScadaDataBaseHandler):
-    """
-    Class for handling GET and POST requests for the sensor configuration
-    of a given SCADA data instance.
-    """
-    def on_get(self, _, resp: falcon.Response, data_id: str) -> None:
-        """
-        Gets the sensor configuration of a given SCADA data instance.
-
-        Parameters
-        ----------
-        resp : `falcon.Response`
-            Response instance.
-        data_id : `str`
-            UUID of the SCADA data.
-        """
-        try:
-            if self.scada_data_mgr.validate_uuid(data_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            my_sensor_config = self.scada_data_mgr.get(data_id).sensor_config
-            self.send_json_response(resp, my_sensor_config)
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
-
-    def on_post(self, req: falcon.Request, resp: falcon.Response, data_id: str) -> None:
-        """
-        Sets the sensor configuration of a given SCADA data instance.
-
-        Parameters
-        ----------
-        req : `falcon.Request`
-            Request instance.
-        resp : `falcon.Response`
-            Response instance.
-        data_id : `str`
-            UUID of the SCADA data.
-        """
-        try:
-            if self.scada_data_mgr.validate_uuid(data_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            sensor_config = self.load_json_data_from_request(req)
-            if not isinstance(sensor_config, SensorConfig):
-                self.send_json_parsing_error(resp)
-                return
-
-            self.scada_data_mgr.get(data_id).sensor_config = sensor_config
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
-
-
-class ScadaDataSensorFaultsHandler(ScadaDataBaseHandler):
-    """
-    Class for handling GET and POST requests concerning sensor faults in a
-    given SCADA data instance.
-    """
-    def on_get(self, _, resp: falcon.Response, data_id: str) -> None:
-        """
-        Gets all sensor faults of a given SCADA data instance.
-
-        Parameters
-        ----------
-        resp : `falcon.Response`
-            Response instance.
-        data_id : `str`
-            UUID of the SCADA data.
-        """
-        try:
-            if self.scada_data_mgr.validate_uuid(data_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            sensor_faults = self.scada_data_mgr.get(data_id).sensor_faults
-            self.send_json_response(resp, sensor_faults)
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
-
-    def on_post(self, req: falcon.Request, resp: falcon.Response, data_id: str) -> None:
-        """
-        Sets (i.e. overrides) the sensor faults in a given SCADA data instance.
-
-        Parameters
-        ----------
-        req : `falcon.Request`
-            Request instance.
-        resp : `falcon.Response`
-            Response instance.
-        data_id : `str`
-            UUID of the SCADA data.
-        """
-        try:
-            if self.scada_data_mgr.validate_uuid(data_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            sensor_faults = self.load_json_data_from_request(req)
-            if not isinstance(sensor_faults, list) or \
-                    any(not isinstance(e, SensorFault) for e in sensor_faults):
-                self.send_json_parsing_error(resp)
-                return
-
-            self.scada_data_mgr.get(data_id).sensor_faults = sensor_faults
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
+from .handlers import ScadaDataBaseHandler
 
 
 class ScadaDataPressuresHandler(ScadaDataBaseHandler):
     """
     Class for handling GET requests for the pressure sensor readings of a given SCADA data instance.
     """
     def on_get(self, _, resp: falcon.Response, data_id: str) -> None:
```

### Comparing `epyt_flow-0.1.1/epyt_flow/rest_api/scenario_handler.py` & `epyt_flow-0.2.0/epyt_flow/rest_api/scenario/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
-This module provides all handlers for requests concerning scenarios.
+This module provides REST API handlers for some requests concerning scenarios.
 """
 import warnings
+import os
 import falcon
 
-from .base_handler import BaseHandler
-from .res_manager import ResourceManager
-from .scada_data_handler import ScadaDataManager
-from ..simulation import ScenarioSimulator, Leakage, SensorConfig
+from ..base_handler import BaseHandler
+from ..res_manager import ResourceManager
+from ...utils import get_temp_folder, pack_zip_archive
+from ...simulation import ScenarioSimulator, SensorConfig
 
 
 class ScenarioManager(ResourceManager):
     """
     Class for managing all scenarios that are currently used by the REST API.
     """
     def create(self, **kwds) -> str:
@@ -32,15 +33,15 @@
 
 class ScenarioBaseHandler(BaseHandler):
     """
     Base class for all handlers concerning scenarios.
 
     Parameters
     ----------
-    scenario_mgr : :class:`~epyt_flow.rest_api.scenario_handler.ScenarioManager`
+    scenario_mgr : :class:`~epyt_flow.rest_api.scenario.handlers.ScenarioManager`
         Instance for managing all scenarios.
     """
     def __init__(self, scenario_mgr: ScenarioManager):
         self.scenario_mgr = scenario_mgr
 
 
 class ScenarioRemoveHandler(ScenarioBaseHandler):
@@ -65,117 +66,134 @@
 
             self.scenario_mgr.remove(scenario_id)
         except Exception as ex:
             warnings.warn(str(ex))
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
 
 
-class ScenarioConfigHandler(ScenarioBaseHandler):
+class ScenarioExportHandler(ScenarioBaseHandler):
     """
-    Class for handling a GET request for getting the scenario configuration of a given scenario.
+    Class for handling GET requests for exporting a given scenario to EPANET files
+    -- i.e. .inp and (otpionally) .msx files.
     """
-    def on_get(self, _, resp: falcon.Response, scenario_id: str) -> None:
+    def __create_temp_file_path(self, scenario_id: str, file_ext: str) -> None:
         """
-        Gets the scenario configuration of a given scenario.
+        Returns a path to a temporary file for storing the scenario.
 
         Parameters
         ----------
-        resp : `falcon.Response`
-            Response instance.
         scenario_id : `str`
             UUID of the scenario.
+        file_ext : `str`
+            File extension.
         """
-        try:
-            if self.scenario_mgr.validate_uuid(scenario_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
+        return os.path.join(get_temp_folder(), f"{scenario_id}.{file_ext}")
 
-            my_sceanrio_config = self.scenario_mgr.get(scenario_id).get_scenario_config()
-            self.send_json_response(resp, my_sceanrio_config)
-        except Exception as ex:
-            warnings.warn(str(ex))
-            resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
+    def __send_temp_file(self, resp: falcon.Response, tmp_file: str,
+                         content_type: str = "application/octet-stream") -> None:
+        """
+        Sends a given file (`tmp_file`) to the the client.
 
+        Parameters
+        ----------
+        resp : `falcon.Response`
+            Response instance.
+        tmp_file : `str`
+            Path to the temporary file to be send.
+        """
+        resp.status = falcon.HTTP_200
+        resp.content_type = content_type
+        with open(tmp_file, 'rb') as f:
+            resp.text = f.read()
 
-class ScenarioNewHandler(ScenarioBaseHandler):
-    """
-    Class for handling POST requests for creating a new scenario.
-    """
-    def on_post(self, req: falcon.Request, resp: falcon.Response) -> None:
+    def on_get(self, _, resp: falcon.Response, scenario_id: str) -> None:
         """
-        Creates/Loads a new scenario.
+        Exports a given scenario to an .inp and (optionally) .msx file.
 
         Parameters
         ----------
-        req : `falcon.Request`
-            Request instance.
         resp : `falcon.Response`
             Response instance.
         scenario_id : `str`
             UUID of the scenario.
         """
         try:
-            args = self.load_json_data_from_request(req)
-            scenario_id = self.scenario_mgr.create(**args)
-            self.send_json_response(resp, {"scenario_id": scenario_id})
+            if self.scenario_mgr.validate_uuid(scenario_id) is False:
+                self.send_invalid_resource_id_error(resp)
+                return
+
+            my_scenario = self.scenario_mgr.get(scenario_id)
+
+            f_inp_out = self.__create_temp_file_path(scenario_id, "inp")
+            f_msx_out = self.__create_temp_file_path(scenario_id, "msx")
+            my_scenario.save_to_epanet_file(f_inp_out, f_msx_out)
+
+            if os.path.isfile(f_msx_out):
+                f_out = self.__create_temp_file_path(scenario_id, "zip")
+                pack_zip_archive([f_inp_out, f_msx_out], f_out)
+
+                self.__send_temp_file(resp, f_out)
+                os.remove(f_out)
+                os.remove(f_msx_out)
+            else:
+                self.__send_temp_file(resp, f_inp_out)
+            os.remove(f_inp_out)
         except Exception as ex:
             warnings.warn(str(ex))
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
 
 
-class ScenarioLeakageHandler(ScenarioBaseHandler):
+class ScenarioConfigHandler(ScenarioBaseHandler):
     """
-    Class for handling GET and POST requests concerning leakages.
+    Class for handling a GET request for getting the scenario configuration of a given scenario.
     """
     def on_get(self, _, resp: falcon.Response, scenario_id: str) -> None:
         """
-        Gets all leakages of a given scenario.
+        Gets the scenario configuration of a given scenario.
 
         Parameters
         ----------
         resp : `falcon.Response`
             Response instance.
         scenario_id : `str`
             UUID of the scenario.
         """
         try:
             if self.scenario_mgr.validate_uuid(scenario_id) is False:
                 self.send_invalid_resource_id_error(resp)
                 return
 
-            my_leakages = self.scenario_mgr.get(scenario_id).leakages
-            self.send_json_response(resp, my_leakages)
+            my_sceanrio_config = self.scenario_mgr.get(scenario_id).get_scenario_config()
+            self.send_json_response(resp, my_sceanrio_config)
         except Exception as ex:
             warnings.warn(str(ex))
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
 
-    def on_post(self, req: falcon.Request, resp: falcon.Response, scenario_id: str) -> None:
+
+class ScenarioNewHandler(ScenarioBaseHandler):
+    """
+    Class for handling POST requests for creating a new scenario.
+    """
+    def on_post(self, req: falcon.Request, resp: falcon.Response) -> None:
         """
-        Adds a new leakage to a given scenario.
+        Creates/Loads a new scenario.
 
         Parameters
         ----------
         req : `falcon.Request`
             Request instance.
         resp : `falcon.Response`
             Response instance.
         scenario_id : `str`
             UUID of the scenario.
         """
         try:
-            if self.scenario_mgr.validate_uuid(scenario_id) is False:
-                self.send_invalid_resource_id_error(resp)
-                return
-
-            leakage = self.load_json_data_from_request(req)
-            if not isinstance(leakage, Leakage):
-                self.send_json_parsing_error(resp)
-                return
-
-            self.scenario_mgr.get(scenario_id).add_leakage(leakage)
+            args = self.load_json_data_from_request(req)
+            scenario_id = self.scenario_mgr.create(**args)
+            self.send_json_response(resp, {"scenario_id": scenario_id})
         except Exception as ex:
             warnings.warn(str(ex))
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
 
 
 class ScenarioTopologyHandler(ScenarioBaseHandler):
     """
@@ -233,14 +251,16 @@
 
     def on_post(self, req: falcon.Request, resp: falcon.Response, scenario_id: str) -> None:
         """
         Sets the general parameters of a given scenario.
 
         Parameters
         ----------
+        req : `falcon.Request`
+            Request instance.
         resp : `falcon.Request`
             Request instance.
         scenario_id : `str`
             UUID of the scenario.
         """
         try:
             if self.scenario_mgr.validate_uuid(scenario_id) is False:
@@ -286,14 +306,16 @@
 
     def on_post(self, req: falcon.Request, resp: falcon.Response, scenario_id: str) -> None:
         """
         Sets the sensor configuration of a given scenario.
 
         Parameters
         ----------
+        req : `falcon.Request`
+            Request instance.
         resp : `falcon.Request`
             Request instance.
         scenario_id : `str`
             UUID of the scenario.
         """
         try:
             if self.scenario_mgr.validate_uuid(scenario_id) is False:
@@ -308,45 +330,42 @@
             my_scenario = self.scenario_mgr.get(scenario_id)
             my_scenario.sensor_config = sensor_config
         except Exception as ex:
             warnings.warn(str(ex))
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
 
 
-class ScenarioSimulationHandler(ScenarioBaseHandler):
+class ScenarioNodeDemandPatternHandler(ScenarioBaseHandler):
     """
-    Class for handling GET requests for simulating a given scenario.
-
-    Parameters
-    ----------
-    scada_data_mgr : :class:`~epyt_flow.rest_api.scenario_handler.ScadaDataBaseHandler`
-        SCADA data manager.
+    Class for handling POST requests for node demand patterns of a given scenario.
     """
-    def __init__(self, scada_data_mgr: ScadaDataManager, **kwds):
-        self.scada_data_mgr = scada_data_mgr
-
-        super().__init__(**kwds)
-
-    def on_get(self, _, resp: falcon.Response, scenario_id: str) -> None:
+    def on_post(self, req: falcon.Request, resp: falcon.Response, scenario_id: str,
+                node_id: str) -> None:
         """
-        Runs the simulation of a given scenario.
+        Sets the demand pattern of a specific node in a given scenario.
 
         Parameters
         ----------
+        req : `falcon.Request`
+            Request instance.
         resp : `falcon.Response`
             Response instance.
         scenario_id : `str`
             UUID of the scenario.
+        node_id : `str`
+            ID of the node.
         """
         try:
             if self.scenario_mgr.validate_uuid(scenario_id) is False:
                 self.send_invalid_resource_id_error(resp)
                 return
 
-            my_scenario = self.scenario_mgr.get(scenario_id)
-            res = my_scenario.run_simulation()
+            params = self.load_json_data_from_request(req)
 
-            data_id = self.scada_data_mgr.create_new_item(res)
-            self.send_json_response(resp, {"data_id": data_id})
+            my_scenario = self.scenario_mgr.get(scenario_id)
+            my_scenario.set_node_demand_pattern(node_id, params["base_demand"],
+                                                params["demand_pattern_id"],
+                                                params["demand_pattern"])
         except Exception as ex:
             warnings.warn(str(ex))
+            resp.data = str(ex)
             resp.status = falcon.HTTP_INTERNAL_SERVER_ERROR
```

### Comparing `epyt_flow-0.1.1/epyt_flow/serialization.py` & `epyt_flow-0.2.0/epyt_flow/serialization.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/actuator_events.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/actuator_events.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/event.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/leakages.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/leakages.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_faults.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_faults.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_attack.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_reading_attack.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/sensor_reading_event.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/sensor_reading_event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/events/system_event.py` & `epyt_flow-0.2.0/epyt_flow/simulation/events/system_event.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/parallel_simulation.py` & `epyt_flow-0.2.0/epyt_flow/simulation/parallel_simulation.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scada/advanced_control.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scada/advanced_control.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scada/scada_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,29 +114,29 @@
         The default is None.
     frozen_sensor_config : `bool`, optional
         If True, the sensor config can not be changed and only the required sensor nodes/links
         will be stored -- this usually leads to a significant reduction in memory consumption.
 
         The default is False.
     """
-
     def __init__(self, sensor_config: SensorConfig, sensor_readings_time: np.ndarray,
                  pressure_data_raw: np.ndarray = None, flow_data_raw: np.ndarray = None,
                  demand_data_raw: np.ndarray = None, node_quality_data_raw: np.ndarray = None,
                  link_quality_data_raw: np.ndarray = None, pumps_state_data_raw: np.ndarray = None,
                  valves_state_data_raw: np.ndarray = None, tanks_volume_data_raw: np.ndarray = None,
                  surface_species_concentration_raw: np.ndarray = None,
                  bulk_species_node_concentration_raw: np.ndarray = None,
                  bulk_species_link_concentration_raw: np.ndarray = None,
                  pump_energy_usage_data: np.ndarray = None,
                  pump_efficiency_data: np.ndarray = None,
                  sensor_faults: list[SensorFault] = [],
                  sensor_reading_attacks: list[SensorReadingAttack] = [],
                  sensor_reading_events: list[SensorReadingEvent] = [],
-                 sensor_noise: SensorNoise = None, frozen_sensor_config: bool = False, **kwds):
+                 sensor_noise: SensorNoise = None, frozen_sensor_config: bool = False,
+                 **kwds):
         if not isinstance(sensor_config, SensorConfig):
             raise TypeError("'sensor_config' must be an instance of " +
                             "'epyt_flow.simulation.SensorConfig' but not of " +
                             f"'{type(sensor_config)}'")
         if not isinstance(sensor_readings_time, np.ndarray):
             raise TypeError("'sensor_readings_time' must be an instance of 'numpy.ndarray' " +
                             f"but not of '{type(sensor_readings_time)}'")
```

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scada/scada_data_export.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scada/scada_data_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,15 @@
         Returns
         -------
         :class:`~epyt_flow.simulation.sensor_config.SensorConfig`
             Global sensor configuration.
         """
         old_sensor_config = scada_data.sensor_config
 
-        sensor_config = SensorConfig(nodes=old_sensor_config.nodes,
-                                     links=old_sensor_config.links,
-                                     valves=old_sensor_config.valves,
-                                     pumps=old_sensor_config.pumps,
-                                     tanks=old_sensor_config.tanks,
-                                     bulk_species=old_sensor_config.bulk_species,
-                                     surface_species=old_sensor_config.surface_species)
+        sensor_config = SensorConfig.create_empty_sensor_config(old_sensor_config)
         sensor_config.pressure_sensors = sensor_config.nodes
         sensor_config.flow_sensors = sensor_config.links
         sensor_config.demand_sensors = sensor_config.nodes
         sensor_config.quality_node_sensors = sensor_config.nodes
         sensor_config.quality_link_sensors = sensor_config.links
         sensor_config.valve_state_sensors = sensor_config.valves
         sensor_config.tank_level_sensors = sensor_config.tanks
```

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scenario_config.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scenario_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,31 +578,25 @@
             sensor_faults = [parse_sensor_fault(sensor_fault)
                              for sensor_fault in data["sensor_faults"]]
 
         #  Load .inp file to get a list of all nodes and links/pipes
         sensor_config = None
         from .scenario_simulator import ScenarioSimulator
         with ScenarioSimulator(f_inp_in) as scenario:
-            sensor_config = SensorConfig(nodes=scenario.sensor_config.nodes,
-                                         links=scenario.sensor_config.links,
-                                         valves=scenario.sensor_config.valves,
-                                         pumps=scenario.sensor_config.pumps,
-                                         tanks=scenario.sensor_config.tanks,
-                                         bulk_species=scenario.sensor_config.bulk_species,
-                                         surface_species=scenario.sensor_config.surface_species,
-                                         pressure_sensors=pressure_sensors,
-                                         flow_sensors=flow_sensors,
-                                         demand_sensors=demand_sensors,
-                                         quality_node_sensors=node_quality_sensors,
-                                         quality_link_sensors=link_quality_sensors,
-                                         valve_state_sensors=valve_state_sensors,
-                                         pump_state_sensors=pump_state_sensors,
-                                         tank_volume_sensors=tank_volume_sensors,
-                                         bulk_species_node_sensors=bulk_species_node_sensors,
-                                         bulk_species_link_sensors=bulk_species_link_sensors,
-                                         surface_species_sensors=surface_species_sensors)
+            sensor_config = SensorConfig.create_empty_sensor_config(scenario.sensor_config)
+            sensor_config.pressure_sensors = pressure_sensors
+            sensor_config.flow_sensors = flow_sensors
+            sensor_config.demand_sensors = demand_sensors
+            sensor_config.quality_node_sensors = node_quality_sensors
+            sensor_config.quality_link_sensors = link_quality_sensors
+            sensor_config.valve_state_sensors = valve_state_sensors
+            sensor_config.pump_state_sensors = pump_state_sensors
+            sensor_config.tank_volume_sensors = tank_volume_sensors
+            sensor_config.bulk_species_node_sensors = bulk_species_node_sensors
+            sensor_config.bulk_species_link_sensors = bulk_species_link_sensors
+            sensor_config.surface_species_sensors = surface_species_sensors
 
         # Create final scenario configuration
         return ScenarioConfig(f_inp_in=f_inp_in, f_msx_in=f_msx_in, general_params=general_params,
                               sensor_config=sensor_config, controls=[], sensor_noise=sensor_noise,
                               model_uncertainty=model_uncertainty, system_events=leakages,
                               sensor_reading_events=sensor_faults)
```

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scenario_simulator.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scenario_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 import uuid
 import numpy as np
 from epyt import epanet
 from epyt.epanet import ToolkitConstants
 from tqdm import tqdm
 
 from .scenario_config import ScenarioConfig
-from .sensor_config import SensorConfig, SENSOR_TYPE_LINK_FLOW, SENSOR_TYPE_LINK_QUALITY, \
-    SENSOR_TYPE_NODE_DEMAND, SENSOR_TYPE_NODE_PRESSURE, SENSOR_TYPE_NODE_QUALITY, \
+from .sensor_config import SensorConfig, areaunit_to_id, massunit_to_id, qualityunits_to_id, \
+    qualityunits_to_str, MASS_UNIT_MG, \
+    SENSOR_TYPE_LINK_FLOW, SENSOR_TYPE_LINK_QUALITY, SENSOR_TYPE_NODE_DEMAND, \
+    SENSOR_TYPE_NODE_PRESSURE, SENSOR_TYPE_NODE_QUALITY, \
     SENSOR_TYPE_PUMP_STATE, SENSOR_TYPE_TANK_VOLUME, SENSOR_TYPE_VALVE_STATE, \
     SENSOR_TYPE_NODE_BULK_SPECIES, SENSOR_TYPE_LINK_BULK_SPECIES, SENSOR_TYPE_SURFACE_SPECIES
 from ..uncertainty import ModelUncertainty, SensorNoise
 from .events import SystemEvent, Leakage, ActuatorEvent, SensorFault, SensorReadingAttack, \
     SensorReadingEvent
 from .scada import ScadaData, AdvancedControlModule
-from ..topology import NetworkTopology
+from ..topology import NetworkTopology, UNITS_SIMETRIC, UNITS_USCUSTOM
 from ..utils import get_temp_folder
 
 
 class ScenarioSimulator():
     """
     Class for running a simulation of a water distribution network scenario.
 
@@ -44,23 +46,27 @@
 
         The default is None.
     scenario_config : :class:`~epyt_flow.simulation.scenario_config.ScenarioConfig`
         Configuration of the scenario -- i.e. a description of the scenario to be simulated.
 
         If this is None, then 'f_inp_in' must be set with a valid path to the .inp file
         that is to be simulated.
+    epanet_verbose : `bool`, optional
+        If True, EPyT is verbose and might print messages from time to time.
+
+        The default is False.
 
     Attributes
     ----------
     epanet_api : `epyt.epanet`
         API to EPANET and EPANET-MSX.
     """
 
     def __init__(self, f_inp_in: str = None, f_msx_in: str = None,
-                 scenario_config: ScenarioConfig = None):
+                 scenario_config: ScenarioConfig = None, epanet_verbose: bool = False):
         if f_msx_in is not None and f_inp_in is None:
             raise ValueError("'f_inp_in' must be set if 'f_msx_in' is set.")
         if f_inp_in is None and scenario_config is None:
             raise ValueError("Either 'f_inp_in' or 'scenario_config' must be set.")
         if f_inp_in is not None:
             if not isinstance(f_inp_in, str):
                 raise TypeError("'f_inp_in' must be an instance of 'str' but not of " +
@@ -70,57 +76,51 @@
                 raise TypeError("'f_msx_in' must be an instance of 'str' but not of " +
                                 f"'{type(f_msx_in)}'")
         if scenario_config is not None:
             if not isinstance(scenario_config, ScenarioConfig):
                 raise TypeError("'scenario_config' must be an instance of " +
                                 "'epyt_flow.simulation.ScenarioConfig' but not of " +
                                 f"'{type(scenario_config)}'")
+        if not isinstance(epanet_verbose, bool):
+            raise TypeError("'epanet_verbose' must be an instance of 'bool' " +
+                            f"but not of '{type(epanet_verbose)}'")
 
         self.__f_inp_in = f_inp_in if scenario_config is None else scenario_config.f_inp_in
         self.__f_msx_in = f_msx_in if scenario_config is None else scenario_config.f_msx_in
         self.__model_uncertainty = ModelUncertainty()
         self.__sensor_noise = None
         self.__sensor_config = None
         self.__controls = []
         self.__system_events = []
         self.__sensor_reading_events = []
 
         custom_epanet_lib = None
         custom_epanetmsx_lib = None
-        if sys.platform.startswith("linux"):
+        if sys.platform.startswith("linux") or sys.platform.startswith("darwin") :
             path_to_custom_libs = os.path.join(pathlib.Path(__file__).parent.resolve(),
                                                "..", "customlibs")
 
-            if os.path.isfile(os.path.join(path_to_custom_libs, "libepanet2_2.so")):
-                custom_epanet_lib = os.path.join(path_to_custom_libs, "libepanet2_2.so")
-            if os.path.isfile(os.path.join(path_to_custom_libs, "libepanetmsx2_2_0.so")):
-                custom_epanetmsx_lib = os.path.join(path_to_custom_libs, "libepanetmsx2_2_0.so")
+            libepanet_name = "libepanet2_2.so" if sys.platform.startswith("linux") \
+                else "libepanet2_2.dylib"
+            libepanetmsx_name = "libepanetmsx2_2_0.so" if sys.platform.startswith("linux") \
+                else "libepanetmsx2_2_0.dylib"
+
+            if os.path.isfile(os.path.join(path_to_custom_libs, libepanet_name)):
+                custom_epanet_lib = os.path.join(path_to_custom_libs, libepanet_name)
+            if os.path.isfile(os.path.join(path_to_custom_libs, libepanetmsx_name)):
+                custom_epanetmsx_lib = os.path.join(path_to_custom_libs, libepanetmsx_name)
 
         self.epanet_api = epanet(self.__f_inp_in, ph=self.__f_msx_in is None,
-                                 customlib=custom_epanet_lib)
+                                 customlib=custom_epanet_lib, loadfile=True,
+                                 display_msg=epanet_verbose)
 
-        bulk_species = []
-        surface_species = []
         if self.__f_msx_in is not None:
             self.epanet_api.loadMSXFile(self.__f_msx_in, customMSXlib=custom_epanetmsx_lib)
 
-            for species_id, species_type in zip(self.epanet_api.getMSXSpeciesNameID(),
-                                                self.epanet_api.getMSXSpeciesType()):
-                if species_type == "BULK":
-                    bulk_species.append(species_id)
-                elif species_type == "WALL":
-                    surface_species.append(species_id)
-
-        self.__sensor_config = SensorConfig(nodes=self.epanet_api.getNodeNameID(),
-                                            links=self.epanet_api.getLinkNameID(),
-                                            valves=self.epanet_api.getLinkValveNameID(),
-                                            pumps=self.epanet_api.getLinkPumpNameID(),
-                                            tanks=self.epanet_api.getNodeTankNameID(),
-                                            bulk_species=bulk_species,
-                                            surface_species=surface_species)
+        self.__sensor_config = self.__get_empty_sensor_config()
         if scenario_config is not None:
             if scenario_config.general_params is not None:
                 self.set_general_parameters(**scenario_config.general_params)
 
             self.__model_uncertainty = scenario_config.model_uncertainty
             self.__sensor_noise = scenario_config.sensor_noise
             self.__sensor_config = scenario_config.sensor_config
@@ -128,14 +128,59 @@
             for control in scenario_config.controls:
                 self.add_control(control)
             for event in scenario_config.system_events:
                 self.add_system_event(event)
             for event in scenario_config.sensor_reading_events:
                 self.add_sensor_reading_event(event)
 
+    def __get_empty_sensor_config(self, node_id_to_idx: dict = None, link_id_to_idx: dict = None,
+                                  valve_id_to_idx: dict = None, pump_id_to_idx: dict = None,
+                                  tank_id_to_idx: dict = None, bulkspecies_id_to_idx: dict = None,
+                                  surfacespecies_id_to_idx: dict = None) -> SensorConfig:
+        flow_unit = self.epanet_api.api.ENgetflowunits()
+        quality_unit = qualityunits_to_id(self.epanet_api.getQualityInfo().QualityChemUnits)
+        bulk_species = []
+        surface_species = []
+        bulk_species_mass_unit = []
+        surface_species_mass_unit = []
+        surface_species_area_unit = None
+
+        if self.__f_msx_in is not None:
+            surface_species_area_unit = areaunit_to_id(self.epanet_api.getMSXAreaUnits())
+
+            for species_id, species_type, mass_unit in zip(self.epanet_api.getMSXSpeciesNameID(),
+                                                           self.epanet_api.getMSXSpeciesType(),
+                                                           self.epanet_api.getMSXSpeciesUnits()):
+                if species_type == "BULK":
+                    bulk_species.append(species_id)
+                    bulk_species_mass_unit.append(massunit_to_id(mass_unit))
+                elif species_type == "WALL":
+                    surface_species.append(species_id)
+                    surface_species_mass_unit.append(massunit_to_id(mass_unit))
+
+        return SensorConfig(nodes=self.epanet_api.getNodeNameID(),
+                            links=self.epanet_api.getLinkNameID(),
+                            valves=self.epanet_api.getLinkValveNameID(),
+                            pumps=self.epanet_api.getLinkPumpNameID(),
+                            tanks=self.epanet_api.getNodeTankNameID(),
+                            bulk_species=bulk_species,
+                            surface_species=surface_species,
+                            flow_unit=flow_unit,
+                            quality_unit=quality_unit,
+                            bulk_species_mass_unit=bulk_species_mass_unit,
+                            surface_species_mass_unit=surface_species_mass_unit,
+                            surface_species_area_unit=surface_species_area_unit,
+                            node_id_to_idx=node_id_to_idx,
+                            link_id_to_idx=link_id_to_idx,
+                            valve_id_to_idx=valve_id_to_idx,
+                            pump_id_to_idx=pump_id_to_idx,
+                            tank_id_to_idx=tank_id_to_idx,
+                            bulkspecies_id_to_idx=bulkspecies_id_to_idx,
+                            surfacespecies_id_to_idx=surfacespecies_id_to_idx)
+
     @property
     def f_inp_in(self) -> str:
         """
         Gets the path to the .inp file.
 
         Returns
         -------
@@ -292,14 +337,29 @@
         """
         self.__adapt_to_network_changes()
 
         return deepcopy(list(filter(lambda e: isinstance(e, SensorFault),
                                     self.__sensor_reading_events)))
 
     @property
+    def sensor_reading_attacks(self) -> list[SensorReadingAttack]:
+        """
+        Gets all sensor reading attacks.
+
+        Returns
+        -------
+        list[:class:`~epyt_flow.simulation.events.sensor_reading_attacks.SensorReadingAttack`]
+            All sensor reading attacks.
+        """
+        self.__adapt_to_network_changes()
+
+        return deepcopy(list(filter(lambda e: isinstance(e, SensorReadingAttack)),
+                             self.__sensor_reading_events))
+
+    @property
     def sensor_reading_events(self) -> list[SensorReadingEvent]:
         """
         Gets all sensor reading events (e.g. sensor faults, etc.).
 
         Returns
         -------
         list[:class:`~epyt_flow.simulation.events.sensor_reading_event.SensorReadingEvent`]
@@ -308,65 +368,41 @@
         self.__adapt_to_network_changes()
 
         return deepcopy(self.__sensor_reading_events)
 
     def __adapt_to_network_changes(self):
         nodes = self.epanet_api.getNodeNameID()
         links = self.epanet_api.getLinkNameID()
-        valves = self.epanet_api.getLinkValveNameID()
-        pumps = self.epanet_api.getLinkPumpNameID()
-        tanks = self.epanet_api.getNodeTankNameID()
-        bulk_species = []
-        surface_species = []
-
-        if self.__f_msx_in is not None:
-            for species_id, species_type in zip(self.epanet_api.getMSXSpeciesNameID(),
-                                                self.epanet_api.getMSXSpeciesType()):
-                if species_type == "BULK":
-                    bulk_species.append(species_id)
-                elif species_type == "WALL":
-                    surface_species.append(species_id)
 
         node_id_to_idx = {node_id: self.epanet_api.getNodeIndex(node_id) - 1 for node_id in nodes}
         link_id_to_idx = {link_id: self.epanet_api.getLinkIndex(link_id) - 1 for link_id in links}
         valve_id_to_idx = None  # {valve_id: self.epanet_api.getLinkValveIndex(valve_id) for valve_id in valves}
         pump_id_to_idx = None  # {pump_id: self.epanet_api.getLinkPumpIndex(pump_id) - 1 for pump_id in pumps}
         tank_id_to_idx = None  # {tank_id: self.epanet_api.getNodeTankIndex(tank_id) - 1 for tank_id in tanks}
         bulkspecies_id_to_idx = None
         surfacespecies_id_to_idx = None
 
-        if nodes != self.__sensor_config.nodes or links != self.__sensor_config.links or \
-                valves != self.__sensor_config.valves or pumps != self.__sensor_config.pumps or \
-                tanks != self.__sensor_config.tanks or \
-                bulk_species != self.__sensor_config.bulk_species or \
-                surface_species != self.__sensor_config.surface_species:
-            # Adapt sensor configuration if anything in the network topology changed
-            new_sensor_config = SensorConfig(nodes=nodes, links=links, valves=valves, pumps=pumps,
-                                             tanks=tanks, bulk_species=bulk_species,
-                                             surface_species=surface_species,
-                                             node_id_to_idx=node_id_to_idx,
-                                             link_id_to_idx=link_id_to_idx,
-                                             valve_id_to_idx=valve_id_to_idx,
-                                             pump_id_to_idx=pump_id_to_idx,
-                                             tank_id_to_idx=tank_id_to_idx,
-                                             bulkspecies_id_to_idx=bulkspecies_id_to_idx,
-                                             surfacespecies_id_to_idx=surfacespecies_id_to_idx)
-            new_sensor_config.pressure_sensors = self.__sensor_config.pressure_sensors
-            new_sensor_config.flow_sensors = self.__sensor_config.flow_sensors
-            new_sensor_config.demand_sensors = self.__sensor_config.demand_sensors
-            new_sensor_config.quality_node_sensors = self.__sensor_config.quality_node_sensors
-            new_sensor_config.quality_link_sensors = self.__sensor_config.quality_link_sensors
-            new_sensor_config.pump_state_sensors = self.__sensor_config.pump_state_sensors
-            new_sensor_config.valve_state_sensors = self.__sensor_config.valve_state_sensors
-            new_sensor_config.tank_volume_sensors = self.__sensor_config.tank_volume_sensors
-            new_sensor_config.bulk_species_node_sensors = self.__sensor_config.bulk_species_node_sensors
-            new_sensor_config.bulk_species_link_sensors = self.__sensor_config.bulk_species_link_sensors
-            new_sensor_config.surface_species_sensors = self.__sensor_config.surface_species_sensors
+        # Adapt sensor configuration to potential cahnges in the network's topology
+        new_sensor_config = self.__get_empty_sensor_config(node_id_to_idx, link_id_to_idx,
+                                                           valve_id_to_idx, pump_id_to_idx,
+                                                           tank_id_to_idx, bulkspecies_id_to_idx,
+                                                           surfacespecies_id_to_idx)
+        new_sensor_config.pressure_sensors = self.__sensor_config.pressure_sensors
+        new_sensor_config.flow_sensors = self.__sensor_config.flow_sensors
+        new_sensor_config.demand_sensors = self.__sensor_config.demand_sensors
+        new_sensor_config.quality_node_sensors = self.__sensor_config.quality_node_sensors
+        new_sensor_config.quality_link_sensors = self.__sensor_config.quality_link_sensors
+        new_sensor_config.pump_state_sensors = self.__sensor_config.pump_state_sensors
+        new_sensor_config.valve_state_sensors = self.__sensor_config.valve_state_sensors
+        new_sensor_config.tank_volume_sensors = self.__sensor_config.tank_volume_sensors
+        new_sensor_config.bulk_species_node_sensors = self.__sensor_config.bulk_species_node_sensors
+        new_sensor_config.bulk_species_link_sensors = self.__sensor_config.bulk_species_link_sensors
+        new_sensor_config.surface_species_sensors = self.__sensor_config.surface_species_sensors
 
-            self.__sensor_config = new_sensor_config
+        self.__sensor_config = new_sensor_config
 
     def close(self):
         """
         Closes & unloads all resources and libraries.
 
         Call this function after the simulation is done -- do not call this function before!
         """
@@ -377,38 +413,222 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.close()
 
+    def save_to_epanet_file(self, inp_file_path: str, msx_file_path: str = None,
+                            export_sensor_config: bool = True) -> None:
+        """
+        Exports this scenario to EPANET files -- i.e. an .inp file
+        and (optionally) a .msx file if EPANET-MSX was loaded.
+
+        Parameters
+        ----------
+        inp_file_path : `str`
+            Path to the .inp file where this scenario will be stored.
+
+            If 'inp_file_path' is None, 'msx_file_path' must not be None!
+        msx_file_path : `str`, optional
+            Path to the .msx file where this MSX component of this scneario will be stored.
+
+            Note that this is only applicable if EPANET-MSX was loaded.
+
+            The default is None.
+        export_sensor_config : `bool`, optional
+            If True, the current sensor placement is exported as well.
+
+            The default is True.
+        """
+        if inp_file_path is None and msx_file_path is None:
+            raise ValueError("At least one of the paths (.inp and .msx) must not be None")
+        if inp_file_path is not None:
+            if not isinstance(inp_file_path, str):
+                raise TypeError("'inp_file_path' must be an instance of 'str' " +
+                                f"but not of '{type(inp_file_path)}'")
+        if msx_file_path is not None:
+            if not isinstance(msx_file_path, str):
+                raise TypeError("msx_file_path' msut be an instance of 'str' " +
+                                f"but not of {type(msx_file_path)}")
+        if not isinstance(export_sensor_config, bool):
+            raise TypeError("'export_sensor_config' must be an instance of 'bool' " +
+                            f"but not of '{type(export_sensor_config)}'")
+
+        def __override_report_section(file_in: str, report_desc: str) -> None:
+            with open(file_in, mode="r+", encoding="utf-8") as f_in:
+                # Find and remove exiting REPORT section
+                content = f_in.read()
+                try:
+                    report_section_start_idx = content.index("[REPORT]")
+                    report_section_end_idx = content.index("[", report_section_start_idx + 1)
+
+                    content = content[:report_section_start_idx] + content[report_section_end_idx:]
+                    f_in.seek(0)
+                    f_in.write(content)
+                    f_in.truncate()
+                except ValueError:
+                    pass
+
+                # Write new REPORT section in the very end of the file
+                write_end_section = False
+                try:
+                    end_idx = content.index("[END]")
+                    write_end_section = True
+                    f_in.seek(end_idx)
+                except ValueError:
+                    pass
+                f_in.write(report_desc)
+                if write_end_section is True:
+                    f_in.write("\n[END]")
+
+        if inp_file_path is not None:
+            self.epanet_api.saveInputFile(inp_file_path)
+
+            if export_sensor_config is True:
+                report_desc = "\n\n[REPORT]\n"
+                report_desc += "ENERGY YES\n"
+                report_desc += "STATUS YES\n"
+
+                nodes = []
+                links = []
+
+                # Parse sensor config
+                pressure_sensors = self.__sensor_config.pressure_sensors
+                if len(pressure_sensors) != 0:
+                    report_desc += "Pressure YES\n"
+                    nodes += pressure_sensors
+
+                flow_sensors = self.__sensor_config.flow_sensors
+                if len(flow_sensors) != 0:
+                    report_desc += "Flow YES\n"
+                    links += flow_sensors
+
+                demand_sensors = self.__sensor_config.demand_sensors
+                if len(demand_sensors) != 0:
+                    report_desc += "Demand YES\n"
+                    nodes += demand_sensors
+
+                node_quality_sensors = self.__sensor_config.quality_node_sensors
+                if len(node_quality_sensors) != 0:
+                    report_desc += "Quality YES\n"
+                    nodes += node_quality_sensors
+
+                link_quality_sensors = self.__sensor_config.quality_link_sensors
+                if len(link_quality_sensors) != 0:
+                    if len(node_quality_sensors) == 0:
+                        report_desc += "Quality YES\n"
+                    links += link_quality_sensors
+
+                # Create final REPORT section
+                nodes = list(set(nodes))
+                links = list(set(links))
+
+                if len(nodes) != 0:
+                    if set(nodes) == set(self.__sensor_config.nodes):
+                        nodes = ["ALL"]
+                    report_desc += f"NODES {' '.join(nodes)}\n"
+
+                if len(links) != 0:
+                    if set(links) == set(self.__sensor_config.links):
+                        links = ["ALL"]
+                    report_desc += f"LINKS {' '.join(links)}\n"
+
+                __override_report_section(inp_file_path, report_desc)
+
+        if self.__f_msx_in is not None and msx_file_path is not None:
+            self.epanet_api.saveMSXFile(msx_file_path)
+
+            if export_sensor_config is True:
+                report_desc = "\n\n[REPORT]\n"
+                species = []
+                nodes = []
+                links = []
+
+                # Parse sensor config
+                bulk_species_node_sensors = self.__sensor_config.bulk_species_node_sensors
+                for bulk_species_id in bulk_species_node_sensors.keys():
+                    species.append(bulk_species_id)
+                    nodes += bulk_species_node_sensors[bulk_species_id]
+
+                bulk_species_link_sensors = self.__sensor_config.bulk_species_link_sensors
+                for bulk_species_id in bulk_species_link_sensors.keys():
+                    species.append(bulk_species_id)
+                    links += bulk_species_link_sensors[bulk_species_id]
+
+                surface_species_link_sensors = self.__sensor_config.surface_species_sensors
+                for surface_species_id in surface_species_link_sensors.keys():
+                    species.append(surface_species_id)
+                    links += surface_species_link_sensors[surface_species_id]
+
+                nodes = list(set(nodes))
+                links = list((set(links)))
+                species = list(set(species))
+
+                # Create REPORT section
+                if len(nodes) != 0:
+                    if set(nodes) == set(self.__sensor_config.nodes):
+                        nodes = ["ALL"]
+                    report_desc += f"NODES {' '.join(nodes)}\n"
+
+                if len(links) != 0:
+                    if set(links) == set(self.__sensor_config.links):
+                        links = ["ALL"]
+                    report_desc += f"LINKS {' '.join(links)}\n"
+
+                for species_id in species:
+                    report_desc += f"SPECIES {species_id} YES\n"
+
+                __override_report_section(msx_file_path, report_desc)
+
     def get_flow_units(self) -> int:
         """
         Gets the flow units.
 
         Will be one of the following EPANET toolkit constants:
 
-            - EN_CFS = 0
-            - EN_GPM = 1
-            - EN_MGD = 2
-            - EN_IMGD = 3
-            - EN_AFD = 4
-            - EN_LPS = 5
-            - EN_LPM = 6
-            - EN_MLD = 7
-            - EN_CMH = 8
-            - EN_CMD = 9
+            - EN_CFS = 0 (cu foot/sec)
+            - EN_GPM = 1 (gal/min)
+            - EN_MGD = 2 (Million gal/day)
+            - EN_IMGD = 3 (Imperial MGD)
+            - EN_AFD = 4 (ac-foot/day)
+            - EN_LPS = 5 (liter/sec)
+            - EN_LPM = 6 (liter/min)
+            - EN_MLD = 7 (Megaliter/day)
+            - EN_CMH = 8 (cubic meter/hr)
+            - EN_CMD = 9 (cubic meter/day)
 
         Returns
         -------
         `int`
             Flow units.
         """
         return self.epanet_api.api.ENgetflowunits()
 
+    def get_units_category(self) -> int:
+        """
+        Gets the category of units -- i.e. US Customary or SI Metric units.
+
+        Will be one of the following constants:
+
+            - UNITS_USCUSTOM = 0  (US Customary)
+            - UNITS_SIMETRIC = 1  (SI Metric)
+
+        Returns
+        -------
+        `int`
+            Units category.
+        """
+        if self.get_flow_units() in [ToolkitConstants.EN_CFS, ToolkitConstants.EN_GPM,
+                                     ToolkitConstants.EN_MGD, ToolkitConstants.EN_IMGD,
+                                     ToolkitConstants.EN_AFD]:
+            return UNITS_USCUSTOM
+        else:
+            return UNITS_SIMETRIC
+
     def get_hydraulic_time_step(self) -> int:
         """
         Gets the hydraulic time step -- i.e. time step in the hydraulic simulation.
 
         Returns
         -------
         `int`
@@ -467,15 +687,15 @@
             Quality model.
         """
         qual_info = self.epanet_api.getQualityInfo()
 
         return {"code": qual_info.QualityCode,
                 "type": qual_info.QualityType,
                 "chemical_name": qual_info.QualityChemName,
-                "units": qual_info.QualityChemUnits,
+                "units": qualityunits_to_id(qual_info.QualityChemUnits),
                 "trace_node_id": qual_info.TraceNode}
 
     def get_scenario_config(self) -> ScenarioConfig:
         """
         Gets the configuration of this scenario -- i.e. all information & elements
         that completely describe this scenario.
 
@@ -514,14 +734,18 @@
         self.__adapt_to_network_changes()
 
         n_time_steps = int(self.epanet_api.getTimeSimulationDuration() /
                            self.epanet_api.getTimeReportingStep())
         n_quantities = self.epanet_api.getNodeCount() * 3 + self.epanet_api.getNodeTankCount() + \
                        self.epanet_api.getLinkValveCount() + self.epanet_api.getLinkPumpCount() + \
                        self.epanet_api.getLinkCount() * 2
+
+        if self.__f_msx_in is not None:
+            n_quantities += self.epanet_api.getLinkCount() * 2 + self.epanet_api.getNodeCount()
+
         n_bytes_per_quantity = 64
 
         return n_time_steps * n_quantities * n_bytes_per_quantity * .000001
 
     def get_topology(self) -> NetworkTopology:
         """
         Gets the topology (incl. information such as elevations, pipe diameters, etc.) of this WDN.
@@ -557,15 +781,16 @@
                 in zip(links_id, links_data, links_diameter, links_length, links_roughness_coeff,
                        links_bulk_coeff, links_wall_coeff, links_loss_coeff):
             links.append((link_id, link, {"diameter": diameter, "length": length,
                                           "roughness_coeff": roughness_coeff,
                                           "bulk_coeff": bulk_coeff, "wall_coeff": wall_coeff,
                                           "loss_coeff": loss_coeff}))
 
-        return NetworkTopology(f_inp=self.f_inp_in, nodes=nodes, links=links)
+        return NetworkTopology(f_inp=self.f_inp_in, nodes=nodes, links=links,
+                               units=self.get_units_category())
 
     def randomize_demands(self) -> None:
         """
         Randomizes all demand patterns.
         """
         self.__adapt_to_network_changes()
 
@@ -970,14 +1195,17 @@
             The default is False.
 
         Returns
         -------
         :class:`~epyt_flow.simulation.scada.scada_data.ScadaData`
             Quality simulation results as SCADA data.
         """
+        if self.__f_msx_in is None:
+            raise ValueError("No .msx file specified")
+
         result = None
 
         gen = self.run_advanced_quality_simulation_as_generator
         for scada_data in gen(hyd_file_in=hyd_file_in,
                               verbose=verbose,
                               return_as_dict=True,
                               frozen_sensor_config=frozen_sensor_config):
@@ -1031,14 +1259,17 @@
 
         Returns
         -------
         :class:`~epyt_flow.simulation.scada.scada_data.ScadaData`
             Generator containing the current EPANET-MSX simulation results as SCADA data
             (i.e. species concentrations).
         """
+        if self.__f_msx_in is None:
+            raise ValueError("No .msx file specified")
+
         # Load pre-computed hydraulics
         self.epanet_api.useMSXHydraulicFile(hyd_file_in)
 
         # Initialize simulation
         n_nodes = self.epanet_api.getNodeCount()
         n_links = self.epanet_api.getLinkCount()
 
@@ -1657,24 +1888,24 @@
             The default is None.
         flow_units : `int`, optional
             Specifies the flow units -- i.e. all flows will be reported in these units.
             If None, the units from the .inp file will be used.
 
             Must be one of the following EPANET toolkit constants:
 
-                - EN_CFS = 0
-                - EN_GPM = 1
-                - EN_MGD = 2
-                - EN_IMGD = 3
-                - EN_AFD = 4
-                - EN_LPS = 5
-                - EN_LPM = 6
-                - EN_MLD = 7
-                - EN_CMH = 8
-                - EN_CMD = 9
+                - EN_CFS = 0 (cu foot/sec)
+                - EN_GPM = 1 (gal/min)
+                - EN_MGD = 2 (Million gal/day)
+                - EN_IMGD = 3 (Imperial MGD)
+                - EN_AFD = 4 (ac-foot/day)
+                - EN_LPS = 5 (liter/sec)
+                - EN_LPM = 6 (liter/min)
+                - EN_MLD = 7 (Megaliter/day)
+                - EN_CMH = 8 (cubic meter/hr)
+                - EN_CMD = 9 (cubic meter/day)
 
             The default is None.
         quality_model : `dict`, optional
             Specifies the quality model -- the dictionary must contain,
             "type", "chemical_name", "chemical_units", and "trace_node_id", of the
             requested quality model.
 
@@ -1754,15 +1985,15 @@
         if quality_model is not None:
             if quality_model["type"] == "NONE":
                 self.epanet_api.setQualityType("none")
             elif quality_model["type"] == "AGE":
                 self.epanet_api.setQualityType("age")
             elif quality_model["type"] == "CHEM":
                 self.epanet_api.setQualityType("chem", quality_model["chemical_name"],
-                                               quality_model["units"])
+                                               qualityunits_to_str(quality_model["units"]))
             elif quality_model["type"] == "TRACE":
                 self.epanet_api.setQualityType("trace", quality_model["trace_node_id"])
             else:
                 raise ValueError(f"Unknown quality type: {quality_model['type']}")
 
     def get_events_active_time_points(self) -> list[int]:
         """
@@ -1805,31 +2036,35 @@
         """
         self.__adapt_to_network_changes()
 
         self.__warn_if_quality_set()
         self.set_general_parameters(quality_model={"type": "AGE"})
 
     def enable_chemical_analysis(self, chemical_name: str = "Chlorine",
-                                 chemical_units: str = "mg/L") -> None:
+                                 chemical_units: int = MASS_UNIT_MG) -> None:
         """
         Sets chemical analysis.
 
         ATTENTION: Do not forget to inject this chemical into the WDN.
 
         Parameters
         ----------
         chemical_name : `str`, optional
             Name of the chemical being analyzed.
 
             The default is "Chlorine".
         chemical_units : `str`, optional
             Units that the chemical is measured in.
-            Either "mg/L" or "ug/L".
 
-            The default is "mg/L".
+            Must be one of the following constants:
+
+                - MASS_UNIT_MG = 4  (mg/L)
+                - MASS_UNIT_UG = 5  (ug/L)
+
+            The default is MASS_UNIT_MG.
         """
         self.__adapt_to_network_changes()
 
         self.__warn_if_quality_set()
         self.set_general_parameters(quality_model={"type": "CHEM", "chemical_name": chemical_name,
                                                    "units": chemical_units})
```

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/scenario_visualizer.py` & `epyt_flow-0.2.0/epyt_flow/simulation/scenario_visualizer.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/simulation/sensor_config.py` & `epyt_flow-0.2.0/epyt_flow/simulation/sensor_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Module provides a class for implementing sensor configurations.
 """
 from copy import deepcopy
+import warnings
 import numpy as np
 import epyt
 
 from ..serialization import SENSOR_CONFIG_ID, JsonSerializable, serializable
 
 
 SENSOR_TYPE_NODE_PRESSURE     = 1
@@ -16,14 +17,123 @@
 SENSOR_TYPE_VALVE_STATE       = 6
 SENSOR_TYPE_PUMP_STATE        = 7
 SENSOR_TYPE_TANK_VOLUME       = 8
 SENSOR_TYPE_NODE_BULK_SPECIES = 9
 SENSOR_TYPE_LINK_BULK_SPECIES = 10
 SENSOR_TYPE_SURFACE_SPECIES   = 11
 
+AREA_UNIT_FT2 = 1
+AREA_UNIT_M2 = 2
+AREA_UNIT_CM2 = 3
+MASS_UNIT_MG = 4
+MASS_UNIT_UG = 5
+MASS_UNIT_MOL = 6
+MASS_UNIT_MMOL = 7
+TIME_UNIT_HRS = 8
+
+
+def areaunit_to_id(unit_desc: str) -> int:
+    """
+    Converts a given area units string to the corresponding ID.
+
+    Parameters
+    ----------
+    unit_desc : `str`
+        Area units string.
+
+    Returns
+    -------
+    `int`
+        Corresponding area unit ID.
+    """
+    return {"FT2": AREA_UNIT_FT2,
+            "M2": AREA_UNIT_M2,
+            "CM2": AREA_UNIT_CM2}[unit_desc]
+
+
+def massunit_to_id(unit_desc: str) -> int:
+    """
+    Converts a given mass units string to the corresponding ID.
+
+    Parameters
+    ----------
+    unit_desc : `str`
+        Mass units string.
+
+    Returns
+    -------
+    `int`
+        Corresponding mass unit ID.
+    """
+    return {"MG": MASS_UNIT_MG,
+            "UG": MASS_UNIT_UG,
+            "MOL": MASS_UNIT_MOL,
+            "MMOL": MASS_UNIT_MMOL}[unit_desc]
+
+
+def qualityunits_to_id(unit_desc: str) -> int:
+    """
+    Converts a given measurement unit description to the corresponding mass unit ID.
+
+    Parameters
+    ----------
+    unit_desc : `str`
+        Mass unit.
+
+    Returns
+    -------
+    `int`
+        Mass unit ID.
+
+        Will be either None (if no water quality analysis was set up) or
+        one of the following constants:
+
+            - MASS_UNIT_MG = 4   (mg/L)
+            - MASS_UNIT_UG = 5   (ug/L)
+            - TIME_UNIT_HRS = 8  (hrs)
+    """
+    if unit_desc == "mg/L":
+        return MASS_UNIT_MG
+    elif unit_desc == "ug/L":
+        return MASS_UNIT_UG
+    elif unit_desc == "hrs":
+        return TIME_UNIT_HRS
+    else:
+        return None
+
+
+def qualityunits_to_str(unit_id: int) -> str:
+    """
+    Converts a given measurement unit ID to the corresponding description.
+
+    Parameters
+    ----------
+    unit_id : `int`
+        ID of the mass unit.
+
+        Must be one of the following constants:
+
+            - MASS_UNIT_MG = 4  (mg/L)
+            - MASS_UNIT_UG = 5  (ug/L)
+            - TIME_UNIT_HRS = 8  (hrs)
+
+    Returns
+    -------
+    `str`
+        Mass unit description.
+    """
+    if unit_id == MASS_UNIT_MG:
+        return "mg/L"
+    elif unit_id == MASS_UNIT_UG:
+        return "ug/L"
+    elif unit_id == TIME_UNIT_HRS:
+        return "hrs"
+    else:
+        raise ValueError(f"Unknown unit ID '{unit_id}'")
+
 
 @serializable(SENSOR_CONFIG_ID, ".epytflow_sensor_config")
 class SensorConfig(JsonSerializable):
     """
     Class for storing a sensor configuration.
 
     Parameters
@@ -35,15 +145,15 @@
     valves : `list[str]`
         List of all valves (i.e. IDs) in the network.
     pumps : `list[str]`
         List of all pumps (i.e. IDs) in the network.
     tanks : `list[str]`
         List of all tanks (i.e. IDs) in the network.
     species : `list[str]`
-        List of all (EPANET-MSX) species (i.e. IDs) in the network    
+        List of all (EPANET-MSX) species (i.e. IDs) in the network
     pressure_sensors : `list[str]`, optional
         List of all nodes (i.e. IDs) at which a pressure sensor is placed.
 
         The default is an empty list.
     flow_sensors : `list[str]`, optional
         List of all links/pipes (i.e. IDs) at which a flow sensor is placed.
 
@@ -127,32 +237,93 @@
         Mapping of a surface species ID to the EPANET index
         (i.e. position in the raw sensor reading data).
 
         If None is given, it is assumed that the surface species (in 'surface_species') are
         sorted according to their EPANET index.
 
         The default is None.
+    flow_unit : `int`
+        Specifies the flow units and consequently all other hydraulic units
+        (US CUSTOMARY or SI METRIC) as well.
+
+        Must be one of the following EPANET toolkit constants:
+
+            - EN_CFS = 0 (cu foot/sec)
+            - EN_GPM = 1 (gal/min)
+            - EN_MGD = 2 (Million gal/day)
+            - EN_IMGD = 3 (Imperial MGD)
+            - EN_AFD = 4 (ac-foot/day)
+            - EN_LPS = 5 (liter/sec)
+            - EN_LPM = 6 (liter/min)
+            - EN_MLD = 7 (Megaliter/day)
+            - EN_CMH = 8 (cubic meter/hr)
+            - EN_CMD = 9 (cubic meter/day)
+    quality_unit : `str`, optional
+        Measurement unit (in a basic quality analysis) -- only relevant
+        if basic water quality is enabled.
+
+        Must be one of the following constants:
+
+            - MASS_UNIT_MG = 4     (mg/L)
+            - MASS_UNIT_UG = 5     (ug/L)
+            - TIME_UNIT_HRS = 8    (hrs)
+
+    bulk_species_mass_unit : `list[int]`, optional
+        Specifies the mass unit for each bulk species -- only relevant if EPANET-MSX is used.
+
+        Must be one of the following constants:
+
+            - MASS_UNIT_MG = 4      (milligram)
+            - MASS_UNIT_UG = 5      (microgram)
+            - MASS_UNIT_MOL = 6     (mole)
+            - MASS_UNIT_MMOL = 7    (millimole)
+
+        Note that the assumed ordering is the same as given in 'bulk_species'.
+    surface_species_mass_unit : `list[int]`, optional
+        Specifies the mass unit for each surface species -- only relevant if EPANET-MSX is used.
+
+        Must be one of the following constants:
+
+            - MASS_UNIT_MG = 4      (milligram)
+            - MASS_UNIT_UG = 5      (microgram)
+            - MASS_UNIT_MOL = 6     (mole)
+            - MASS_UNIT_MMOL = 7    (millimole)
+
+        Note that the assumed ordering is the same as given in 'surface_species'.
+    surface_species_area_unit : `int`, optional
+        Species the area unit of all surface species -- only relevant if EPANET-MSX is used.
+        Must be one of the following constants:
+
+            - AREA_UNIT_FT2 = 1     (square feet)
+            - AREA_UNIT_M2 = 2      (square meters)
+            - AREA_UNIT_CM2 = 3     (square centimeters)
     """
     def __init__(self, nodes: list[str], links: list[str], valves: list[str], pumps: list[str],
                  tanks: list[str], bulk_species: list[str], surface_species: list[str],
+                 flow_unit: int = None,
                  pressure_sensors: list[str] = [],
                  flow_sensors: list[str] = [],
                  demand_sensors: list[str] = [],
                  quality_node_sensors: list[str] = [],
                  quality_link_sensors: list[str] = [],
                  valve_state_sensors: list[str] = [],
                  pump_state_sensors: list[str] = [],
                  tank_volume_sensors: list[str] = [],
                  bulk_species_node_sensors: dict = {},
                  bulk_species_link_sensors: dict = {},
                  surface_species_sensors: dict = {},
                  node_id_to_idx: dict = None, link_id_to_idx: dict = None,
                  valve_id_to_idx: dict = None, pump_id_to_idx: dict = None,
                  tank_id_to_idx: dict = None, bulkspecies_id_to_idx: dict = None,
-                 surfacespecies_id_to_idx: dict = None, **kwds):
+                 surfacespecies_id_to_idx: dict = None,
+                 quality_unit: int = None,
+                 bulk_species_mass_unit : list[int] = [],
+                 surface_species_mass_unit : list[int] = [],
+                 surface_species_area_unit : int = None,
+                 **kwds):
         if not isinstance(nodes, list):
             raise TypeError("'nodes' must be an instance of 'list[str]' " +
                             f"but not of '{type(nodes)}'")
         if len(nodes) == 0:
             raise ValueError("'nodes' must be a list of all nodes (i.e. IDs) in the network.")
         if any(not isinstance(n, str) for n in nodes):
             raise TypeError("Each item in 'nodes' must be an instance of 'str' -- " +
@@ -325,14 +496,56 @@
         if surfacespecies_id_to_idx is not None:
             if not isinstance(surfacespecies_id_to_idx, dict):
                 raise TypeError("'surfacespecies_id_to_idx' must be an instance of 'dict' " +
                                 f"but not of '{type(surfacespecies_id_to_idx)}'")
             if any(s not in surface_species for s in surfacespecies_id_to_idx.keys()):
                 raise ValueError("Unknown surface species ID in 'surfacespecies_id_to_idx'")
 
+        if flow_unit is not None:
+            if not isinstance(flow_unit, int):
+                raise TypeError("'flow_unit' must be a an instance of 'int' " +
+                                f"but not of '{type(flow_unit)}'")
+            if flow_unit not in range(10):
+                raise ValueError("Invalid value of 'flow_unit'")
+        else:
+            warnings.warn("Loading a file that was created with an outdated version of EPyT-Flow" +
+                          " -- support of such old files will be removed in the next release!",
+                          DeprecationWarning)
+
+        if quality_unit is not None:
+            if not isinstance(quality_unit, int):
+                raise TypeError("'quality_mass_unit' must be an instance of 'int' " +
+                                f"but not of '{type(quality_unit)}'")
+            if quality_unit not in [MASS_UNIT_MG, MASS_UNIT_UG, TIME_UNIT_HRS]:
+                raise ValueError("Invalid value of 'quality_unit'")
+
+        if len(bulk_species_mass_unit) != len(bulk_species):
+            raise ValueError("Inconsistency between 'bulk_species_mass_unit' and 'bulk_species'")
+        if any(not isinstance(mass_unit, int) for mass_unit in bulk_species_mass_unit):
+            raise TypeError("All items in 'bulk_species_mass_unit' must be an instance of 'int'")
+        if any(mass_unit not in [MASS_UNIT_MG, MASS_UNIT_UG, MASS_UNIT_MOL, MASS_UNIT_MMOL]
+               for mass_unit in bulk_species_mass_unit):
+            raise ValueError("Invalid mass unit in 'bulk_species_mass_unit'")
+
+        if len(surface_species_mass_unit) != len(surface_species):
+            raise ValueError("Inconsistency between 'surface_species_mass_unit' " +
+                             "and 'surface_species'")
+        if any(not isinstance(mass_unit, int) for mass_unit in surface_species_mass_unit):
+            raise TypeError("All items in 'surface_species_mass_unit' must be an instance of 'int'")
+        if any(mass_unit not in [MASS_UNIT_MG, MASS_UNIT_UG, MASS_UNIT_MOL, MASS_UNIT_MMOL]
+               for mass_unit in surface_species_mass_unit):
+            raise ValueError("Invalid mass unit in 'surface_species_mass_unit'")
+
+        if surface_species_area_unit is not None:
+            if not isinstance(surface_species_area_unit, int):
+                raise TypeError("'surface_species_area_unit' must be a an instance of 'int' " +
+                                f"but not of '{type(surface_species_area_unit)}'")
+            if surface_species_area_unit not in [AREA_UNIT_FT2, AREA_UNIT_M2, AREA_UNIT_CM2]:
+                raise ValueError("Invalid area unit 'surface_species_area_unit'")
+
         self.__nodes = nodes
         self.__links = links
         self.__valves = valves
         self.__pumps = pumps
         self.__tanks = tanks
         self.__bulk_species = bulk_species
         self.__surface_species = surface_species
@@ -350,19 +563,53 @@
         self.__node_id_to_idx = node_id_to_idx
         self.__link_id_to_idx = link_id_to_idx
         self.__valve_id_to_idx = valve_id_to_idx
         self.__pump_id_to_idx = pump_id_to_idx
         self.__tank_id_to_idx = tank_id_to_idx
         self.__bulkspecies_id_to_idx = bulkspecies_id_to_idx
         self.__surfacespecies_id_to_idx = surfacespecies_id_to_idx
+        self.__flow_unit = flow_unit
+        self.__quality_unit = quality_unit
+        self.__bulk_species_mass_unit = bulk_species_mass_unit
+        self.__surface_species_mass_unit = surface_species_mass_unit
+        self.__surface_species_area_unit = surface_species_area_unit
 
         self.__compute_indices()    # Compute indices
 
         super().__init__(**kwds)
 
+    @staticmethod
+    def create_empty_sensor_config(sensor_config):
+        """
+        Creates an empty sensor configuration from a given sensor configuration
+        -- i.e. a clone of the given sensor configuration except that no sensors are set.
+
+        Parameters
+        ----------
+        sensor_config : :class:`epyt_flow.simulation.sensor_config.SensorConfig`
+            Sensor configuration used as a basis.
+
+        Returns
+        -------
+        :class:`epyt_flow.simulation.sensor_config.SensorConfig`
+            Empty sensor configuration.
+        """
+        return SensorConfig(nodes=sensor_config.nodes,
+                            links=sensor_config.links,
+                            valves=sensor_config.valves,
+                            pumps=sensor_config.pumps,
+                            tanks=sensor_config.tanks,
+                            flow_unit=sensor_config.flow_unit,
+                            quality_unit=sensor_config.quality_unit,
+                            bulk_species=sensor_config.bulk_species,
+                            surface_species=sensor_config.surface_species,
+                            bulk_species_mass_unit=sensor_config.bulk_species_mass_unit,
+                            surface_species_mass_unit=sensor_config.surface_species_mass_unit,
+                            surface_species_area_unit=sensor_config.surface_species_area_unit)
+
     def node_id_to_idx(self, node_id: str) -> int:
         """
         Gets the index of a given node ID.
 
         Parameters
         ----------
         node_id : `str`
@@ -698,14 +945,58 @@
         -------
         `list[str]`
             All tank IDs.
         """
         return self.__tanks.copy()
 
     @property
+    def flow_unit(self) -> int:
+        """
+        Gets the flow units.
+        Note that this specifies all other hydraulic units as well.
+
+        Will be one of the following EPANET toolkit constants:
+
+            - EN_CFS = 0 (cu foot/sec)
+            - EN_GPM = 1 (gal/min)
+            - EN_MGD = 2 (Million gal/day)
+            - EN_IMGD = 3 (Imperial MGD)
+            - EN_AFD = 4 (ac-foot/day)
+            - EN_LPS = 5 (liter/sec)
+            - EN_LPM = 6 (liter/min)
+            - EN_MLD = 7 (Megaliter/day)
+            - EN_CMH = 8 (cubic meter/hr)
+            - EN_CMD = 9 (cubic meter/day)
+
+        Returns
+        -------
+        `int`
+            Flow unit ID.
+        """
+        return self.__flow_unit
+
+    @property
+    def quality_unit(self) -> int:
+        """
+        Gets the measurement unit ID used in the basic quality analysis.
+
+        Will be one of the following constants:
+
+            - MASS_UNIT_MG = 4      (milligram)
+            - MASS_UNIT_UG = 5      (microgram)
+            - TIME_UNIT_HRS = 6     (hours)
+
+        Returns
+        -------
+        `int`
+            Mass unit ID.
+        """
+        return self.__quality_unit
+
+    @property
     def bulk_species(self) -> list[str]:
         """
         Gets all bulk species IDs -- i.e. species that live in the water.
 
         Returns
         -------
         `list[str]`
@@ -722,14 +1013,70 @@
         -------
         `list[str]`
             All species IDs.
         """
         return self.__surface_species.copy()
 
     @property
+    def bulk_species_mass_unit(self) -> list[int]:
+        """
+        Gets the mass unit of each bulk species.
+
+        Will be one of the following constants:
+
+            - MASS_UNIT_MG = 4      (milligram)
+            - MASS_UNIT_UG = 5      (microgram)
+            - MASS_UNIT_MOL = 6     (mole)
+            - MASS_UNIT_MMOL = 7    (millimole)
+
+        Returns
+        -------
+        `int`
+            Mass unit ID.
+        """
+        return self.__bulk_species_mass_unit
+
+    @property
+    def surface_species_mass_unit(self) -> list[int]:
+        """
+        Gets the mass unit of each surface species.
+
+        Will be one of the following constants:
+
+            - MASS_UNIT_MG = 4      (milligram)
+            - MASS_UNIT_UG = 5      (microgram)
+            - MASS_UNIT_MOL = 6     (mole)
+            - MASS_UNIT_MMOL = 7    (millimole)
+
+        Returns
+        -------
+        `int`
+            Mass unit ID.
+        """
+        return self.__surface_species_mass_unit
+
+    @property
+    def surface_species_area_unit(self) -> int:
+        """
+        Gets the surface species area unit.
+
+        Will be one of the following constants:
+
+            - AREA_UNIT_FT2 = 1     (square feet)
+            - AREA_UNIT_M2 = 2      (square meters)
+            - AREA_UNIT_CM2 = 3     (square centimeters)
+
+        Returns
+        -------
+        `int`
+            Area unit ID.
+        """
+        return self.__surface_species_area_unit
+
+    @property
     def pressure_sensors(self) -> list[str]:
         """
         Gets all pressure sensors (i.e. IDs of nodes at which a pressure sensor is placed).
 
         Returns
         -------
         `list[str]`
@@ -1038,15 +1385,20 @@
                 "surface_species_sensors": self.__surface_species_sensors,
                 "node_id_to_idx": self.__node_id_to_idx,
                 "link_id_to_idx": self.__link_id_to_idx,
                 "valve_id_to_idx": self.__valve_id_to_idx,
                 "pump_id_to_idx": self.__pump_id_to_idx,
                 "tank_id_to_idx": self.__tank_id_to_idx,
                 "bulkspecies_id_to_idx": self.__bulkspecies_id_to_idx,
-                "surfacespecies_id_to_idx": self.__surfacespecies_id_to_idx}
+                "surfacespecies_id_to_idx": self.__surfacespecies_id_to_idx,
+                "flow_unit": self.__flow_unit,
+                "quality_unit": self.__quality_unit,
+                "bulk_species_mass_unit": self.__bulk_species_mass_unit,
+                "surface_species_mass_unit": self.__surface_species_mass_unit,
+                "surface_species_area_unit": self.__surface_species_area_unit}
 
         return super().get_attributes() | attr
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, SensorConfig):
             raise TypeError("Can not compare 'SensorConfig' instance " +
                             f"with '{type(other)}' instance")
@@ -1061,30 +1413,39 @@
             and self.__quality_node_sensors == other.quality_node_sensors \
             and self.__quality_link_sensors == other.quality_link_sensors \
             and self.__valve_state_sensors == other.valve_state_sensors \
             and self.__pump_state_sensors == other.pump_state_sensors \
             and self.__tank_volume_sensors == other.tank_volume_sensors \
             and self.__bulk_species_node_sensors == other.bulk_species_node_sensors \
             and self.__bulk_species_link_sensors == other.bulk_species_link_sensors \
-            and self.__surface_species_sensors == other.surface_species_sensors
+            and self.__surface_species_sensors == other.surface_species_sensors \
+            and self.__flow_unit == other.flow_unit \
+            and self.__quality_unit == other.quality_unit \
+            and self.__bulk_species_mass_unit == other.bulk_species_mass_unit \
+            and self.__surface_species_mass_unit == other.surface_species_mass_unit \
+            and self.__surface_species_area_unit == other.surface_species_area_unit
 
     def __str__(self) -> str:
         return f"nodes: {self.__nodes} links: {self.__links} valves: {self.__valves} " +\
             f"pumps: {self.__pumps} tanks: {self.__tanks} bulk_species: {self.__bulk_species} " +\
             f"surface_species: {self.__surface_species}" + \
             f"pressure_sensors: {self.__pressure_sensors} flow_sensors: {self.__flow_sensors} " +\
             f"demand_sensors: {self.__demand_sensors} " +\
             f"quality_node_sensors: {self.__quality_node_sensors} " +\
             f"quality_link_sensors: {self.__quality_link_sensors} " +\
             f"valve_state_sensors: {self.__valve_state_sensors} " +\
             f"pump_state_sensors: {self.__pump_state_sensors} " +\
-            f"tank_volume_sensors: {self.__tank_volume_sensors}" +\
-            f"bulk_species_node_sensors: {self.__bulk_species_node_sensors}" +\
-            f"bulk_species_link_sensors: {self.__bulk_species_link_sensors}" +\
-            f"surface_species_sensors: {self.__surface_species_sensors}"
+            f"tank_volume_sensors: {self.__tank_volume_sensors} " +\
+            f"bulk_species_node_sensors: {self.__bulk_species_node_sensors} " +\
+            f"bulk_species_link_sensors: {self.__bulk_species_link_sensors} " +\
+            f"surface_species_sensors: {self.__surface_species_sensors} " +\
+            f"flow_unit: {self.__flow_unit} quality_unit: {self.__quality_unit}" +\
+            f"bulk_species_mass_unit: {self.__bulk_species_mass_unit} " +\
+            f"surface_species_mass_unit: {self.__surface_species_mass_unit} " +\
+            f"surface_species_area_unit: {self.__surface_species_area_unit}"
 
     def compute_readings(self, pressures: np.ndarray, flows: np.ndarray, demands: np.ndarray,
                          nodes_quality: np.ndarray, links_quality: np.ndarray,
                          pumps_state: np.ndarray, valves_state: np.ndarray,
                          tanks_volume: np.ndarray, bulk_species_node_concentrations: np.ndarray,
                          bulk_species_link_concentrations: np.ndarray,
                          surface_species_concentrations: np.ndarray) -> np.ndarray:
```

### Comparing `epyt_flow-0.1.1/epyt_flow/topology.py` & `epyt_flow-0.2.0/epyt_flow/topology.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 """
 Module provides a class for representing the topology of WDN.
 """
+from copy import deepcopy
+import warnings
 import numpy as np
 import networkx as nx
 from scipy.sparse import bsr_array
 
 from .serialization import serializable, JsonSerializable, NETWORK_TOPOLOGY_ID
 
 
+UNITS_USCUSTOM = 0
+UNITS_SIMETRIC = 1
+
+
 @serializable(NETWORK_TOPOLOGY_ID, ".epytflow_topology")
 class NetworkTopology(nx.Graph, JsonSerializable):
     """
     Class representing the topology of a WDN.
 
     Parameters
     ----------
     f_inp : `str`
         Path to .inp file to which this topology belongs.
     nodes : `list[tuple[str, dict]]`
         List of all nodes -- i.e. node ID and node information such as type and elevation.
     links : `list[tuple[tuple[str, str], dict]]`
         List of all links/pipes -- i.e. link ID, ID of connecting nodes, and link information
         such as pipe diameter, length, etc.
+    units : `int`
+        Measurement units category.
+
+        Must be one of the following constants:
+
+            - UNITS_USCUSTOM = 0  (US Customary)
+            - UNITS_SIMETRIC = 1  (SI Metric)
     """
     def __init__(self, f_inp: str, nodes: list[tuple[str, dict]],
-                 links: list[tuple[str, tuple[str, str], dict]], **kwds):
+                 links: list[tuple[str, tuple[str, str], dict]],
+                 units: int = None,
+                 **kwds):
         super().__init__(name=f_inp, **kwds)
 
         self.__nodes = nodes
         self.__links = links
+        self.__units = units
+
+        if units is None:
+            warnings.warn("Loading a file that was created with an outdated version of EPyT-Flow" +
+                          " -- support of such old files will be removed in the next release!",
+                          DeprecationWarning)
 
         for node_id, node_info in nodes:
             node_elevation = node_info["elevation"]
             node_type = node_info["type"]
             self.add_node(node_id, info={"elevation": node_elevation, "type": node_type})
 
         for link_id, link, link_info in links:
@@ -100,31 +121,51 @@
         """
         for link_id_, link_nodes, link_info in self.__links:
             if link_id_ == link_id:
                 return {"nodes": link_nodes} | link_info
 
         raise ValueError(f"Unknown link '{link_id}'")
 
+    @property
+    def units(self) -> int:
+        """
+        Gets the used measurement units category.
+
+        Will be one of the following constants:
+
+            - UNITS_USCUSTOM = 0  (US Customary)
+            - UNITS_SIMETRIC = 1  (SI Metric)
+
+        Returns
+        -------
+        `int`
+            Measurement units category.
+        """
+        return self.__units
+
     def __eq__(self, other) -> bool:
         if not isinstance(other, NetworkTopology):
             raise TypeError("Can not compare 'NetworkTopology' instance to " +
                             f"'{type(other)}' instance")
 
         return super().__eq__(other) and \
-            self.get_all_nodes() == other.get_all_nodes() and \
-            all(link_a[0] == link_b[0] and all(link_a[1] == link_b[1])
-                for link_a, link_b in zip(self.get_all_links(), other.get_all_links()))
+            self.get_all_nodes() == other.get_all_nodes() \
+            and all(link_a[0] == link_b[0] and all(link_a[1] == link_b[1])
+                    for link_a, link_b in zip(self.get_all_links(), other.get_all_links())) \
+            and self.__units == other.units
 
     def __str__(self) -> str:
-        return f"f_inp: {self.name} nodes: {self.__nodes} links: {self.__links}"
+        return f"f_inp: {self.name} nodes: {self.__nodes} links: {self.__links} " +\
+            f"units: {self.__units}"
 
     def get_attributes(self) -> dict:
         return super().get_attributes() | {"f_inp": self.name,
                                            "nodes": self.__nodes,
-                                           "links": self.__links}
+                                           "links": self.__links,
+                                           "units": self.__units}
 
     def get_adj_matrix(self) -> bsr_array:
         """
         Gets the adjacency matrix of this graph.
 
         Returns
         -------
```

### Comparing `epyt_flow-0.1.1/epyt_flow/uncertainty/model_uncertainty.py` & `epyt_flow-0.2.0/epyt_flow/uncertainty/model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/uncertainty/sensor_noise.py` & `epyt_flow-0.2.0/epyt_flow/uncertainty/sensor_noise.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/uncertainty/uncertainties.py` & `epyt_flow-0.2.0/epyt_flow/uncertainty/uncertainties.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/uncertainty/utils.py` & `epyt_flow-0.2.0/epyt_flow/uncertainty/utils.py`

 * *Files identical despite different names*

### Comparing `epyt_flow-0.1.1/epyt_flow/utils.py` & `epyt_flow-0.2.0/epyt_flow/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import math
 import tempfile
 import zipfile
 from pathlib import Path
 import requests
 from tqdm import tqdm
 import numpy as np
+import matplotlib
 import matplotlib.pyplot as plt
 
 
 def time_points_to_one_hot_encoding(time_points: list[int], total_length: int) -> list[int]:
     """
     Converts a list of time points into a one-hot-encoding.
 
@@ -63,15 +64,16 @@
     if tank_diameter <= 0:
         raise ValueError("'tank_diameter' must be greater than zero")
 
     return (4. / (math.pow(tank_diameter, 2) * math.pi)) * tank_volume
 
 
 def plot_timeseries_data(data: np.ndarray, labels: list[str] = None, x_axis_label: str = None,
-                         y_axis_label: str = None, show: bool = True) -> None:
+                         y_axis_label: str = None, show: bool = True,
+                         ax: matplotlib.axes.Axes = None) -> matplotlib.axes.Axes:
     """
     Plots a single or multiple time series.
 
     Parameters
     ----------
     data : `numpy.ndarray`
         Time series data -- each row in `data` corresponds to a complete time series.
@@ -87,15 +89,26 @@
     y_axis_label : `str`, optional
         Y axis label.
 
         The default is None.
     show : `bool`, optional
         If True, the plot/figure is shown in a window.
 
+        Only considered when 'ax' is None.
+
         The default is True.
+    ax : `matplotlib.axes.Axes`, optional
+        If not None, 'ax' is used for plotting.
+
+        The default is None.
+
+    Returns
+    -------
+    `matplotlib.axes.Axes`
+        Plot.
     """
     if not isinstance(data, np.ndarray):
         raise TypeError(f"'data' must be an instance of 'numpy.ndarray' but not of '{type(data)}'")
     if len(data.shape) != 2:
         raise ValueError("'data' must be a 2d array where each row corresponds to a time series " +
                          "-- use '.reshape(1, -1)' in case of single time series")
     if labels is not None:
@@ -107,36 +120,45 @@
                             f"but not of '{type(x_axis_label)}'")
     if y_axis_label is not None:
         if not isinstance(y_axis_label, str):
             raise TypeError("'y_axis_label' must be an instance of 'str' " +
                             f"but not of '{type(y_axis_label)}'")
     if not isinstance(show, bool):
         raise TypeError(f"'show' must be an instance of 'bool' but not of '{type(show)}'")
-
-    plt.figure()
+    if ax is not None:
+        if not isinstance(ax, matplotlib.axes.Axes):
+            raise TypeError("ax' must be an instance of 'matplotlib.axes.Axes'" +
+                            f"but not of '{type(ax)}'")
+
+    fig = None
+    if ax is None:
+        fig, ax = plt.subplots()
 
     labels = labels if labels is not None else [None] * data.shape[0]
 
     for i in range(data.shape[0]):
-        plt.plot(data[i, :], ".-", label=labels[i])
+        ax.plot(data[i, :], ".-", label=labels[i])
 
     if not any(label is None for label in labels):
-        plt.legend()
+        ax.legend()
 
     if x_axis_label is not None:
-        plt.xlabel(x_axis_label)
+        ax.set_xlabel(x_axis_label)
     if y_axis_label is not None:
-        plt.ylabel(y_axis_label)
+        ax.set_ylabel(y_axis_label)
 
-    if show is True:
+    if show is True and fig is not None:
         plt.show()
 
+    return ax
+
 
 def plot_timeseries_prediction(y: np.ndarray, y_pred: np.ndarray,
-                               confidence_interval: np.ndarray = None, show: bool = True) -> None:
+                               confidence_interval: np.ndarray = None, show: bool = True,
+                               ax: matplotlib.axes.Axes = None) -> matplotlib.axes.Axes:
     """
     Plots the prediction (e.g. forecast) of *single* time series together with the
     ground truth time series. In addition, confidence intervals can be plotted as well.
 
     Parameters
     ----------
     y : `numpy.ndarray`
@@ -147,15 +169,26 @@
         Confidence interval (upper and lower value) for each prediction in `y_pred`.
         If not None, the confidence interval is plotted as well.
 
         The default is None.
     show : `bool`, optional
         If True, the plot/figure is shown in a window.
 
+        Only considered when 'ax' is None.
+
         The default is True.
+    ax : `matplotlib.axes.Axes`, optional
+        If not None, 'axes' is used for plotting.
+
+        The default is None.
+
+    Returns
+    -------
+    `matplotlib.axes.Axes`
+        Plot.
     """
     if not isinstance(y_pred, np.ndarray):
         raise TypeError("'y_pred' must be an instance of 'numpy.ndarray' " +
                         f"but not of '{type(y_pred)}'")
     if not isinstance(y, np.ndarray):
         raise TypeError("'y' must be an instance of 'numpy.ndarray' " +
                         f"but not of '{type(y)}'")
@@ -163,29 +196,37 @@
         raise ValueError(f"Shape mismatch: {y_pred.shape} vs. {y.shape}")
     if len(y_pred.shape) != 1:
         raise ValueError("'y_pred' must be a 1d array")
     if len(y.shape) != 1:
         raise ValueError("'y' must be a 1d array")
     if not isinstance(show, bool):
         raise TypeError(f"'show' must be an instance of 'bool' but not of '{type(show)}'")
-
-    plt.figure()
+    if ax is not None:
+        if not isinstance(ax, matplotlib.axes.Axes):
+            raise TypeError("ax' must be an instance of 'matplotlib.axes.Axes'" +
+                            f"but not of '{type(ax)}'")
+
+    fig = None
+    if ax is None:
+        fig, ax = plt.subplots()
 
     if confidence_interval is not None:
-        plt.fill_between(range(len(y_pred)),
-                         y_pred - confidence_interval[0],
-                         y_pred + confidence_interval[1],
-                         alpha=0.5)
-    plt.plot(y_pred, ".-", label="Prediction")
-    plt.plot(y, ".-", label="Ground truth")
-    plt.legend()
+        ax.fill_between(range(len(y_pred)),
+                        y_pred - confidence_interval[0],
+                        y_pred + confidence_interval[1],
+                        alpha=0.5)
+    ax.plot(y_pred, ".-", label="Prediction")
+    ax.plot(y, ".-", label="Ground truth")
+    ax.legend()
 
-    if show is True:
+    if show is True and fig is not None:
         plt.show()
 
+    return ax
+
 
 def download_if_necessary(download_path: str, url: str, verbose: bool = True) -> None:
     """
     Downloads a file from a given URL if it does not already exist in a given path.
 
     Note that if the path (folder) does not already exist, it will be created.
 
@@ -230,14 +271,30 @@
     ----------
     path_in : `str`
         Path to be created.
     """
     Path(path_in).mkdir(parents=True, exist_ok=True)
 
 
+def pack_zip_archive(f_in: list[str], f_out: str) -> None:
+    """
+    Compresses a given list of files into a .zip archive.
+
+    Parameters
+    ----------
+    f_in : `list[str]`
+        List of files to be compressed into the .zip archive.
+    f_out : `str`
+        Path to the final .zip file.
+    """
+    with zipfile.ZipFile(f_out, "w") as f_zip_out:
+        for f_cur_in in f_in:
+            f_zip_out.write(f_cur_in, compress_type=zipfile.ZIP_DEFLATED)
+
+
 def unpack_zip_archive(f_in: str, folder_out: str) -> None:
     """
     Unpacks a .zip archive.
 
     Parameters
     ----------
     f_in : `str`
```

### Comparing `epyt_flow-0.1.1/epyt_flow.egg-info/PKG-INFO` & `epyt_flow-0.2.0/epyt_flow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyt-flow
-Version: 0.1.1
+Version: 0.2.0
 Summary: EPyT-Flow -- EPANET Python Toolkit - Flow
 Author-email: André Artelt <aartelt@techfak.uni-bielefeld.de>, "Marios S. Kyriakou" <kiriakou.marios@ucy.ac.cy>, "Stelios G. Vrachimis" <vrachimis.stelios@ucy.ac.cy>
 License: MIT License
 Project-URL: Homepage, https://github.com/WaterFutures/EPyT-Flow
 Project-URL: Documentation, https://epyt-flow.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/WaterFutures/EPyT-Flow.git
 Project-URL: Issues, https://github.com/WaterFutures/EPyT-Flow/issues
@@ -48,14 +48,31 @@
 and [EPANET-MSX](https://github.com/USEPA/EPANETMSX/).
 
 EPyT-Flow provides easy access to popular benchmark data sets for event detection and localization.
 Furthermore, it also provides an environment for developing and testing control algorithms.
 
 ![](https://github.com/WaterFutures/EPyT-Flow/blob/main/docs/_static/net1_plot.png?raw=true)
 
+
+## Unique Features
+
+Unique features of EPyT-Flow that make it superior to other (Python) toolboxes are the following:
+
+- High-performance hydraulic and (advanced) water quality simulation
+- High- and low-level interface
+- Object-orientated design that is easy to extend and customize
+- Sensor configurations
+- Wide variety of pre-defined events (e.g. leakages, sensor faults, actuator events, cyber-attacks, etc.)
+- Wide variety of pre-defined types of uncertainties (e.g. model uncertainties)
+- Step-wise simulation and environment for training and evaluating control strategies
+- Serialization module for easy exchange of data and (scenario) configurations
+- REST API to make EPyT-Flow accessible in other applications
+- Access to many WDNs and popular benchmarks (incl. their evaluation)
+
+
 ## Installation
 
 EPyT-Flow supports Python 3.9 - 3.12
 
 Note that [EPANET and EPANET-MSX sources](epyt_flow/EPANET/) are compiled and overwrite the binaries
 shipped by EPyT IF EPyT-Flow is installed on a Linux system. By this we not only aim to achieve
 a better performance of the simulations but also avoid any compatibility problems of pre-compiled binaries.
```

### Comparing `epyt_flow-0.1.1/epyt_flow.egg-info/SOURCES.txt` & `epyt_flow-0.2.0/epyt_flow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 epyt_flow/topology.py
 epyt_flow/utils.py
 epyt_flow.egg-info/PKG-INFO
 epyt_flow.egg-info/SOURCES.txt
 epyt_flow.egg-info/dependency_links.txt
 epyt_flow.egg-info/requires.txt
 epyt_flow.egg-info/top_level.txt
-epyt_flow/EPANET/compile.sh
+epyt_flow/EPANET/compile_linux.sh
 epyt_flow/EPANET/EPANET-MSX/MSX_Updates.txt
 epyt_flow/EPANET/EPANET-MSX/readme.txt
 epyt_flow/EPANET/EPANET-MSX/Src/dispersion.h
 epyt_flow/EPANET/EPANET-MSX/Src/hash.c
 epyt_flow/EPANET/EPANET-MSX/Src/hash.h
 epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.c
 epyt_flow/EPANET/EPANET-MSX/Src/mathexpr.h
@@ -106,17 +106,24 @@
 epyt_flow/gym/scenario_control_env.py
 epyt_flow/models/__init__.py
 epyt_flow/models/event_detector.py
 epyt_flow/models/sensor_interpolation_detector.py
 epyt_flow/rest_api/__init__.py
 epyt_flow/rest_api/base_handler.py
 epyt_flow/rest_api/res_manager.py
-epyt_flow/rest_api/scada_data_handler.py
-epyt_flow/rest_api/scenario_handler.py
 epyt_flow/rest_api/server.py
+epyt_flow/rest_api/scada_data/__init__.py
+epyt_flow/rest_api/scada_data/data_handlers.py
+epyt_flow/rest_api/scada_data/export_handlers.py
+epyt_flow/rest_api/scada_data/handlers.py
+epyt_flow/rest_api/scenario/__init__.py
+epyt_flow/rest_api/scenario/event_handlers.py
+epyt_flow/rest_api/scenario/handlers.py
+epyt_flow/rest_api/scenario/simulation_handlers.py
+epyt_flow/rest_api/scenario/uncertainty_handlers.py
 epyt_flow/simulation/__init__.py
 epyt_flow/simulation/parallel_simulation.py
 epyt_flow/simulation/scenario_config.py
 epyt_flow/simulation/scenario_simulator.py
 epyt_flow/simulation/scenario_visualizer.py
 epyt_flow/simulation/sensor_config.py
 epyt_flow/simulation/events/__init__.py
```

### Comparing `epyt_flow-0.1.1/pyproject.toml` & `epyt_flow-0.2.0/pyproject.toml`

 * *Files identical despite different names*

