# Comparing `tmp/rgrow-0.13.1.tar.gz` & `tmp/rgrow-0.14.0.tar.gz`

## Comparing `rgrow-0.13.1.tar` & `rgrow-0.14.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0     1001      127     1905 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/Cargo.toml
--rw-r--r--   0     1001      127     3580 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/benches/ratestore.drs
--rw-r--r--   0     1001      127     1847 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/benches/sierpinski.drs
--rw-r--r--   0     1001      127      627 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/benches/ui.rs
--rw-r--r--   0     1001      127     3224 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/barish-perfect-sc.yaml
--rwxr-xr-x   0     1001      127     5883 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/barish-perfect.yaml
--rw-r--r--   0     1001      127      167 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/fission-small-ribbon.yaml
--rw-r--r--   0     1001      127     1718 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/sierpinski.yaml
--rw-r--r--   0     1001      127      403 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/tube.yaml
--rwxr-xr-x   0     1001      127      212 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/1dXOR.tiles
--rwxr-xr-x   0     1001      127      478 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/9-square.tiles
--rwxr-xr-x   0     1001      127      165 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/AB.tiles
--rwxr-xr-x   0     1001      127      137 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/ABdiff.tiles
--rwxr-xr-x   0     1001      127      554 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/BarishSeed.tiles
--rwxr-xr-x   0     1001      127      240 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/BinaryCounter.tiles
--rwxr-xr-x   0     1001      127     1357 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles
--rwxr-xr-x   0     1001      127     2661 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/BinaryTree.tiles
--rwxr-xr-x   0     1001      127     3149 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles
--rwxr-xr-x   0     1001      127      171 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/COPY.tiles
--rwxr-xr-x   0     1001      127      215 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/COPYseed.tiles
--rwxr-xr-x   0     1001      127      245 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/CombSquare.tiles
--rwxr-xr-x   0     1001      127      927 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/DiamondSet.tiles
--rwxr-xr-x   0     1001      127      534 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles
--rwxr-xr-x   0     1001      127      544 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110.tiles
--rwxr-xr-x   0     1001      127      643 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110D.tiles
--rwxr-xr-x   0     1001      127      674 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110Drandom.tiles
--rwxr-xr-x   0     1001      127      712 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110V.tiles
--rwxr-xr-x   0     1001      127     2686 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles
--rwxr-xr-x   0     1001      127     3177 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/UL.seed
--rwxr-xr-x   0     1001      127     3041 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/ULcounter.seed
--rwxr-xr-x   0     1001      127      327 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/UnarySquare.tiles
--rwxr-xr-x   0     1001      127      535 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/UnarySquareBig.tiles
--rwxr-xr-x   0     1001      127      561 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/XOR.tiles
--rwxr-xr-x   0     1001      127      801 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/asyncdemo.tiles
--rwxr-xr-x   0     1001      127      185 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/barcode.tiles
--rwxr-xr-x   0     1001      127      229 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/barseed.tiles
--rwxr-xr-x   0     1001      127      528 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/chunk-test.tiles
--rwxr-xr-x   0     1001      127     7278 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles
--rwxr-xr-x   0     1001      127     2491 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles
--rwxr-xr-x   0     1001      127      852 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/crosshatch.tiles
--rwxr-xr-x   0     1001      127      131 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/diagonal.tiles
--rwxr-xr-x   0     1001      127      145 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/linear1.tiles
--rwxr-xr-x   0     1001      127      187 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/linear2.tiles
--rwxr-xr-x   0     1001      127      204 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/linear3.tiles
--rwxr-xr-x   0     1001      127      172 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/lines1.tiles
--rwxr-xr-x   0     1001      127      184 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/lines2.tiles
--rwxr-xr-x   0     1001      127      600 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/reversibleXOR.tiles
--rwxr-xr-x   0     1001      127      840 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski.tiles
--rwxr-xr-x   0     1001      127     1561 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles
--rwxr-xr-x   0     1001      127      737 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski2x2.tiles
--rwxr-xr-x   0     1001      127     6791 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles
--rwxr-xr-x   0     1001      127     2503 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles
--rwxr-xr-x   0     1001      127     2491 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles
--rwxr-xr-x   0     1001      127      874 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski_diag.tiles
--rwxr-xr-x   0     1001      127      700 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/spiral.tiles
--rw-r--r--   0     1001      127      364 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/zig-zag-3w.tiles
--rwxr-xr-x   0     1001      127      614 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles
--rw-r--r--   0     1001      127     6523 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/base.rs
--rw-r--r--   0     1001      127    22198 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/canvas.rs
--rw-r--r--   0     1001      127     3603 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/cffi.rs
--rw-r--r--   0     1001      127    30787 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/colors.rs
--rw-r--r--   0     1001      127    29900 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/ffs.rs
--rw-r--r--   0     1001      127      537 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/lib.rs
--rw-r--r--   0     1001      127     2546 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/main.rs
--rw-r--r--   0     1001      127    33336 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/atam.rs
--rw-r--r--   0     1001      127    14794 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/covers.rs
--rw-r--r--   0     1001      127    58318 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/ktam.rs
--rw-r--r--   0     1001      127    13216 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/ktam_fission.rs
--rw-r--r--   0     1001      127      111 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/mod.rs
--rw-r--r--   0     1001      127    32542 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/oldktam.rs
--rw-r--r--   0     1001      127    12397 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/models/oldktam_fission.rs
--rw-r--r--   0     1001      127    11243 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/parser_xgrow.rs
--rw-r--r--   0     1001      127     9617 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/python.rs
--rw-r--r--   0     1001      127     6980 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/pytileset.rs
--rw-r--r--   0     1001      127     7903 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/ratestore.rs
--rw-r--r--   0     1001      127    14079 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/state.rs
--rw-r--r--   0     1001      127    25286 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/system.rs
--rw-r--r--   0     1001      127    34156 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/src/tileset.rs
--rw-r--r--   0     1001      127     6346 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/tests/main.rs
--rw-r--r--   0     1001      127     1371 2024-06-01 23:11:07.000000 rgrow-0.13.1/README.md
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 rgrow-0.13.1/py-rgrow/Cargo.toml
--rw-r--r--   0     1001      127     1074 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/LICENSE
--rw-r--r--   0     1001      127      634 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/Makefile
--rw-r--r--   0     1001      127      162 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/README.md
--rw-r--r--   0     1001      127       20 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/.gitignore
--rw-r--r--   0     1001      127      638 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/Makefile
--rw-r--r--   0     1001      127      491 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/requirements-docs.txt
--rw-r--r--   0     1001      127     1863 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/source/conf.py
--rw-r--r--   0     1001      127      498 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/source/index.rst
--rw-r--r--   0     1001      127      135 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/source/reference/ffs.rst
--rw-r--r--   0     1001      127     1005 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/source/reference/simulation.rst
--rw-r--r--   0     1001      127      385 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/docs/source/reference/tileset.rst
--rw-r--r--   0     1001      127      736 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/index.rst
--rw-r--r--   0     1001      127    27267 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/rgrow/__init__.py
--rw-r--r--   0     1001      127        0 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/rgrow/py.typed
--rw-r--r--   0     1001      127     5890 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/rgrow/rgrow.pyi
--rw-r--r--   0     1001      127      563 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/src/lib.rs
--rw-r--r--   0     1001      127     1683 2024-06-01 23:11:07.000000 rgrow-0.13.1/py-rgrow/tests/test_runs.py
--rw-r--r--   0     1001      127    75424 2024-06-01 23:11:11.000000 rgrow-0.13.1/Cargo.lock
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 rgrow-0.13.1/Cargo.toml
--rw-r--r--   0        0        0      352 1970-01-01 00:00:00.000000 rgrow-0.13.1/pyproject.toml
--rw-r--r--   0     1001      127    27267 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/__init__.py
--rw-r--r--   0     1001      127        0 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/py.typed
--rw-r--r--   0     1001      127     5890 2024-06-01 23:11:07.000000 rgrow-0.13.1/rgrow/rgrow.pyi
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 rgrow-0.13.1/PKG-INFO
+-rw-r--r--   0     1001      127     1911 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/Cargo.toml
+-rw-r--r--   0     1001      127     3580 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/benches/ratestore.drs
+-rw-r--r--   0     1001      127     1847 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/benches/sierpinski.drs
+-rw-r--r--   0     1001      127      627 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/benches/ui.rs
+-rw-r--r--   0     1001      127     3224 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/barish-perfect-sc.yaml
+-rwxr-xr-x   0     1001      127     5883 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/barish-perfect.yaml
+-rw-r--r--   0     1001      127      167 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/fission-small-ribbon.yaml
+-rw-r--r--   0     1001      127     1718 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/sierpinski.yaml
+-rw-r--r--   0     1001      127      403 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/tube.yaml
+-rwxr-xr-x   0     1001      127      212 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/1dXOR.tiles
+-rwxr-xr-x   0     1001      127      478 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/9-square.tiles
+-rwxr-xr-x   0     1001      127      165 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/AB.tiles
+-rwxr-xr-x   0     1001      127      137 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/ABdiff.tiles
+-rwxr-xr-x   0     1001      127      554 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/BarishSeed.tiles
+-rwxr-xr-x   0     1001      127      240 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/BinaryCounter.tiles
+-rwxr-xr-x   0     1001      127     1357 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles
+-rwxr-xr-x   0     1001      127     2661 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/BinaryTree.tiles
+-rwxr-xr-x   0     1001      127     3149 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles
+-rwxr-xr-x   0     1001      127      171 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/COPY.tiles
+-rwxr-xr-x   0     1001      127      215 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/COPYseed.tiles
+-rwxr-xr-x   0     1001      127      245 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/CombSquare.tiles
+-rwxr-xr-x   0     1001      127      927 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/DiamondSet.tiles
+-rwxr-xr-x   0     1001      127      534 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles
+-rwxr-xr-x   0     1001      127      544 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110.tiles
+-rwxr-xr-x   0     1001      127      643 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110D.tiles
+-rwxr-xr-x   0     1001      127      674 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110Drandom.tiles
+-rwxr-xr-x   0     1001      127      712 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110V.tiles
+-rwxr-xr-x   0     1001      127     2686 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles
+-rwxr-xr-x   0     1001      127     3177 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/UL.seed
+-rwxr-xr-x   0     1001      127     3041 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/ULcounter.seed
+-rwxr-xr-x   0     1001      127      327 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/UnarySquare.tiles
+-rwxr-xr-x   0     1001      127      535 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/UnarySquareBig.tiles
+-rwxr-xr-x   0     1001      127      561 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/XOR.tiles
+-rwxr-xr-x   0     1001      127      801 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/asyncdemo.tiles
+-rwxr-xr-x   0     1001      127      185 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/barcode.tiles
+-rwxr-xr-x   0     1001      127      229 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/barseed.tiles
+-rwxr-xr-x   0     1001      127      528 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/chunk-test.tiles
+-rwxr-xr-x   0     1001      127     7278 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      127     2491 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      127      852 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/crosshatch.tiles
+-rwxr-xr-x   0     1001      127      131 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/diagonal.tiles
+-rwxr-xr-x   0     1001      127      145 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/linear1.tiles
+-rwxr-xr-x   0     1001      127      187 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/linear2.tiles
+-rwxr-xr-x   0     1001      127      204 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/linear3.tiles
+-rwxr-xr-x   0     1001      127      172 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/lines1.tiles
+-rwxr-xr-x   0     1001      127      184 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/lines2.tiles
+-rwxr-xr-x   0     1001      127      600 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/reversibleXOR.tiles
+-rwxr-xr-x   0     1001      127      840 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski.tiles
+-rwxr-xr-x   0     1001      127     1561 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles
+-rwxr-xr-x   0     1001      127      737 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski2x2.tiles
+-rwxr-xr-x   0     1001      127     6791 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      127     2503 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles
+-rwxr-xr-x   0     1001      127     2491 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      127      874 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski_diag.tiles
+-rwxr-xr-x   0     1001      127      700 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/spiral.tiles
+-rw-r--r--   0     1001      127      364 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/zig-zag-3w.tiles
+-rwxr-xr-x   0     1001      127      614 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles
+-rw-r--r--   0     1001      127     6523 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/base.rs
+-rw-r--r--   0     1001      127    22198 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/canvas.rs
+-rw-r--r--   0     1001      127     3603 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/cffi.rs
+-rw-r--r--   0     1001      127    30787 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/colors.rs
+-rw-r--r--   0     1001      127    31219 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/ffs.rs
+-rw-r--r--   0     1001      127      537 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/lib.rs
+-rw-r--r--   0     1001      127     2546 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/main.rs
+-rw-r--r--   0     1001      127    33336 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/atam.rs
+-rw-r--r--   0     1001      127    14794 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/covers.rs
+-rw-r--r--   0     1001      127    58318 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/ktam.rs
+-rw-r--r--   0     1001      127    13216 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/ktam_fission.rs
+-rw-r--r--   0     1001      127      111 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/mod.rs
+-rw-r--r--   0     1001      127    32542 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/oldktam.rs
+-rw-r--r--   0     1001      127    12397 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/models/oldktam_fission.rs
+-rw-r--r--   0     1001      127    11243 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/parser_xgrow.rs
+-rw-r--r--   0     1001      127    10238 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/python.rs
+-rw-r--r--   0     1001      127     6980 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/pytileset.rs
+-rw-r--r--   0     1001      127     7903 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/ratestore.rs
+-rw-r--r--   0     1001      127    15303 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/state.rs
+-rw-r--r--   0     1001      127    25286 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/system.rs
+-rw-r--r--   0     1001      127    34156 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/src/tileset.rs
+-rw-r--r--   0     1001      127     6346 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/tests/main.rs
+-rw-r--r--   0     1001      127     1371 2024-06-02 20:24:16.000000 rgrow-0.14.0/README.md
+-rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 rgrow-0.14.0/py-rgrow/Cargo.toml
+-rw-r--r--   0     1001      127     1074 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/LICENSE
+-rw-r--r--   0     1001      127      634 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/Makefile
+-rw-r--r--   0     1001      127      162 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/README.md
+-rw-r--r--   0     1001      127       20 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/.gitignore
+-rw-r--r--   0     1001      127      638 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/Makefile
+-rw-r--r--   0     1001      127      491 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/requirements-docs.txt
+-rw-r--r--   0     1001      127     1863 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/source/conf.py
+-rw-r--r--   0     1001      127      498 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/source/index.rst
+-rw-r--r--   0     1001      127      135 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/source/reference/ffs.rst
+-rw-r--r--   0     1001      127     1005 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/source/reference/simulation.rst
+-rw-r--r--   0     1001      127      385 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/docs/source/reference/tileset.rst
+-rw-r--r--   0     1001      127      736 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/index.rst
+-rw-r--r--   0     1001      127    27355 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/rgrow/__init__.py
+-rw-r--r--   0     1001      127        0 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/rgrow/py.typed
+-rw-r--r--   0     1001      127     6434 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/rgrow/rgrow.pyi
+-rw-r--r--   0     1001      127      610 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/src/lib.rs
+-rw-r--r--   0     1001      127     1683 2024-06-02 20:24:16.000000 rgrow-0.14.0/py-rgrow/tests/test_runs.py
+-rw-r--r--   0     1001      127    75424 2024-06-02 20:24:27.000000 rgrow-0.14.0/Cargo.lock
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 rgrow-0.14.0/Cargo.toml
+-rw-r--r--   0        0        0      352 1970-01-01 00:00:00.000000 rgrow-0.14.0/pyproject.toml
+-rw-r--r--   0     1001      127    27355 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/__init__.py
+-rw-r--r--   0     1001      127        0 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/py.typed
+-rw-r--r--   0     1001      127     6434 2024-06-02 20:24:16.000000 rgrow-0.14.0/rgrow/rgrow.pyi
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 rgrow-0.14.0/PKG-INFO
```

### Comparing `rgrow-0.13.1/rgrow/Cargo.toml` & `rgrow-0.14.0/rgrow/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #crate_type = ["rlib", "cdylib"]
 
 [[bin]]
 name = "rgrow"
 path = "src/main.rs"
 
 [features]
