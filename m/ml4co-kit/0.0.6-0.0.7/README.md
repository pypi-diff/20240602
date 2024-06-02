# Comparing `tmp/ml4co_kit-0.0.6.tar.gz` & `tmp/ml4co_kit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4co_kit-0.0.6.tar", last modified: Sun Jun  2 14:56:17 2024, max compression
+gzip compressed data, was "ml4co_kit-0.0.7.tar", last modified: Sun Jun  2 17:41:01 2024, max compression
```

## Comparing `ml4co_kit-0.0.6.tar` & `ml4co_kit-0.0.7.tar`

### file list

```diff
@@ -1,788 +1,808 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.794100 ml4co_kit-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.810100 ml4co_kit-0.0.6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    21840 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/cvrp_problem.png
--rw-r--r--   0 runner    (1001) docker     (127)    47630 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/cvrp_solution.png
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/kroA150_problem.png
--rw-r--r--   0 runner    (1001) docker     (127)    34941 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/kroA150_solution.png
--rw-r--r--   0 runner    (1001) docker     (127)    87460 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/mis_problem.png
--rw-r--r--   0 runner    (1001) docker     (127)    87798 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/mis_solution.png
--rw-r--r--   0 runner    (1001) docker     (127)   180376 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/ml4co-kit-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   171559 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/assets/organization.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/docs/project_example/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/project_example/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/project_example/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/project_example/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/project_example/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/docs/project_example/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/ml4co_kit/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/ml4co_kit/data/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/ml4co_kit/data/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/mis/satlib_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/ml4co_kit/data/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/tsp/ml4tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsp_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsplib4ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsplib_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.814100 ml4co_kit-0.0.6/ml4co_kit/data/vrp/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/vrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/data/vrp/vrplib_original.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/draw/
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/draw/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/draw/mis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/draw/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/draw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/evaluate/cvrp/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/cvrp/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/evaluate/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/mis/satlib_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/tsplib4ml_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/tsplib_original_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/uniform_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/generator/cvrp_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/generator/mis_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/generator/tsp_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/learning/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/learning/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/learning/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/learning/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/learning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.818100 ml4co_kit-0.0.6/ml4co_kit/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.822100 ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26696 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/lkh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/pyvrp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.822100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/gurobi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.822100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101393 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.822100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/graphchecker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/online_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/parse_parameters_omis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/reduction_evomis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/sort_adjacencies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/compile_withcmake.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.798100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.794100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.822100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/configuration.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.826100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.826100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.826100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.826100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.826100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.830100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.834100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.834100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.834100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.834100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.838100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.842100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.846100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.846100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.846100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.846100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.850100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.854100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.854100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.858100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.858100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.862100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.862100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.866100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.866100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.866100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.866100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.866100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.870100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.870100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.870100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/
--rw-r--r--   0 runner    (1001) docker     (127)    70067 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.802100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.874100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)    36218 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67592 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/sort_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/cpp.vim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/branch_reduce.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/weighted_ls.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.806100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.878100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.882100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.882100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.882100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.882100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.882100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.886100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.886100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.886100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.890100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.894100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.894100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.894100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.894100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.898100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.898100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.898100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.898100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.902100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    25053 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.902100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.902100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.902100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.906100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.906100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.906100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.906100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.906100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.910100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.910100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.910100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h
--rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.910100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.910100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.914101 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.918100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.918100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.922100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.806100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.922100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.922100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.922100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.926100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.926100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.926100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.926100 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.h
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.926100 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/concorde.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.930101 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.930101 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.930101 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/_concorde.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.942101 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/
--rw-r--r--   0 runner    (1001) docker     (127)  7630518 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/concorde.a
--rw-r--r--   0 runner    (1001) docker     (127)   248168 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/concorde.h
--rw-r--r--   0 runner    (1001) docker     (127)   854866 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.a
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.h
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/ml4co_kit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/utils/mis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/utils/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/ml4co_kit/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/ml4co_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-06-02 14:56:17.000000 ml4co_kit-0.0.6/ml4co_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    56294 2024-06-02 14:56:17.000000 ml4co_kit-0.0.6/ml4co_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 14:56:17.000000 ml4co_kit-0.0.6/ml4co_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-02 14:56:17.000000 ml4co_kit-0.0.6/ml4co_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 14:56:17.000000 ml4co_kit-0.0.6/ml4co_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 14:56:17.946101 ml4co_kit-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-06-02 14:56:12.000000 ml4co_kit-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.944535 ml4co_kit-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-06-02 17:41:01.940535 ml4co_kit-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8998 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.724535 ml4co_kit-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.748535 ml4co_kit-0.0.7/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    21840 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/cvrp_problem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47630 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/cvrp_solution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/kroA150_problem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34941 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/kroA150_solution.png
+-rw-r--r--   0 runner    (1001) docker     (127)    87460 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/mis_problem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    87798 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/mis_solution.png
+-rw-r--r--   0 runner    (1001) docker     (127)   180376 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/ml4co-kit-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171559 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/assets/organization.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.748535 ml4co_kit-0.0.7/docs/project_example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/project_example/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/project_example/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/project_example/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/project_example/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/docs/project_example/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.748535 ml4co_kit-0.0.7/ml4co_kit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.748535 ml4co_kit-0.0.7/ml4co_kit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.748535 ml4co_kit-0.0.7/ml4co_kit/data/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/mis/satlib_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/data/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/tsp/ml4tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsp_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsplib4ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsplib_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/data/vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/vrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/data/vrp/vrplib_original.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/draw/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/draw/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/draw/mis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/draw/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/draw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/evaluate/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/cvrp/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.752535 ml4co_kit-0.0.7/ml4co_kit/evaluate/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/mis/satlib_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.756535 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/tsplib4ml_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/tsplib_original_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/uniform_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.756535 ml4co_kit-0.0.7/ml4co_kit/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/generator/cvrp_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/generator/mis_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14294 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/generator/tsp_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.756535 ml4co_kit-0.0.7/ml4co_kit/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/learning/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/learning/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/learning/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/learning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.756535 ml4co_kit-0.0.7/ml4co_kit/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.756535 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26759 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.760535 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/CircleSector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Genetic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Genetic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Individual.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Individual.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29102 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/LocalSearch.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/LocalSearch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Params.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Params.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Population.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Population.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Split.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/Split.h
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/commandline.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)   119560 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/cvrp_hgs_solver
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/c_hgs/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/hgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/lkh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/pyvrp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.760535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/gurobi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.764535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101393 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.764535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/configuration_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/graphchecker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/online_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/parse_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/parse_parameters_omis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/reduction_evomis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/sort_adjacencies.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/compile_withcmake.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.732535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.728535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.764535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/configuration.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.764535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.764535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.768535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.768535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.768535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.768535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.768535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.772535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.776535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.776535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.776535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.776535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.784535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.784535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.784535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.784535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.788535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.788535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.788535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.792535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.792535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.792535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.792535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.792535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.800535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.800535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.804535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.804535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.808535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.816535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.816535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.820535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c
+-rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.824535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.824535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.824535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.824535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.828535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.828535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.828535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/
+-rw-r--r--   0 runner    (1001) docker     (127)    70067 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.736535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.832535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.836535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.836535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36218 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.836535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67592 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/mis_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.836535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/sort_metis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/cpp.vim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/branch_reduce.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/configuration_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/parse_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/weighted_ls.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.740535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.840535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.844535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.844535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.844535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.844535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.844535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.848535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.848535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.852535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.856535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.856535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.856535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.856535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.860535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.860535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.860535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.860535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25053 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.864535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.864535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.864535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.868535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.868535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.868535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.868535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.868535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.872535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.872535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.872535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.872535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.872535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.876535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.880535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.888535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.888535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c
+-rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.744535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.896535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.896535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.896535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.896535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.896535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.904535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/mis_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.904535 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.904535 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/concorde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.908535 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.908535 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.908535 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/_concorde.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.940535 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  7630518 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/concorde.a
+-rw-r--r--   0 runner    (1001) docker     (127)   248168 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/concorde.h
+-rw-r--r--   0 runner    (1001) docker     (127)   854866 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.a
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.940535 ml4co_kit-0.0.7/ml4co_kit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/utils/mis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/utils/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/ml4co_kit/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.940535 ml4co_kit-0.0.7/ml4co_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-06-02 17:41:01.000000 ml4co_kit-0.0.7/ml4co_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    57048 2024-06-02 17:41:01.000000 ml4co_kit-0.0.7/ml4co_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 17:41:01.000000 ml4co_kit-0.0.7/ml4co_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-02 17:41:01.000000 ml4co_kit-0.0.7/ml4co_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 17:41:01.000000 ml4co_kit-0.0.7/ml4co_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 17:41:01.944535 ml4co_kit-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 17:41:01.940535 ml4co_kit-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-06-02 17:40:55.000000 ml4co_kit-0.0.7/tests/test_utils.py
```

### Comparing `ml4co_kit-0.0.6/PKG-INFO` & `ml4co_kit-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4co-kit
-Version: 0.0.6
+Version: 0.0.7
 Summary: ml4co-kit provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/Thinklab-SJTU/ML4CO-Kit
 Author: SJTU-ReThinkLab
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -34,36 +34,36 @@
 Requires-Dist: cython>=3.0.8
 
 
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
 [![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/ml4co_kit/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fml4co_kit%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
 
-`ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
+`ML4CO-Kit` is an in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
 This repository focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
 
 | Problem |                Data                |    solver     |      Supervision      | evaluator |      visualization      |
 | :-----: | :--------------------------------: | :-----------: | :-------------------: | :-------: | :---------------------: |
 |   TSP   | Uniform, Gaussian, Cluster, TSPLIB | LKH, Concorde | Solution, Edge Regret |     ✔     | Problem Graph, Solution |
 |   MIS   |       SATLIB, ER, BA, HK, WS       | KaMIS, Gurobi |       Solution        |     ✔     | Problem Graph, Solution |
-|  CVRP   |    Uniform, Gaussian, VRPLIB       | LKH, PyVRP    |       Solution        |     ✔     | Problem Graph, Solution |
+|  CVRP   |    Uniform, Gaussian, VRPLIB       | PyVRP, LKH, HGS |       Solution        |     ✔     | Problem Graph, Solution |
 
 ###### ML4CO Organization:
 
 <img src="docs/assets/organization.jpg" alt="Organization" width="800"/>
 
-We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies coming soon.
+We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies is coming soon.
 
 ## Installation
 
 You can install the stable release on PyPI:
 
 ```bash
 $ pip install ml4co_kit
@@ -71,15 +71,15 @@
 
 or get the latest version by running:
 
 ```bash
 $ pip install -U https://github.com/Thinklab-SJTU/ML4CO-Kit/archive/master.zip # with --user for user install (no root)
 ```
 
-The following packages are required, and shall be automatically installed by ``pip``:
+The following packages are required and shall be automatically installed by ``pip``:
 
 ```
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 tsplib95==0.7.1
 tqdm>=4.66.1
@@ -99,15 +99,15 @@
 pytorch_lightning
 ```
 
 ## Usage Examples
 
 ### Solve with Traditional Solver Baselines
 
-We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
+We provide base classes with a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, it includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
 >>> tsp_lkh_solver = TSPLKHSolver(lkh_max_trials=500)
```

### Comparing `ml4co_kit-0.0.6/README.md` & `ml4co_kit-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
 [![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/ml4co_kit/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fml4co_kit%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
 
-`ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
+`ML4CO-Kit` is an in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
 This repository focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
 
 | Problem |                Data                |    solver     |      Supervision      | evaluator |      visualization      |
 | :-----: | :--------------------------------: | :-----------: | :-------------------: | :-------: | :---------------------: |
 |   TSP   | Uniform, Gaussian, Cluster, TSPLIB | LKH, Concorde | Solution, Edge Regret |     ✔     | Problem Graph, Solution |
 |   MIS   |       SATLIB, ER, BA, HK, WS       | KaMIS, Gurobi |       Solution        |     ✔     | Problem Graph, Solution |
-|  CVRP   |    Uniform, Gaussian, VRPLIB       | LKH, PyVRP    |       Solution        |     ✔     | Problem Graph, Solution |
+|  CVRP   |    Uniform, Gaussian, VRPLIB       | PyVRP, LKH, HGS |       Solution        |     ✔     | Problem Graph, Solution |
 
 ###### ML4CO Organization:
 
 <img src="docs/assets/organization.jpg" alt="Organization" width="800"/>
 
-We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies coming soon.
+We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies is coming soon.
 
 ## Installation
 
 You can install the stable release on PyPI:
 
 ```bash
 $ pip install ml4co_kit
@@ -35,15 +35,15 @@
 
 or get the latest version by running:
 
 ```bash
 $ pip install -U https://github.com/Thinklab-SJTU/ML4CO-Kit/archive/master.zip # with --user for user install (no root)
 ```
 
-The following packages are required, and shall be automatically installed by ``pip``:
+The following packages are required and shall be automatically installed by ``pip``:
 
 ```
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 tsplib95==0.7.1
 tqdm>=4.66.1
@@ -63,15 +63,15 @@
 pytorch_lightning
 ```
 
 ## Usage Examples
 
 ### Solve with Traditional Solver Baselines
 
-We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
+We provide base classes with a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, it includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
 >>> tsp_lkh_solver = TSPLKHSolver(lkh_max_trials=500)
```

### Comparing `ml4co_kit-0.0.6/docs/assets/cvrp_problem.png` & `ml4co_kit-0.0.7/docs/assets/cvrp_problem.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/cvrp_solution.png` & `ml4co_kit-0.0.7/docs/assets/cvrp_solution.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/kroA150_problem.png` & `ml4co_kit-0.0.7/docs/assets/kroA150_problem.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/kroA150_solution.png` & `ml4co_kit-0.0.7/docs/assets/kroA150_solution.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/mis_problem.png` & `ml4co_kit-0.0.7/docs/assets/mis_problem.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/mis_solution.png` & `ml4co_kit-0.0.7/docs/assets/mis_solution.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/ml4co-kit-logo.png` & `ml4co_kit-0.0.7/docs/assets/ml4co-kit-logo.png`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/assets/organization.jpg` & `ml4co_kit-0.0.7/docs/assets/organization.jpg`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/project_example/data.py` & `ml4co_kit-0.0.7/docs/project_example/data.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/project_example/env.py` & `ml4co_kit-0.0.7/docs/project_example/env.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/project_example/model.py` & `ml4co_kit-0.0.7/docs/project_example/model.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/docs/project_example/solver.py` & `ml4co_kit-0.0.7/docs/project_example/solver.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/__init__.py` & `ml4co_kit-0.0.7/ml4co_kit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from .data import SATLIBOriDataset
 from .data import VRPLIBOriDataset
 from .evaluate import TSPEvaluator, TSPLIBOriEvaluator, TSPLIB4MLEvaluator, TSPUniformEvaluator
 from .evaluate import SATLIBEvaluator
 from .evaluate import CVRPEvaluator
 from .generator import TSPDataGenerator, MISDataGenerator, CVRPDataGenerator
 from .solver import TSPSolver, TSPLKHSolver, TSPConcordeSolver
-from .solver import MISSolver, KaMISSolver, MISGurobi
-from .solver import CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver
+from .solver import MISSolver, KaMISSolver, MISGurobiSolver
+from .solver import CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver, CVRPHGSSolver
 from .utils import download, compress_folder, extract_archive, _get_md5, iterative_execution
 
 # expand - matplotlib
 found_matplotlib = importlib.util.find_spec("matplotlib")
 if found_matplotlib is not None:
     from .draw.tsp import draw_tsp_problem, draw_tsp_solution
     from .draw.mis import draw_mis_problem, draw_mis_solution
@@ -27,9 +27,9 @@
     from .learning.model import BaseModel
     from .learning.train import Checkpoint, Logger, Trainer
     from .learning.utils import to_numpy, to_tensor
     from .learning.utils import check_dim
     from .learning.utils import points_to_distmat, sparse_points
 
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 __author__ = "SJTU-ReThinkLab"
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/mis/satlib_original.py` & `ml4co_kit-0.0.7/ml4co_kit/data/mis/satlib_original.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/tsp/ml4tsp.py` & `ml4co_kit-0.0.7/ml4co_kit/data/tsp/ml4tsp.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsp_uniform.py` & `ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsp_uniform.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsplib4ml.py` & `ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsplib4ml.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/tsp/tsplib_original.py` & `ml4co_kit-0.0.7/ml4co_kit/data/tsp/tsplib_original.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/data/vrp/vrplib_original.py` & `ml4co_kit-0.0.7/ml4co_kit/data/vrp/vrplib_original.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/draw/cvrp.py` & `ml4co_kit-0.0.7/ml4co_kit/draw/cvrp.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/draw/mis.py` & `ml4co_kit-0.0.7/ml4co_kit/draw/mis.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/draw/tsp.py` & `ml4co_kit-0.0.7/ml4co_kit/draw/tsp.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/draw/utils.py` & `ml4co_kit-0.0.7/ml4co_kit/draw/utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/cvrp/base.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/cvrp/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/mis/satlib_eval.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/mis/satlib_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/base.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/tsplib4ml_eval.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/tsplib4ml_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/tsplib_original_eval.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/tsplib_original_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/evaluate/tsp/uniform_eval.py` & `ml4co_kit-0.0.7/ml4co_kit/evaluate/tsp/uniform_eval.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/generator/cvrp_data.py` & `ml4co_kit-0.0.7/ml4co_kit/generator/cvrp_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import time
 import numpy as np
 import pathlib
 from tqdm import tqdm
 from typing import Union
 from multiprocessing import Pool
-from ml4co_kit.solver.cvrp import CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver
+from ml4co_kit.solver.cvrp import (
+    CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver, CVRPHGSSolver
+)
 
 
 class CVRPDataGenerator:
     def __init__(
         self,
         num_threads: int = 1,
         nodes_num: int = 50,
@@ -108,15 +110,16 @@
 
     def check_solver(self):
         # get solver
         if type(self.solver) == str:
             self.solver_type = self.solver
             supported_solver_dict = {
                 "pyvrp": CVRPPyVRPSolver,
-                "lkh": CVRPLKHSolver
+                "lkh": CVRPLKHSolver,
+                "hgs": CVRPHGSSolver
             }
             supported_solver_type = supported_solver_dict.keys()
             if self.solver_type not in supported_solver_type:
                 message = (
                     f"The input solver_type ({self.solver_type}) is not a valid type, "
                     f"and the generator only supports {supported_solver_type}."
                 )
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/generator/mis_data.py` & `ml4co_kit-0.0.7/ml4co_kit/generator/mis_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pickle
 import pathlib
 import random
 import networkx as nx
 import numpy as np
 from tqdm import tqdm
 from typing import Union
-from ml4co_kit.solver.mis import KaMISSolver, MISGurobi
-from ml4co_kit.solver import MISSolver, KaMISSolver, MISGurobi
+from ml4co_kit.solver.mis import KaMISSolver, MISGurobiSolver
+from ml4co_kit.solver import MISSolver, KaMISSolver, MISGurobiSolver
 
 
 class MISDataGenerator:
     def __init__(
         self,
         nodes_num_min: int = 700,
         nodes_num_max: int = 800,
@@ -131,15 +131,15 @@
                 f"mis_{self.data_type}_{self.nodes_num_min}_{self.nodes_num_max}"
             )
 
     def check_solver(self):
         # check solver
         if type(self.solver) == str:
             self.solver_type = self.solver
-            supported_solver_dict = {"kamis": KaMISSolver, "gurobi": MISGurobi}
+            supported_solver_dict = {"kamis": KaMISSolver, "gurobi": MISGurobiSolver}
             supported_solver_type = supported_solver_dict.keys()
             if self.solver not in supported_solver_type:
                 message = (
                     f"The input solver type ({self.solver}) is not a valid type, "
                     f"and the generator only supports {supported_solver_type}."
                 )
                 raise ValueError(message)
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/generator/tsp_data.py` & `ml4co_kit-0.0.7/ml4co_kit/generator/tsp_data.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/learning/env.py` & `ml4co_kit-0.0.7/ml4co_kit/learning/env.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/learning/model.py` & `ml4co_kit-0.0.7/ml4co_kit/learning/model.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/learning/train.py` & `ml4co_kit-0.0.7/ml4co_kit/learning/train.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/learning/utils.py` & `ml4co_kit-0.0.7/ml4co_kit/learning/utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/base.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 class CVRPSolver:
     def __init__(
         self, 
         solver_type: str = None, 
         depots_scale: int = 1e6,
         points_scale: int = 1e6,
-        demands_scale: int = 1e6,
-        capacities_scale: int = 1e6,
+        demands_scale: int = 1e3,
+        capacities_scale: int = 1e3,
     ):
         self.solver_type = solver_type
         self.depots_scale = depots_scale
         self.points_scale = points_scale
         self.demands_scale = demands_scale
         self.capacities_scale = capacities_scale
         self.depots = None
@@ -570,14 +570,15 @@
             os.makedirs(save_dir)
 
         # write
         for idx in range(points.shape[0]):
             save_path = os.path.join(save_dir, filename + f"-{idx}.vrp")
             with open(save_path, "w") as f:
                 f.write(f"NAME : {save_path}\n")
+                f.write(f"COMMENT : Generated by ML4CO-Kit\n")
                 f.write("TYPE : CVRP\n")
                 f.write(f"DIMENSION : {self.nodes_num + 1}\n")
                 f.write(f"EDGE_WEIGHT_TYPE : {self.norm}\n")
                 f.write(f"CAPACITY : {self.capacities[idx]}\n")
                 f.write("NODE_COORD_SECTION\n")
                 x, y = depots[idx]
                 f.write(f"1 {x} {y}\n")
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/lkh.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/lkh.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 class CVRPLKHSolver(CVRPSolver):
     def __init__(
         self,
         depots_scale: int = 1e6,
         points_scale: int = 1e6,
-        demands_scale: int = 1e6,
-        capacities_scale: int = 1e6,
+        demands_scale: int = 1e3,
+        capacities_scale: int = 1e3,
         lkh_max_trials: int = 1000,
         lkh_path: pathlib.Path = "LKH",
         lkh_runs: int = 10,
         lkh_seed: int = 1234,
     ):
         """
         TSPLKHSolver
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/cvrp/pyvrp.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/cvrp/pyvrp.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 class CVRPPyVRPSolver(CVRPSolver):
     def __init__(
         self,
         depots_scale: int = 1e6,
         points_scale: int = 1e6,
-        demands_scale: int = 1e6,
-        capacities_scale: int = 1e6,
+        demands_scale: int = 1e3,
+        capacities_scale: int = 1e3,
         time_limit: float = 1.0,
     ):
         super(CVRPPyVRPSolver, self).__init__(
             solver_type="pyvrp", 
             depots_scale = depots_scale,
             points_scale = points_scale,
             demands_scale = demands_scale,
@@ -62,19 +62,19 @@
         for frm in locations:
             for to in locations:
                 distance = self.get_distance(x1=(frm.x, frm.y), x2=(to.x, to.y))
                 cvrp_model.add_edge(frm, to, distance=self.round_func(distance))
         res = cvrp_model.solve(stop=MaxRuntime(self.time_limit))
         
         routes = res.best.get_routes() if CP38 else res.best.routes()
-        tours = [0]
+        tour = [0]
         for route in routes:
-            tours += route.visits()
-            tours.append(0)
-        return tours
+            tour += route.visits()
+            tour.append(0)
+        return tour
         
     def solve(
         self,
         depots: Union[list, np.ndarray] = None,
         points: Union[list, np.ndarray] = None,
         demands: Union[list, np.ndarray] = None,
         capacities: Union[list, np.ndarray] = None,
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/base.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/gurobi.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/gurobi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import networkx as nx
 import pandas as pd
 from pathlib import Path
 from ml4co_kit.solver.mis.base import MISSolver
 
 
-class MISGurobi(MISSolver):
+class MISGurobiSolver(MISSolver):
     def __init__(
         self,
         weighted: bool = False,
         time_limit: float = 60.0,
         num_threads: int = 8,
         quadratic: bool = False,
         write_mps: bool = False,
@@ -34,15 +34,15 @@
                 Maximum number of threads to use.
             quadratic (bool, optional):
                 Whether a quadratic program should be used instead of a linear program
                 to solve the MIS problem (cannot be used together with weighted).
             write_mps (bool, optional):
                 Instead of solving, write mps output (e.g., for tuning)
         """
-        super(MISGurobi, self).__init__()
+        super(MISGurobiSolver, self).__init__()
         self.solver_type = "gurobi"
         self.weighted = weighted
         self.time_limit = time_limit
         self.num_threads = num_threads
         self.quadratic = quadratic
         self.write_mps = write_mps
         self.gurobi_path = pathlib.Path(__file__).parent
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/Doxyfile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/Doxyfile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/configuration_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/graphchecker.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/graphchecker.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/online_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/online_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/parse_parameters.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/parse_parameters.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/parse_parameters_omis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/parse_parameters_omis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/reduction_evomis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/reduction_evomis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/app/sort_adjacencies.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/app/sort_adjacencies.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/compile_withcmake.sh` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/compile_withcmake.sh`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/configuration.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/app/configuration.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConscript` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConscript`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/array_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/array_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/operation_log.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/ils.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/local_search_online.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/ils/online_ils.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/fast_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/fast_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/kernel/modified.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/mis/mis_config.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/mis/mis_config.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/lib/tools/mis_log.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/conversion/sort_metis.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/conversion/sort_metis.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/misc/cpp.vim` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/misc/cpp.vim`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/branch_reduce.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/branch_reduce.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/configuration_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/parse_parameters.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/parse_parameters.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/app/weighted_ls.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/app/weighted_ls.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/mis_config.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/mis/mis_config.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis-source/wmis/lib/tools/mis_log.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/mis/kamis.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/mis/kamis.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/base.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/base.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/concorde.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/concorde.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/problems.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/problems.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/lkh_solver/solve.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/lkh_solver/solve.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/_concorde.pyx` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/_concorde.pyx`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/concorde/solve.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/concorde.a` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/concorde.a`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/concorde.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/concorde.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.a` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.a`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.h` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/data/qsopt.h`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/solver/tsp/pyconcorde/setup.py` & `ml4co_kit-0.0.7/ml4co_kit/solver/tsp/pyconcorde/setup.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/utils/file_utils.py` & `ml4co_kit-0.0.7/ml4co_kit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit/utils/mis_utils.py` & `ml4co_kit-0.0.7/ml4co_kit/utils/mis_utils.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/ml4co_kit.egg-info/PKG-INFO` & `ml4co_kit-0.0.7/ml4co_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4co-kit
-Version: 0.0.6
+Version: 0.0.7
 Summary: ml4co-kit provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/Thinklab-SJTU/ML4CO-Kit
 Author: SJTU-ReThinkLab
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -34,36 +34,36 @@
 Requires-Dist: cython>=3.0.8
 
 
 <img src="docs/assets/ml4co-kit-logo.png" alt="ML4CO-Kit" width="800"/>
 
 [![PyPi version](https://badgen.net/pypi/v/ml4co-kit/)](https://pypi.org/pypi/ml4co_kit/) [![PyPI pyversions](https://img.shields.io/badge/dynamic/json?color=blue&label=python&query=info.requires_python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fml4co_kit%2Fjson)](https://pypi.python.org/pypi/ml4co-kit/) [![Downloads](https://static.pepy.tech/badge/ml4co-kit)](https://pepy.tech/project/ml4co-kit) [![GitHub stars](https://img.shields.io/github/stars/Thinklab-SJTU/ML4CO-Kit.svg?style=social&label=Star&maxAge=8640)](https://GitHub.com/Thinklab-SJTU/ML4CO-Kit/stargazers/)
 
-`ML4CO-Kit` is a in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
+`ML4CO-Kit` is an in-development toolkit for machine learning practices on combinatorial optimization problems, which is a by-product of our research for a unified modular framework that integrates existing ML4CO practices, minimizing disparities among methods and supporting the investigations via in-depth analysis and transparent ablation. 
 
 This repository focuses on the supporting code for method development instead of implementing core technologies, which will be presented in the future in our full implementation and organization. `ML4CO-Kit` has the following features:
 
 * The skeleton of framework organization for ML4CO projects;
 * Implemented base classes that facilitate method development;
 * Mainstream traditional solver baselines and reference solution acquisition;
 * Data generation of various distributions;
 * Problem and solution visualization;
 * Evaluators for different problems.
 
 | Problem |                Data                |    solver     |      Supervision      | evaluator |      visualization      |
 | :-----: | :--------------------------------: | :-----------: | :-------------------: | :-------: | :---------------------: |
 |   TSP   | Uniform, Gaussian, Cluster, TSPLIB | LKH, Concorde | Solution, Edge Regret |     ✔     | Problem Graph, Solution |
 |   MIS   |       SATLIB, ER, BA, HK, WS       | KaMIS, Gurobi |       Solution        |     ✔     | Problem Graph, Solution |
-|  CVRP   |    Uniform, Gaussian, VRPLIB       | LKH, PyVRP    |       Solution        |     ✔     | Problem Graph, Solution |
+|  CVRP   |    Uniform, Gaussian, VRPLIB       | PyVRP, LKH, HGS |       Solution        |     ✔     | Problem Graph, Solution |
 
 ###### ML4CO Organization:
 
 <img src="docs/assets/organization.jpg" alt="Organization" width="800"/>
 
-We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies coming soon.
+We are still enriching the library and we welcome any contributions/ideas/suggestions from the community. A comprehensive modular framework built upon this library that integrates core ML4CO technologies is coming soon.
 
 ## Installation
 
 You can install the stable release on PyPI:
 
 ```bash
 $ pip install ml4co_kit
@@ -71,15 +71,15 @@
 
 or get the latest version by running:
 
 ```bash
 $ pip install -U https://github.com/Thinklab-SJTU/ML4CO-Kit/archive/master.zip # with --user for user install (no root)
 ```
 
-The following packages are required, and shall be automatically installed by ``pip``:
+The following packages are required and shall be automatically installed by ``pip``:
 
 ```
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 tsplib95==0.7.1
 tqdm>=4.66.1
@@ -99,15 +99,15 @@
 pytorch_lightning
 ```
 
 ## Usage Examples
 
 ### Solve with Traditional Solver Baselines
 
-We provide base classes that offer a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, which includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
+We provide base classes with a user-friendly approach for implementing traditional and learning-based solvers. Taking `TSPSolver` as an example, it includes functionalities for data input and output, as well as an evaluation function. The solver supports different data inputs, such as Numpy arrays and .txt and .tsp files. The outputs can be saved to corresponding types of files as needed. Additionally, the solver offers an evaluation function, by which users can quickly obtain the average tour length, average gap, and standard deviation of the test dataset. Traditional solvers are directly incorporated in our library inheriting `TSPSolver`.
 
 ```python
 >>> from ml4co_kit.solver import TSPLKHSolver
 
 # initialization
 >>> tsp_lkh_solver = TSPLKHSolver(lkh_max_trials=500)
```

### Comparing `ml4co_kit-0.0.6/ml4co_kit.egg-info/SOURCES.txt` & `ml4co_kit-0.0.7/ml4co_kit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,35 @@
 ml4co_kit/learning/env.py
 ml4co_kit/learning/model.py
 ml4co_kit/learning/train.py
 ml4co_kit/learning/utils.py
 ml4co_kit/solver/__init__.py
 ml4co_kit/solver/cvrp/__init__.py
 ml4co_kit/solver/cvrp/base.py
+ml4co_kit/solver/cvrp/hgs.py
 ml4co_kit/solver/cvrp/lkh.py
 ml4co_kit/solver/cvrp/pyvrp.py
+ml4co_kit/solver/cvrp/c_hgs/CircleSector.h
+ml4co_kit/solver/cvrp/c_hgs/Genetic.cpp
+ml4co_kit/solver/cvrp/c_hgs/Genetic.h
+ml4co_kit/solver/cvrp/c_hgs/Individual.cpp
+ml4co_kit/solver/cvrp/c_hgs/Individual.h
+ml4co_kit/solver/cvrp/c_hgs/LocalSearch.cpp
+ml4co_kit/solver/cvrp/c_hgs/LocalSearch.h
+ml4co_kit/solver/cvrp/c_hgs/Makefile
+ml4co_kit/solver/cvrp/c_hgs/Params.cpp
+ml4co_kit/solver/cvrp/c_hgs/Params.h
+ml4co_kit/solver/cvrp/c_hgs/Population.cpp
+ml4co_kit/solver/cvrp/c_hgs/Population.h
+ml4co_kit/solver/cvrp/c_hgs/Split.cpp
+ml4co_kit/solver/cvrp/c_hgs/Split.h
+ml4co_kit/solver/cvrp/c_hgs/__init__.py
+ml4co_kit/solver/cvrp/c_hgs/commandline.h
+ml4co_kit/solver/cvrp/c_hgs/cvrp_hgs_solver
+ml4co_kit/solver/cvrp/c_hgs/main.cpp
 ml4co_kit/solver/mis/__init__.py
 ml4co_kit/solver/mis/base.py
 ml4co_kit/solver/mis/gurobi.py
 ml4co_kit/solver/mis/kamis.py
 ml4co_kit/solver/mis/kamis-source/CMakeLists.txt
 ml4co_kit/solver/mis/kamis-source/Doxyfile
 ml4co_kit/solver/mis/kamis-source/cleanup.sh
```

### Comparing `ml4co_kit-0.0.6/setup.py` & `ml4co_kit-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/tests/test_draw.py` & `ml4co_kit-0.0.7/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/tests/test_evaluate.py` & `ml4co_kit-0.0.7/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/tests/test_generator.py` & `ml4co_kit-0.0.7/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ml4co_kit-0.0.6/tests/test_solver.py` & `ml4co_kit-0.0.7/tests/test_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 root_folder = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 sys.path.append(root_folder)
 from ml4co_kit.solver import TSPSolver, TSPLKHSolver, TSPConcordeSolver
 from ml4co_kit.solver import KaMISSolver
-from ml4co_kit.solver import CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver
+from ml4co_kit.solver import CVRPSolver, CVRPPyVRPSolver, CVRPLKHSolver, CVRPHGSSolver
 from ml4co_kit.utils.mis_utils import cnf_folder_to_gpickle_folder
 
 
 ##############################################
 #             Test Func For TSP              #
 ##############################################
 
@@ -172,23 +172,45 @@
 
 
 def test_cvrp_lkh_solver():
     _test_cvrp_lkh_solver(True, 1)
     _test_cvrp_lkh_solver(True, 2)
     _test_cvrp_lkh_solver(False, 1)
     _test_cvrp_lkh_solver(False, 2)
-    
+
+
+def _test_cvrp_hgs_solver(show_time: bool, num_threads: int):
+    cvrp_hgs_solver = CVRPHGSSolver(time_limit=2)
+    cvrp_hgs_solver.from_txt("tests/solver_test/cvrp50_test_small.txt")
+    cvrp_hgs_solver.solve(show_time=show_time, num_threads=num_threads)
+    _, _, gap_avg, _ = cvrp_hgs_solver.evaluate(calculate_gap=True)
+    print(f"CVRPHGSSolver Gap: {gap_avg}")
+    if gap_avg >= 1e-5:
+        message = (
+            f"The average gap ({gap_avg}) of CVRP50 solved by CVRPHGSSolver "
+            "is larger than or equal to 1e-5%."
+        )
+        raise ValueError(message)
+
+
+def test_cvrp_hgs_solver():
+    _test_cvrp_hgs_solver(True, 1)
+    _test_cvrp_hgs_solver(True, 2)
+    _test_cvrp_hgs_solver(False, 1)
+    _test_cvrp_hgs_solver(False, 2)
+
 
 def test_cvrp():
     """
     Test CVRPSolver
     """
     test_cvrp_base_solver()
     test_cvrp_pyvrp_solver()
     test_cvrp_lkh_solver()
+    test_cvrp_hgs_solver()
     
 
 ##############################################
 #                    MAIN                    #
 ##############################################
 
 if __name__ == "__main__":
```

### Comparing `ml4co_kit-0.0.6/tests/test_utils.py` & `ml4co_kit-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*