-default = ["use_rayon"]
+default = ["use_rayon", "ui"]
 ui = ["fltk", "pixels"]
 use_rayon = ["rayon"]
 python = ["pyo3", "numpy"]
 
 [dependencies]
 fltk = { version = "^1.4", features = [
     "rwh05",
```

### Comparing `rgrow-0.13.1/rgrow/benches/ratestore.drs` & `rgrow-0.14.0/rgrow/benches/ratestore.drs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/benches/sierpinski.drs` & `rgrow-0.14.0/rgrow/benches/sierpinski.drs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/benches/ui.rs` & `rgrow-0.14.0/rgrow/benches/ui.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/barish-perfect-sc.yaml` & `rgrow-0.14.0/rgrow/examples/barish-perfect-sc.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/barish-perfect.yaml` & `rgrow-0.14.0/rgrow/examples/barish-perfect.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/sierpinski.yaml` & `rgrow-0.14.0/rgrow/examples/sierpinski.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/BarishSeed.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/BarishSeed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/BinaryTree.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/BinaryTree.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/DiamondSet.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/DiamondSet.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110D.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110D.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110Drandom.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110Drandom.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/Rule110V.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/Rule110V.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/UL.seed` & `rgrow-0.14.0/rgrow/examples/xgrow-format/UL.seed`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/ULcounter.seed` & `rgrow-0.14.0/rgrow/examples/xgrow-format/ULcounter.seed`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/UnarySquareBig.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/UnarySquareBig.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/XOR.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/XOR.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/asyncdemo.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/asyncdemo.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/chunk-test.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/chunk-test.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/crosshatch.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/crosshatch.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/reversibleXOR.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/reversibleXOR.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski2x2.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski2x2.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/sierpinski_diag.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/sierpinski_diag.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/spiral.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/spiral.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles` & `rgrow-0.14.0/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/base.rs` & `rgrow-0.14.0/rgrow/src/base.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/canvas.rs` & `rgrow-0.14.0/rgrow/src/canvas.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/cffi.rs` & `rgrow-0.14.0/rgrow/src/cffi.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/colors.rs` & `rgrow-0.14.0/rgrow/src/colors.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/ffs.rs` & `rgrow-0.14.0/rgrow/src/ffs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 use crate::models::oldktam::OldKTAM;
 use crate::state::{NullStateTracker, QuadTreeState};
 use crate::system::{EvolveBounds, SystemWithDimers};
 use crate::tileset::{CanvasType, FromTileSet, Model, TileSet, SIZE_DEFAULT};
 
 #[cfg(feature = "python")]
 use polars::prelude::*;
+#[cfg(feature = "python")]
+use python::PyState;
 
 use super::*;
 //use ndarray::prelude::*;
 //use ndarray::Zip;
 use base::{NumTiles, Rate};
 
 use ndarray::{s, ArrayView2};
@@ -36,15 +38,15 @@
 use self::state::OrderTracker;
 use self::tileset::TrackingType;
 #[cfg(feature = "python")]
 use numpy::PyArray1;
 #[cfg(feature = "python")]
 use pyo3_polars::PyDataFrame;
 
-use state::{State, StateWithCreate};
+use state::{ClonableState, StateWithCreate};
 
 use system::{Orientation, System};
 //use std::convert::{TryFrom, TryInto};
 
 /// Configuration options for FFS.
 #[derive(Debug, Clone)]
 #[cfg_attr(feature = "python", pyclass(get_all, set_all))]
@@ -210,24 +212,25 @@
     fn dimerization_rate(&self) -> f64;
     fn surfaces(&self) -> Vec<&dyn FFSSurface>;
     fn get_surface(&self, i: usize) -> &dyn FFSSurface;
 }
 
 pub trait FFSSurface: Send + Sync {
     fn get_config(&self, i: usize) -> ArrayView2<Tile>;
-    fn get_state(&self, i: usize) -> &dyn State;
-    fn states(&self) -> Vec<&dyn State> {
-        (0..self.num_configs()).map(|i| self.get_state(i)).collect()
+    fn get_state(&self, i: usize) -> &dyn ClonableState;
+    fn states(&self) -> Vec<&dyn ClonableState> {
+        (0..self.num_stored_states()).map(|i| self.get_state(i)).collect()
     }
     fn configs(&self) -> Vec<ArrayView2<Tile>> {
-        (0..self.num_configs())
+        (0..self.num_stored_states())
             .map(|i| self.get_config(i))
             .collect()
     }
     fn previous_list(&self) -> Vec<usize>;
+    fn num_stored_states(&self) -> usize;
     fn num_configs(&self) -> usize;
     fn num_trials(&self) -> usize;
     fn target_size(&self) -> NumTiles;
     fn p_r(&self) -> f64;
 }
 
 impl TileSet {
@@ -314,21 +317,21 @@
                     self, config,
                 )?,
             )),
         }
     }
 }
 
-pub struct FFSRun<St: State> {
+pub struct FFSRun<St: ClonableState> {
     pub level_list: Vec<FFSLevel<St>>,
     pub dimerization_rate: f64,
     pub forward_prob: Vec<f64>,
 }
 
-impl<St: State> FFSResult for FFSRun<St> {
+impl<St: ClonableState> FFSResult for FFSRun<St> {
     fn nucleation_rate(&self) -> Rate {
         self.dimerization_rate * self.forward_prob.iter().fold(1., |acc, level| acc * *level)
     }
 
     fn forward_vec(&self) -> &Vec<f64> {
         &self.forward_prob
     }
@@ -345,15 +348,15 @@
     }
 
     fn dimerization_rate(&self) -> f64 {
         self.dimerization_rate
     }
 }
 
-impl<St: State + StateWithCreate<Params = (usize, usize)>> FFSRun<St> {
+impl<St: ClonableState + StateWithCreate<Params = (usize, usize)>> FFSRun<St> {
     pub fn create<Sy: SystemWithDimers + System>(
         system: &mut Sy,
         config: &FFSRunConfig,
     ) -> Result<Self, GrowError> {
         let level_list = Vec::new();
 
         let dimerization_rate = system
@@ -417,15 +420,15 @@
         Ok(ret)
     }
     pub fn dimer_conc(&self) -> f64 {
         self.level_list[0].p_r
     }
 }
 
-impl<St: State + StateWithCreate<Params = (usize, usize)>> FFSRun<St> {
+impl<St: ClonableState + StateWithCreate<Params = (usize, usize)>> FFSRun<St> {
     pub fn create_from_tileset<Sy: SystemWithDimers + System + FromTileSet>(
         tileset: &TileSet,
         config: &FFSRunConfig,
     ) -> Result<Self, RgrowError> {
         let mut sys = Sy::from_tileset(tileset)?;
         let c = {
             let mut c = config.clone();
@@ -466,29 +469,29 @@
     }
 
     let subarr = arr.slice(s![mini..maxi + 1, minj..maxj + 1]);
 
     (subarr, mini, minj, maxi, maxj)
 }
 
-pub struct FFSLevel<St: State> {
+pub struct FFSLevel<St: ClonableState> {
     pub state_list: Vec<St>,
     pub previous_list: Vec<usize>,
     pub p_r: f64,
     pub num_states: usize,
     pub num_trials: usize,
     pub target_size: NumTiles,
 }
 
-impl<St: State> FFSSurface for FFSLevel<St> {
+impl<St: ClonableState> FFSSurface for FFSLevel<St> {
     fn get_config(&self, i: usize) -> ArrayView2<Tile> {
         self.state_list[i].raw_array()
     }
 
-    fn get_state(&self, i: usize) -> &dyn State {
+    fn get_state(&self, i: usize) -> &dyn ClonableState {
         self.state_list.get(i).unwrap()
     }
 
     fn num_configs(&self) -> usize {
         self.num_states
     }
 
@@ -503,17 +506,21 @@
     fn previous_list(&self) -> Vec<usize> {
         self.previous_list.clone()
     }
 
     fn p_r(&self) -> f64 {
         self.p_r
     }
+    
+    fn num_stored_states(&self) -> usize {
+        self.state_list.len()
+    }
 }
 
-impl<St: State + StateWithCreate<Params = (usize, usize)>> FFSLevel<St> {
+impl<St: ClonableState + StateWithCreate<Params = (usize, usize)>> FFSLevel<St> {
     pub fn drop_states(&mut self) -> &Self {
         self.state_list.drain(..);
         self
     }
 
     pub fn next_level<Sy: SystemWithDimers + System>(
         &self,
@@ -870,14 +877,29 @@
             .configs()
             .iter()
             .map(|x| x.to_pyarray_bound(py))
             .collect()
     }
 
     #[getter]
+    fn get_states<'py>(&self) -> Vec<FFSStateRef> {
+        self.res
+            .get_surface(self.level)
+            .states()
+            .iter()
+            .enumerate()
+            .map(|(i, x)| FFSStateRef {
+                res: self.res.clone(),
+                level: self.level,
+                state: i,
+            })
+            .collect()
+    }
+
+    #[getter]
     fn get_previous_indices(&self) -> Vec<usize> {
         self.res.get_surface(self.level).previous_list()
     }
 
     #[getter]
     fn level(&self) -> usize {
         self.level
@@ -886,27 +908,43 @@
     fn get_state(&self, i: usize) -> FFSStateRef {
         FFSStateRef {
             res: self.res.clone(),
             level: self.level,
             state: i,
         }
     }
+
+    fn has_stored_states(&self) -> bool {
+        self.res.get_surface(self.level).num_stored_states() > 0
+    }
+
+    fn __repr__(&self) -> String {
+        format!(
+            "FFSLevelRef(n_configs={}, n_trials={}, target_size={}, p_r={}, has_stored_states={})",
+            self.res.get_surface(self.level).num_configs(),
+            self.res.get_surface(self.level).num_trials(),
+            self.res.get_surface(self.level).target_size(),
+            self.res.get_surface(self.level).p_r(),
+            self.has_stored_states()
+        )
+    }
 }
 
 #[cfg_attr(feature = "python", pyclass)]
 #[allow(dead_code)] // This is used in the python interface
+#[derive(Clone)]
 pub struct FFSStateRef {
     res: Arc<Box<dyn ffs::FFSResult>>,
     level: usize,
     state: usize,
 }
 
 #[cfg(feature = "python")]
 impl FFSStateRef {
-    fn get_st(&self) -> &dyn State {
+    fn get_st(&self) -> &dyn ClonableState {
         self.res.get_surface(self.level).get_state(self.state)
     }
 }
 
 #[cfg(feature = "python")]
 #[pymethods]
 impl FFSStateRef {
@@ -918,29 +956,33 @@
         self.get_st().total_events()
     }
 
     pub fn n_tiles(&self) -> NumTiles {
         self.get_st().n_tiles()
     }
 
+    pub fn clone_state(&self) -> PyState {
+        PyState(self.get_st().clone_as_stateenum())
+    }
+
     #[getter]
     /// A direct, mutable view of the state's canvas.  This is potentially unsafe.
     pub fn canvas_view<'py>(
         this: Bound<'py, Self>,
         _py: Python<'py>,
     ) -> PyResult<Bound<'py, PyArray2<crate::base::Tile>>> {
         let t = this.borrow();
         let ra = t.get_st().raw_array();
 
         unsafe { Ok(PyArray2::borrow_from_array_bound(&ra, this.into_any())) }
     }
 
     /// A copy of the state's canvas.  This is safe, but can't be modified and is slower than `canvas_view`.
     pub fn canvas_copy<'py>(
-        this: &Bound<'py, Self>,
+        this: &Bound<Self>,
         py: Python<'py>,
     ) -> PyResult<Bound<'py, PyArray2<crate::base::Tile>>> {
         let t = this.borrow();
         let ra = t.get_st().raw_array();
 
         Ok(PyArray2::from_array_bound(py, &ra))
     }
```

### Comparing `rgrow-0.13.1/rgrow/src/lib.rs` & `rgrow-0.14.0/rgrow/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/main.rs` & `rgrow-0.14.0/rgrow/src/main.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/atam.rs` & `rgrow-0.14.0/rgrow/src/models/atam.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/covers.rs` & `rgrow-0.14.0/rgrow/src/models/covers.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/ktam.rs` & `rgrow-0.14.0/rgrow/src/models/ktam.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/ktam_fission.rs` & `rgrow-0.14.0/rgrow/src/models/ktam_fission.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/oldktam.rs` & `rgrow-0.14.0/rgrow/src/models/oldktam.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/models/oldktam_fission.rs` & `rgrow-0.14.0/rgrow/src/models/oldktam_fission.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/parser_xgrow.rs` & `rgrow-0.14.0/rgrow/src/parser_xgrow.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/python.rs` & `rgrow-0.14.0/rgrow/src/python.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::ops::DerefMut;
 use std::time::Duration;
 
 use crate::base::{NumEvents, NumTiles, RustAny, Tile};
 use crate::canvas::Canvas;
-use crate::ffs::{BoxedFFSResult, FFSRunConfig};
+use crate::ffs::{BoxedFFSResult, FFSRunConfig, FFSStateRef};
 use crate::ratestore::RateStore;
-use crate::state::{StateEnum, StateStatus, TrackerData};
+use crate::state::{ClonableState, StateEnum, StateStatus, TrackerData};
 use crate::system::{
     DynSystem, EvolveBounds, EvolveOutcome, NeededUpdate, SystemEnum, TileBondInfo,
 };
 use crate::tileset::CanvasType;
 use ndarray::Array2;
 use numpy::{IntoPyArray, PyArray2};
 use pyo3::prelude::*;
@@ -99,21 +99,35 @@
 pub enum PyStateOrStates<'py> {
     #[pyo3(transparent)]
     State(Bound<'py, PyState>),
     #[pyo3(transparent)]
     States(Vec<Bound<'py, PyState>>),
 }
 
+#[cfg(feature = "python")]
+#[derive(FromPyObject)]
+
+pub enum PyStateOrRef<'py> {
+    State(Bound<'py, PyState>),
+    Ref(Bound<'py, FFSStateRef>),
+}
+
 #[repr(transparent)]
 #[cfg_attr(
     feature = "python",
     pyclass(module = "rgrow", name = "System", subclass)
 )]
 pub struct PySystem(pub SystemEnum);
 
+impl From<FFSStateRef> for PyState {
+    fn from(state: FFSStateRef) -> Self {
+        state.clone_state()
+    }
+}
+
 #[cfg(feature = "python")]
 #[pymethods]
 impl PySystem {
     #[allow(clippy::too_many_arguments)]
     #[pyo3(
         name = "evolve",
         signature = (state,
@@ -210,25 +224,31 @@
                     .map(|x| x.map_err(|y| pyo3::exceptions::PyValueError::new_err(y.to_string())))
                     .collect();
                 o.map(|x| x.into_py(py))
             }
         }
     }
 
-    fn calc_mismatches(&self, state: &PyState) -> usize {
-        self.0.calc_mismatches(&state.0)
+    fn calc_mismatches(&self, state: PyStateOrRef) -> usize {
+        match state {
+            PyStateOrRef::State(s) => self.0.calc_mismatches(&s.borrow().0),
+            PyStateOrRef::Ref(s) => self.0.calc_mismatches(&s.borrow().clone_state().0),
+        }
     }
 
     fn calc_mismatch_locations<'py>(
         this: &Bound<'py, Self>,
-        state: &PyState,
+        state: PyStateOrRef,
         py: Python<'py>,
     ) -> PyResult<Bound<'py, PyArray2<usize>>> {
         let t = this.borrow();
-        let ra = t.0.calc_mismatch_locations(&state.0);
+        let ra = match state {
+            PyStateOrRef::State(s) => t.0.calc_mismatch_locations(&s.borrow().0),
+            PyStateOrRef::Ref(s) => t.0.calc_mismatch_locations(&s.borrow().clone_state().0),
+        };
         Ok(PyArray2::from_array_bound(py, &ra))
     }
 
     fn set_param(&mut self, param_name: &str, value: RustAny) -> PyResult<NeededUpdate> {
         Ok(self.0.set_param(param_name, value.0)?)
     }
```

### Comparing `rgrow-0.13.1/rgrow/src/pytileset.rs` & `rgrow-0.14.0/rgrow/src/pytileset.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/ratestore.rs` & `rgrow-0.14.0/rgrow/src/ratestore.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/state.rs` & `rgrow-0.14.0/rgrow/src/state.rs`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,58 @@
 use std::fmt::Debug;
 
 #[enum_dispatch]
 pub trait State: RateStore + Canvas + StateStatus + Sync + Send + TrackerData {
     fn panicinfo(&self) -> String;
 }
 
-#[enum_dispatch(State, StateStatus, Canvas, RateStore, TrackerData)]
+#[enum_dispatch]
+pub trait ClonableState: State {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        panic!("Not implemented")
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasSquare, OrderTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::SquareOrderTracking(self.clone())
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasSquare, NullStateTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::SquareNoTracking(self.clone())
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasPeriodic, OrderTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::PeriodicOrderTracking(self.clone())
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasPeriodic, NullStateTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::PeriodicNoTracking(self.clone())
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasTube, OrderTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::TubeOrderTracking(self.clone())
+    }
+}
+
+impl ClonableState for QuadTreeState<CanvasTube, NullStateTracker> {
+    fn clone_as_stateenum(&self) -> StateEnum {
+        StateEnum::TubeNoTracking(self.clone())
+    }
+}
+
+#[enum_dispatch(State, StateStatus, Canvas, RateStore, TrackerData, CloneAsStateEnum)]
 #[derive(Debug, Clone)]
 pub enum StateEnum {
     SquareNoTracking(QuadTreeState<CanvasSquare, NullStateTracker>),
     PeriodicNoTracking(QuadTreeState<CanvasPeriodic, NullStateTracker>),
     TubeNoTracking(QuadTreeState<CanvasTube, NullStateTracker>),
     SquareOrderTracking(QuadTreeState<CanvasSquare, OrderTracker>),
     PeriodicOrderTracking(QuadTreeState<CanvasPeriodic, OrderTracker>),
```

### Comparing `rgrow-0.13.1/rgrow/src/system.rs` & `rgrow-0.14.0/rgrow/src/system.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/src/tileset.rs` & `rgrow-0.14.0/rgrow/src/tileset.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/rgrow/tests/main.rs` & `rgrow-0.14.0/rgrow/tests/main.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/README.md` & `rgrow-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/Cargo.toml` & `rgrow-0.14.0/py-rgrow/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 numpy = { workspace = true }
 rayon = { version = "1", optional = true }
 polars = {workspace = true}
 pyo3-polars = {workspace = true}
 
 [dependencies.rgrow]
 path = "../rgrow"
-features = ["python"]
+features = ["python", "use_rayon"]
 default-features = false
 
 [dependencies.pyo3]
 workspace = true
 features = ["extension-module"]
```

### Comparing `rgrow-0.13.1/py-rgrow/LICENSE` & `rgrow-0.14.0/py-rgrow/LICENSE`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/Makefile` & `rgrow-0.14.0/py-rgrow/Makefile`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/docs/Makefile` & `rgrow-0.14.0/py-rgrow/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/docs/source/conf.py` & `rgrow-0.14.0/py-rgrow/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/docs/source/reference/simulation.rst` & `rgrow-0.14.0/py-rgrow/docs/source/reference/simulation.rst`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/index.rst` & `rgrow-0.14.0/py-rgrow/index.rst`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/py-rgrow/rgrow/__init__.py` & `rgrow-0.14.0/py-rgrow/rgrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,28 @@
     EvolveOutcome,
     # FFSLevel,
     FFSResult,
     FFSRunConfig,
     System,
     State,
     EvolveBounds,
+    FFSStateRef
 )
 import attrs
 import attr
 
 
 from typing import TYPE_CHECKING, Any, List, Optional, Sequence, Tuple
 
 if TYPE_CHECKING:  # pragma: no cover
     import matplotlib.pyplot as plt
     import matplotlib.colors
 
 
-def _system_name_canvas(self: System, state: State) -> np.ndarray:
+def _system_name_canvas(self: System, state: State | FFSStateRef) -> np.ndarray:
     """Returns the current canvas for state, as an array of tile names.
     'empty' indicates empty locations; numbers are translated to strings.
 
     Parameters
     ----------
     state : State
       The state to return.
@@ -51,41 +52,41 @@
     a = np.array(self.tile_names)
     return a[state.canvas_view]
 
 
 System.name_canvas = _system_name_canvas  # type: ignore
 
 
-def _system_color_canvas(self: System, state: State | np.ndarray) -> np.ndarray:
+def _system_color_canvas(self: System, state: State | np.ndarray | FFSStateRef) -> np.ndarray:
     """Returns the current canvas for state, as an array of tile colors."""
 
-    if isinstance(state, State):
+    if isinstance(state, (State, FFSStateRef)):
         return self.tile_colors[state.canvas_view]
     else:
         return self.tile_colors[state]
 
 
 System.color_canvas = _system_color_canvas  # type: ignore
 
 
 def _system_plot_canvas(
     sys: System,
-    state: State | np.ndarray,
+    state: State | np.ndarray | FFSStateRef,
     ax=None,
     annotate_tiles=False,
     annotate_mismatches=False,
     crop=False,
 ) -> "plt.Axes":
     import matplotlib.pyplot as plt
     import numpy as np
 
     if ax is None:
         _, ax = plt.subplots(figsize=(6, 6), constrained_layout=True)
 
-    if isinstance(state, State):
+    if isinstance(state, (State, FFSStateRef)):
         cv = state.canvas_view
     else:
         cv = state
 
     rows, cols = cv.shape
 
     if crop:
```

### Comparing `rgrow-0.13.1/py-rgrow/rgrow/rgrow.pyi` & `rgrow-0.14.0/py-rgrow/rgrow/rgrow.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Sequence, overload
 import numpy as np
 import polars as pl
 
 if TYPE_CHECKING:  # pragma: no cover
-    import matplotlib.pyplot as plt
+    from matplotlib.axes import Axes
 
 class TileShape(Enum):
     Single = ...
     Vertical = ...
     Horizontal = ...
 
 class EvolveOutcome(object): ...
@@ -55,46 +55,64 @@
         size_min=float | None,
         size_max=float | None,
         for_wall_time: float | None = None,
         require_strong_bound: bool = True,
         show_window: bool = False,
         parallel: bool = True,
     ) -> list[EvolveOutcome]: ...
-    def calc_mismatches(self, state: State) -> int: ...
-    def calc_mismatch_locations(self, state: State) -> np.ndarray: ...
-    def name_canvas(self, state: State) -> np.ndarray: ...
-    def color_canvas(self, state: State | np.ndarray) -> np.ndarray: ...
+    def calc_mismatches(self, state: State | FFSStateRef) -> int: ...
+    def calc_mismatch_locations(self, state: State | FFSStateRef) -> np.ndarray: ...
+    def name_canvas(self, state: State | FFSStateRef) -> np.ndarray: ...
+    def color_canvas(self, state: State | np.ndarray | FFSStateRef) -> np.ndarray: ...
     @property
     def tile_names(self) -> list[str]: ...
     @property
     def tile_colors(self) -> np.ndarray: ...
     def update_all(self, state: State, needed) -> None: ...
     def plot_canvas(
         self,
         state: State,
         ax=None,
         annotate_tiles=False,
         annotate_mismatches=False,
         crop=False,
-    ) -> "plt.Axes": ...
+    ) -> "Axes": ...
     def get_param(self, name: str) -> Any: ...
     def set_param(self, name: str, value: Any): ...
 
 class FissionHandling(object): ...
 class CanvasType(object): ...
 class ChunkSize(object): ...
 class ChunkHandling(object): ...
 class Model(object): ...
 
-class FFSLevel(object):
+class FFSStateRef(object):
+    @property
+    def canvas_view(self) -> np.ndarray: ...
+    def canvas_copy(self) -> np.ndarray: ...
+    @property
+    def n_tiles(self) -> int: ...
+    @property
+    def total_events(self) -> int: ...
+    @property
+    def time(self) -> float: ...
+    def tracking_copy(self) -> np.ndarray: ...
+    def clone_state(self) -> State: ...
+    
+
+class FFSLevelRef(object):
     @property
     def configs(self) -> list[np.ndarray]:
         """List of configurations at this level, as arrays (not full states)."""
         ...
     @property
+    def states(self) -> list[FFSStateRef]:
+        """List of states at this level."""
+        ...
+    @property
     def previous_indices(self) -> list[int]:
         """For each configuration, the index of the configuration in the previous
         level that resulted in it."""
         ...
 
 class FFSResult(object):
     @property
@@ -104,15 +122,15 @@
         """
         ...
     @property
     def forward_vec(self) -> np.ndarray: ...
     @property
     def dimerization_rate(self) -> float: ...
     @property
-    def surfaces(self) -> list[FFSLevel]: ...
+    def surfaces(self) -> list[FFSLevelRef]: ...
     @property
     def previous_indices(self) -> list[list[int]]: ...
     def configs_dataframe(self) -> pl.DataFrame: ...
     def surfaces_dataframe(self) -> pl.DataFrame: ...
 
 class Tile(object):
     def __init__(
```

### Comparing `rgrow-0.13.1/py-rgrow/tests/test_runs.py` & `rgrow-0.14.0/py-rgrow/tests/test_runs.py`

 * *Files identical despite different names*

### Comparing `rgrow-0.13.1/Cargo.lock` & `rgrow-0.14.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1856,17 +1856,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.84"
+version = "1.0.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
+checksum = "22244ce15aa966053a896d1accb3a6e68469b97c7f33f284b99f0d576879fc23"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "profiling"
 version = "1.0.15"
@@ -1956,15 +1956,15 @@
  "polars-core",
  "pyo3",
  "thiserror",
 ]
 
 [[package]]
 name = "pyrgrow"
-version = "0.13.1"
+version = "0.14.0"
 dependencies = [
  "bincode",
  "indent",
  "ndarray",
  "numpy",
  "polars",
  "pyo3",
@@ -2133,15 +2133,15 @@
 name = "renderdoc-sys"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b30a45b0cd0bcca8037f3d0dc3421eaf95327a17cad11964fb8179b4fc4832"
 
 [[package]]
 name = "rgrow"
-version = "0.13.1"
+version = "0.14.0"
 dependencies = [
  "anyhow",
  "bimap",
  "cached",
  "clap 4.5.4",
  "criterion",
  "enum_dispatch",
```

### Comparing `rgrow-0.13.1/Cargo.toml` & `rgrow-0.14.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 rayon = { version = "1" }
 numpy = "^0.21"
 enum_dispatch = "0.3"
 pyo3-polars = "^0.14"
 polars = {version = "^0.40", features = ["lazy"]}
 
 [workspace.package]
-version = "0.13.1"
+version = "0.14.0"
 authors = ["Constantine Evans <const@costi.net>"]
 edition = "2021"
 repository = "https://github.com/cgevans/rgrow"
 license = "BSD-3-Clause"
 categories = ["science", "simulation"]
 
 [profile.release]
```

### Comparing `rgrow-0.13.1/rgrow/__init__.py` & `rgrow-0.14.0/rgrow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,28 @@
     EvolveOutcome,
     # FFSLevel,
     FFSResult,
     FFSRunConfig,
     System,
     State,
     EvolveBounds,
+    FFSStateRef
 )
 import attrs
 import attr
 
 
 from typing import TYPE_CHECKING, Any, List, Optional, Sequence, Tuple
 
 if TYPE_CHECKING:  # pragma: no cover
     import matplotlib.pyplot as plt
     import matplotlib.colors
 
 
-def _system_name_canvas(self: System, state: State) -> np.ndarray:
+def _system_name_canvas(self: System, state: State | FFSStateRef) -> np.ndarray:
     """Returns the current canvas for state, as an array of tile names.
     'empty' indicates empty locations; numbers are translated to strings.
 
     Parameters
     ----------
     state : State
       The state to return.
@@ -51,41 +52,41 @@
     a = np.array(self.tile_names)
     return a[state.canvas_view]
 
 
 System.name_canvas = _system_name_canvas  # type: ignore
 
 
-def _system_color_canvas(self: System, state: State | np.ndarray) -> np.ndarray:
+def _system_color_canvas(self: System, state: State | np.ndarray | FFSStateRef) -> np.ndarray:
     """Returns the current canvas for state, as an array of tile colors."""
 
-    if isinstance(state, State):
+    if isinstance(state, (State, FFSStateRef)):
         return self.tile_colors[state.canvas_view]
     else:
         return self.tile_colors[state]
 
 
 System.color_canvas = _system_color_canvas  # type: ignore
 
 
 def _system_plot_canvas(
     sys: System,
-    state: State | np.ndarray,
+    state: State | np.ndarray | FFSStateRef,
     ax=None,
     annotate_tiles=False,
     annotate_mismatches=False,
     crop=False,
 ) -> "plt.Axes":
     import matplotlib.pyplot as plt
     import numpy as np
 
     if ax is None:
         _, ax = plt.subplots(figsize=(6, 6), constrained_layout=True)
 
-    if isinstance(state, State):
+    if isinstance(state, (State, FFSStateRef)):
         cv = state.canvas_view
     else:
         cv = state
 
     rows, cols = cv.shape
 
     if crop:
```

### Comparing `rgrow-0.13.1/rgrow/rgrow.pyi` & `rgrow-0.14.0/rgrow/rgrow.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Sequence, overload
 import numpy as np
 import polars as pl
 
 if TYPE_CHECKING:  # pragma: no cover
-    import matplotlib.pyplot as plt
+    from matplotlib.axes import Axes
 
 class TileShape(Enum):
     Single = ...
     Vertical = ...
     Horizontal = ...
 
 class EvolveOutcome(object): ...
@@ -55,46 +55,64 @@
         size_min=float | None,
         size_max=float | None,
         for_wall_time: float | None = None,
         require_strong_bound: bool = True,
         show_window: bool = False,
         parallel: bool = True,
     ) -> list[EvolveOutcome]: ...
-    def calc_mismatches(self, state: State) -> int: ...
-    def calc_mismatch_locations(self, state: State) -> np.ndarray: ...
-    def name_canvas(self, state: State) -> np.ndarray: ...
-    def color_canvas(self, state: State | np.ndarray) -> np.ndarray: ...
+    def calc_mismatches(self, state: State | FFSStateRef) -> int: ...
+    def calc_mismatch_locations(self, state: State | FFSStateRef) -> np.ndarray: ...
+    def name_canvas(self, state: State | FFSStateRef) -> np.ndarray: ...
+    def color_canvas(self, state: State | np.ndarray | FFSStateRef) -> np.ndarray: ...
     @property
     def tile_names(self) -> list[str]: ...
     @property
     def tile_colors(self) -> np.ndarray: ...
     def update_all(self, state: State, needed) -> None: ...
     def plot_canvas(
         self,
         state: State,
         ax=None,
         annotate_tiles=False,
         annotate_mismatches=False,
         crop=False,
-    ) -> "plt.Axes": ...
+    ) -> "Axes": ...
     def get_param(self, name: str) -> Any: ...
     def set_param(self, name: str, value: Any): ...
 
 class FissionHandling(object): ...
 class CanvasType(object): ...
 class ChunkSize(object): ...
 class ChunkHandling(object): ...
 class Model(object): ...
 
-class FFSLevel(object):
+class FFSStateRef(object):
+    @property
+    def canvas_view(self) -> np.ndarray: ...
+    def canvas_copy(self) -> np.ndarray: ...
+    @property
+    def n_tiles(self) -> int: ...
+    @property
+    def total_events(self) -> int: ...
+    @property
+    def time(self) -> float: ...
+    def tracking_copy(self) -> np.ndarray: ...
+    def clone_state(self) -> State: ...
+    
+
+class FFSLevelRef(object):
     @property
     def configs(self) -> list[np.ndarray]:
         """List of configurations at this level, as arrays (not full states)."""
         ...
     @property
+    def states(self) -> list[FFSStateRef]:
+        """List of states at this level."""
+        ...
+    @property
     def previous_indices(self) -> list[int]:
         """For each configuration, the index of the configuration in the previous
         level that resulted in it."""
         ...
 
 class FFSResult(object):
     @property
@@ -104,15 +122,15 @@
         """
         ...
     @property
     def forward_vec(self) -> np.ndarray: ...
     @property
     def dimerization_rate(self) -> float: ...
     @property
-    def surfaces(self) -> list[FFSLevel]: ...
+    def surfaces(self) -> list[FFSLevelRef]: ...
     @property
     def previous_indices(self) -> list[list[int]]: ...
     def configs_dataframe(self) -> pl.DataFrame: ...
     def surfaces_dataframe(self) -> pl.DataFrame: ...
 
 class Tile(object):
     def __init__(
```

### Comparing `rgrow-0.13.1/PKG-INFO` & `rgrow-0.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgrow
-Version: 0.13.1
+Version: 0.14.0
 Requires-Dist: numpy ~=1.26
 Requires-Dist: attrs ~=23.2
 Requires-Dist: matplotlib ~=3.8.2
 License-File: LICENSE
 Summary: Python interface to rgrow.
 Author: Constantine Evans <const@costi.net>
 Author-email: Constantine Evans <const@costi.net>
```

