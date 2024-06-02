# Comparing `tmp/starknet_crypto_py-0.1.0.tar.gz` & `tmp/starknet_crypto_py-0.2.0.tar.gz`

## Comparing `starknet_crypto_py-0.1.0.tar` & `starknet_crypto_py-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 starknet_crypto_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3252 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/.gitignore
--rw-r--r--   0     1001      127      569 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      546 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/Makefile
--rw-r--r--   0     1001      127      697 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/README.md
--rw-r--r--   0     1001      127    21520 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/poetry.lock
--rw-r--r--   0     1001      127       19 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/python/starknet_crypto_py/__init__.py
--rw-r--r--   0     1001      127      638 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/python/starknet_crypto_py/lib.py
--rw-r--r--   0     1001      127        0 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/python/starknet_crypto_py/py.typed
--rw-r--r--   0     1001      127      268 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/python/starknet_crypto_py/starknet_crypto_py.pyi
--rw-r--r--   0     1001      127     2347 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/python/tests/test_starknet_crypto.py
--rw-r--r--   0     1001      127     1949 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127      276 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/tox.ini
--rw-r--r--   0     1001      127    19454 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1761 2024-01-17 11:51:33.000000 starknet_crypto_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 starknet_crypto_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 starknet_crypto_py-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     2826 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/.gitignore
+-rw-r--r--   0     1001      127      569 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      535 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/Makefile
+-rw-r--r--   0     1001      127     1201 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/README.md
+-rw-r--r--   0     1001      127    21719 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/poetry.lock
+-rw-r--r--   0     1001      127       19 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/python/starknet_crypto_py/__init__.py
+-rw-r--r--   0     1001      127      644 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/python/starknet_crypto_py/lib.py
+-rw-r--r--   0     1001      127        0 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/python/starknet_crypto_py/py.typed
+-rw-r--r--   0     1001      127      268 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/python/starknet_crypto_py/starknet_crypto_py.pyi
+-rw-r--r--   0     1001      127     1910 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/python/tests/test_starknet_crypto.py
+-rw-r--r--   0     1001      127     2091 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127      276 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/tox.ini
+-rw-r--r--   0     1001      127    19454 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1781 2024-06-02 15:36:33.000000 starknet_crypto_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 starknet_crypto_py-0.2.0/PKG-INFO
```

### Comparing `starknet_crypto_py-0.1.0/Cargo.toml` & `starknet_crypto_py-0.2.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "starknet-crypto-py"
-version = "0.1.0"
+version = "0.2.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "starknet_crypto_py"
 crate-type = ["cdylib"]
```

### Comparing `starknet_crypto_py-0.1.0/.github/workflows/CI.yml` & `starknet_crypto_py-0.2.0/.github/workflows/CI.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
+        target: [x86_64, x86, aarch64, armv7, s390x]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: Build wheels
         uses: PyO3/maturin-action@v1
@@ -103,31 +103,18 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
     needs: [linux, windows, macos, sdist]
-    permissions:
-      # Used to upload release artifacts
-      contents: write
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --non-interactive --skip-existing *
-      - uses: actions/download-artifact@v3
-        with:
-          name: wasm-wheels
-          path: wasm
-      - name: Upload to GitHub Release
-        uses: softprops/action-gh-release@v1
-        with:
-          files: |
-            wasm/*.whl
-          prerelease: ${{ contains(github.ref, 'alpha') || contains(github.ref, 'beta') }}
```

### Comparing `starknet_crypto_py-0.1.0/.gitignore` & `starknet_crypto_py-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `starknet_crypto_py-0.1.0/.pre-commit-config.yaml` & `starknet_crypto_py-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `starknet_crypto_py-0.1.0/Makefile` & `starknet_crypto_py-0.2.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 check:
 	@echo "🩺 Checking..."
 	cargo check
 	poetry check
 
 build:
 	@echo "🔨 Building..."
-	RUSTFLAGS="-C target-cpu=haswell" maturin build -i 3.9 --sdist --release --zig --strip \
-    --target x86_64-unknown-linux-gnu \
-    --compatibility manylinux_2_24
+	RUSTFLAGS="-C target-cpu=haswell" maturin build -i 3.9 --sdist --release --strip \
+    --target x86_64-apple-darwin \
+    --compatibility manylinux_2_28
 
 sdist:
 	@echo "🔨 Building..."
 	maturin sdist
 
 develop:
 	@echo "⛏️ Building..."
```

### Comparing `starknet_crypto_py-0.1.0/poetry.lock` & `starknet_crypto_py-0.2.0/poetry.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "cachetools"
-version = "5.3.2"
+version = "5.3.3"
 description = "Extensible memoizing collections and decorators"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "cachetools-5.3.2-py3-none-any.whl", hash = "sha256:861f35a13a451f94e301ce2bec7cac63e881232ccce7ed67fab9b5df4d3beaa1"},
-    {file = "cachetools-5.3.2.tar.gz", hash = "sha256:086ee420196f7b2ab9ca2db2520aca326318b68fe5ba8bc4d49cca91add450f2"},
+    {file = "cachetools-5.3.3-py3-none-any.whl", hash = "sha256:0abad1021d3f8325b2fc1d2e9c8b9c9d57b04c3932657a72465447332c24d945"},
+    {file = "cachetools-5.3.3.tar.gz", hash = "sha256:ba29e2dfa0b8b556606f097407ed1aa62080ee108ab0dc5ec9d6a723a007d105"},
 ]
 
 [[package]]
 name = "chardet"
 version = "5.2.0"
 description = "Universal encoding detector for Python 3"
 optional = false
@@ -42,40 +42,40 @@
 files = [
     {file = "distlib-0.3.8-py2.py3-none-any.whl", hash = "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784"},
     {file = "distlib-0.3.8.tar.gz", hash = "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 description = "Backport of PEP 654 (exception groups)"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "filelock"
-version = "3.13.1"
+version = "3.14.0"
 description = "A platform independent file lock."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "filelock-3.13.1-py3-none-any.whl", hash = "sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c"},
-    {file = "filelock-3.13.1.tar.gz", hash = "sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e"},
+    {file = "filelock-3.14.0-py3-none-any.whl", hash = "sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f"},
+    {file = "filelock-3.14.0.tar.gz", hash = "sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a"},
 ]
 
 [package.extras]
-docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.24)"]
-testing = ["covdefaults (>=2.3)", "coverage (>=7.3.2)", "diff-cover (>=8)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-timeout (>=2.2)"]
+docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
+testing = ["covdefaults (>=2.3)", "coverage (>=7.3.2)", "diff-cover (>=8.0.1)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-timeout (>=2.2)"]
 typing = ["typing-extensions (>=4.8)"]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 description = "brain-dead simple config-ini parsing"
 optional = false
@@ -83,75 +83,75 @@
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "maturin"
-version = "1.4.0"
+version = "1.5.1"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "maturin-1.4.0-py3-none-linux_armv6l.whl", hash = "sha256:b84bee85620e1b7b662a7af71289f7f6c23df8269e42c0f76882676dfc9c733f"},
-    {file = "maturin-1.4.0-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:076970a73da7fa3648204a584cd347b899c1ea67f8124b212bccd06728e63ed9"},
-    {file = "maturin-1.4.0-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:f8eded83abdb30b2b6ae6d32c80b8192bdd8bcfec0ebfacee6ac02434aa499d6"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:ff95a4494d9e57b6e74d4d7f8a9a2ee8ed29bd7f0e61855656ad959a432c0efc"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:16239a7648ef17976585353e381840c18e650d352576ed9545abca407d65e534"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:77428c043d585f038f4b056c4d617e00a8027b49598ab6d065b8f6b9b9b8d144"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:b4b2f006db1e92687c814576029157dcc2d97b5750fd35fd4f3aabb97e36444f"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.musllinux_1_1_ppc64le.whl", hash = "sha256:ffe4e967080ceb83c156e73a37d3974b30cad01c376a86dc39a76a0c6bccf9b0"},
-    {file = "maturin-1.4.0-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:01473dc30aed8f2cee3572b3e99e3ea75bf09c84b028bf6077f7643a189699c8"},
-    {file = "maturin-1.4.0-py3-none-win32.whl", hash = "sha256:e669ba5984c15e29b8545b295ba6738974180b44f47f5d9e75569a5ce6b8add5"},
-    {file = "maturin-1.4.0-py3-none-win_amd64.whl", hash = "sha256:e2c1b157397ef3721b9c2f3f24d9a5a60bd84322aac13b4dd0704a80448741b0"},
-    {file = "maturin-1.4.0-py3-none-win_arm64.whl", hash = "sha256:2979175a7eee837dc3a6931980b37ddc86b9ced54d600856668fc074ca2530ef"},
-    {file = "maturin-1.4.0.tar.gz", hash = "sha256:ed12e1768094a7adeafc3a74ebdb8dc2201fa64c4e7e31f14cfc70378bf93790"},
+    {file = "maturin-1.5.1-py3-none-linux_armv6l.whl", hash = "sha256:589e9b7024007e130b136ba6f1c2c8393a87e42cf968d12852913ab1e3c69ed3"},
+    {file = "maturin-1.5.1-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:a1abda07093b3c8ef897626166c02ed64e3e446c48460b28efb51833abf89cbb"},
+    {file = "maturin-1.5.1-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:48a1fbbdc2514525f27d6d339ab97b098ede28759f8593d110c89cc07bbe40ed"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:96d96b1fa3a165db9ca539f764d31da8ebc92e31ca3a1dd6ccd50008d222bd96"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:786bf36a98c4e27cbebb1dc8e432c1bcbbb59e7a9719592cbb89e46a0ccd5bcc"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:d821b37da759884ad09cfee4cd9deac10f4132744cc66e4d9190a1972233bc83"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:62133bf690555bbc8cc6b1c18a0c57b0ab2b4d68d3fcd320eb16df941563fe06"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.musllinux_1_1_ppc64le.whl", hash = "sha256:6bff165252b1fcc887679ddf7b71b5cc024327ba96ea893133be38c0ed38f163"},
+    {file = "maturin-1.5.1-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2c42a95466ffc3de0a3940cd20c57cf0c44fe5ea679375d73422afbb00236c64"},
+    {file = "maturin-1.5.1-py3-none-win32.whl", hash = "sha256:d09538b4aa0da4b59fd47cb429003b45bfd5d801714adf1db2511bf8bdea532f"},
+    {file = "maturin-1.5.1-py3-none-win_amd64.whl", hash = "sha256:a3db9054222ac79275e082b21cfd234b8e036714a4ff227a0a28f6a3ffa3744d"},
+    {file = "maturin-1.5.1-py3-none-win_arm64.whl", hash = "sha256:acf528e51413f6ae489473d64116d8c83f140386349004949d29137c16a82193"},
+    {file = "maturin-1.5.1.tar.gz", hash = "sha256:3dd834ece80edb866af18cbd4635e0ecac40139c726428d5f1849ae154b26dca"},
 ]
 
 [package.dependencies]
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "mypy"
-version = "1.8.0"
+version = "1.10.0"
 description = "Optional static typing for Python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "mypy-1.8.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3"},
-    {file = "mypy-1.8.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4"},
-    {file = "mypy-1.8.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d"},
-    {file = "mypy-1.8.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9"},
-    {file = "mypy-1.8.0-cp310-cp310-win_amd64.whl", hash = "sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410"},
-    {file = "mypy-1.8.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae"},
-    {file = "mypy-1.8.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3"},
-    {file = "mypy-1.8.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817"},
-    {file = "mypy-1.8.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d"},
-    {file = "mypy-1.8.0-cp311-cp311-win_amd64.whl", hash = "sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835"},
-    {file = "mypy-1.8.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd"},
-    {file = "mypy-1.8.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55"},
-    {file = "mypy-1.8.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218"},
-    {file = "mypy-1.8.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3"},
-    {file = "mypy-1.8.0-cp312-cp312-win_amd64.whl", hash = "sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e"},
-    {file = "mypy-1.8.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6"},
-    {file = "mypy-1.8.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66"},
-    {file = "mypy-1.8.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6"},
-    {file = "mypy-1.8.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d"},
-    {file = "mypy-1.8.0-cp38-cp38-win_amd64.whl", hash = "sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02"},
-    {file = "mypy-1.8.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8"},
-    {file = "mypy-1.8.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259"},
-    {file = "mypy-1.8.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b"},
-    {file = "mypy-1.8.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592"},
-    {file = "mypy-1.8.0-cp39-cp39-win_amd64.whl", hash = "sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a"},
-    {file = "mypy-1.8.0-py3-none-any.whl", hash = "sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d"},
-    {file = "mypy-1.8.0.tar.gz", hash = "sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99"},
+    {file = "mypy-1.10.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2"},
+    {file = "mypy-1.10.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9"},
+    {file = "mypy-1.10.0-cp310-cp310-win_amd64.whl", hash = "sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee"},
+    {file = "mypy-1.10.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de"},
+    {file = "mypy-1.10.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7"},
+    {file = "mypy-1.10.0-cp311-cp311-win_amd64.whl", hash = "sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30"},
+    {file = "mypy-1.10.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e"},
+    {file = "mypy-1.10.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5"},
+    {file = "mypy-1.10.0-cp312-cp312-win_amd64.whl", hash = "sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727"},
+    {file = "mypy-1.10.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4"},
+    {file = "mypy-1.10.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061"},
+    {file = "mypy-1.10.0-cp38-cp38-win_amd64.whl", hash = "sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec"},
+    {file = "mypy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821"},
+    {file = "mypy-1.10.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746"},
+    {file = "mypy-1.10.0-cp39-cp39-win_amd64.whl", hash = "sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a"},
+    {file = "mypy-1.10.0-py3-none-any.whl", hash = "sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee"},
+    {file = "mypy-1.10.0.tar.gz", hash = "sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131"},
 ]
 
 [package.dependencies]
 mypy-extensions = ">=1.0.0"
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typing-extensions = ">=4.1.0"
 
@@ -170,47 +170,48 @@
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.2"
+version = "24.0"
 description = "Core utilities for Python packages"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-23.2-py3-none-any.whl", hash = "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"},
-    {file = "packaging-23.2.tar.gz", hash = "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5"},
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "4.1.0"
-description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
+version = "4.2.1"
+description = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "platformdirs-4.1.0-py3-none-any.whl", hash = "sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380"},
-    {file = "platformdirs-4.1.0.tar.gz", hash = "sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420"},
+    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
+    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
 ]
 
 [package.extras]
-docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.1)", "sphinx-autodoc-typehints (>=1.24)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.11.1)"]
+docs = ["furo (>=2023.9.10)", "proselint (>=0.13)", "sphinx (>=7.2.6)", "sphinx-autodoc-typehints (>=1.25.2)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.4.3)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)"]
+type = ["mypy (>=1.8)"]
 
 [[package]]
 name = "pluggy"
-version = "1.3.0"
+version = "1.5.0"
 description = "plugin and hook calling mechanisms for python"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "pluggy-1.3.0-py3-none-any.whl", hash = "sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7"},
-    {file = "pluggy-1.3.0.tar.gz", hash = "sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [package.extras]
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
@@ -252,36 +253,36 @@
 tomli = {version = ">=1.0.0", markers = "python_version < \"3.11\""}
 
 [package.extras]
 testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "setuptools", "xmlschema"]
 
 [[package]]
 name = "ruff"
-version = "0.1.13"
+version = "0.1.15"
 description = "An extremely fast Python linter and code formatter, written in Rust."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "ruff-0.1.13-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:e3fd36e0d48aeac672aa850045e784673449ce619afc12823ea7868fcc41d8ba"},
-    {file = "ruff-0.1.13-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:9fb6b3b86450d4ec6a6732f9f60c4406061b6851c4b29f944f8c9d91c3611c7a"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b13ba5d7156daaf3fd08b6b993360a96060500aca7e307d95ecbc5bb47a69296"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:9ebb40442f7b531e136d334ef0851412410061e65d61ca8ce90d894a094feb22"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:226b517f42d59a543d6383cfe03cccf0091e3e0ed1b856c6824be03d2a75d3b6"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:5f0312ba1061e9b8c724e9a702d3c8621e3c6e6c2c9bd862550ab2951ac75c16"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2f59bcf5217c661254bd6bc42d65a6fd1a8b80c48763cb5c2293295babd945dd"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e6894b00495e00c27b6ba61af1fc666f17de6140345e5ef27dd6e08fb987259d"},
-    {file = "ruff-0.1.13-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9a1600942485c6e66119da294c6294856b5c86fd6df591ce293e4a4cc8e72989"},
-    {file = "ruff-0.1.13-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:ee3febce7863e231a467f90e681d3d89210b900d49ce88723ce052c8761be8c7"},
-    {file = "ruff-0.1.13-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:dcaab50e278ff497ee4d1fe69b29ca0a9a47cd954bb17963628fa417933c6eb1"},
-    {file = "ruff-0.1.13-py3-none-musllinux_1_2_i686.whl", hash = "sha256:f57de973de4edef3ad3044d6a50c02ad9fc2dff0d88587f25f1a48e3f72edf5e"},
-    {file = "ruff-0.1.13-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:7a36fa90eb12208272a858475ec43ac811ac37e91ef868759770b71bdabe27b6"},
-    {file = "ruff-0.1.13-py3-none-win32.whl", hash = "sha256:a623349a505ff768dad6bd57087e2461be8db58305ebd5577bd0e98631f9ae69"},
-    {file = "ruff-0.1.13-py3-none-win_amd64.whl", hash = "sha256:f988746e3c3982bea7f824c8fa318ce7f538c4dfefec99cd09c8770bd33e6539"},
-    {file = "ruff-0.1.13-py3-none-win_arm64.whl", hash = "sha256:6bbbc3042075871ec17f28864808540a26f0f79a4478c357d3e3d2284e832998"},
-    {file = "ruff-0.1.13.tar.gz", hash = "sha256:e261f1baed6291f434ffb1d5c6bd8051d1c2a26958072d38dfbec39b3dda7352"},
+    {file = "ruff-0.1.15-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:5fe8d54df166ecc24106db7dd6a68d44852d14eb0729ea4672bb4d96c320b7df"},
+    {file = "ruff-0.1.15-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:6f0bfbb53c4b4de117ac4d6ddfd33aa5fc31beeaa21d23c45c6dd249faf9126f"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e0d432aec35bfc0d800d4f70eba26e23a352386be3a6cf157083d18f6f5881c8"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:9405fa9ac0e97f35aaddf185a1be194a589424b8713e3b97b762336ec79ff807"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c66ec24fe36841636e814b8f90f572a8c0cb0e54d8b5c2d0e300d28a0d7bffec"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:6f8ad828f01e8dd32cc58bc28375150171d198491fc901f6f98d2a39ba8e3ff5"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:86811954eec63e9ea162af0ffa9f8d09088bab51b7438e8b6488b9401863c25e"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:fd4025ac5e87d9b80e1f300207eb2fd099ff8200fa2320d7dc066a3f4622dc6b"},
+    {file = "ruff-0.1.15-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b17b93c02cdb6aeb696effecea1095ac93f3884a49a554a9afa76bb125c114c1"},
+    {file = "ruff-0.1.15-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:ddb87643be40f034e97e97f5bc2ef7ce39de20e34608f3f829db727a93fb82c5"},
+    {file = "ruff-0.1.15-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:abf4822129ed3a5ce54383d5f0e964e7fef74a41e48eb1dfad404151efc130a2"},
+    {file = "ruff-0.1.15-py3-none-musllinux_1_2_i686.whl", hash = "sha256:6c629cf64bacfd136c07c78ac10a54578ec9d1bd2a9d395efbee0935868bf852"},
+    {file = "ruff-0.1.15-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:1bab866aafb53da39c2cadfb8e1c4550ac5340bb40300083eb8967ba25481447"},
+    {file = "ruff-0.1.15-py3-none-win32.whl", hash = "sha256:2417e1cb6e2068389b07e6fa74c306b2810fe3ee3476d5b8a96616633f40d14f"},
+    {file = "ruff-0.1.15-py3-none-win_amd64.whl", hash = "sha256:3837ac73d869efc4182d9036b1405ef4c73d9b1f88da2413875e34e0d6919587"},
+    {file = "ruff-0.1.15-py3-none-win_arm64.whl", hash = "sha256:9a933dfb1c14ec7a33cceb1e49ec4a16b51ce3c20fd42663198746efc0427360"},
+    {file = "ruff-0.1.15.tar.gz", hash = "sha256:f6dfa8c1b21c913c326919056c390966648b680966febcb796cc9d1aaab8564e"},
 ]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
 optional = false
@@ -289,21 +290,21 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tox"
-version = "4.12.0"
+version = "4.15.0"
 description = "tox is a generic virtualenv management and test command line tool"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "tox-4.12.0-py3-none-any.whl", hash = "sha256:c94bf5852ba41f3d9f1e3470ccf3390e0b7bdc938095be3cd96dce25ab5062a0"},
-    {file = "tox-4.12.0.tar.gz", hash = "sha256:76adc53a3baff7bde80d6ad7f63235735cfc5bc42e8cb6fccfbf62cb5ffd4d92"},
+    {file = "tox-4.15.0-py3-none-any.whl", hash = "sha256:300055f335d855b2ab1b12c5802de7f62a36d4fd53f30bd2835f6a201dda46ea"},
+    {file = "tox-4.15.0.tar.gz", hash = "sha256:7a0beeef166fbe566f54f795b4906c31b428eddafc0102ac00d20998dd1933f6"},
 ]
 
 [package.dependencies]
 cachetools = ">=5.3.2"
 chardet = ">=5.2"
 colorama = ">=0.4.6"
 filelock = ">=3.13.1"
@@ -316,56 +317,57 @@
 
 [package.extras]
 docs = ["furo (>=2023.9.10)", "sphinx (>=7.2.6)", "sphinx-argparse-cli (>=1.11.1)", "sphinx-autodoc-typehints (>=1.25.2)", "sphinx-copybutton (>=0.5.2)", "sphinx-inline-tabs (>=2023.4.21)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.11)"]
 testing = ["build[virtualenv] (>=1.0.3)", "covdefaults (>=2.3)", "detect-test-pollution (>=1.2)", "devpi-process (>=1)", "diff-cover (>=8.0.2)", "distlib (>=0.3.8)", "flaky (>=3.7)", "hatch-vcs (>=0.4)", "hatchling (>=1.21)", "psutil (>=5.9.7)", "pytest (>=7.4.4)", "pytest-cov (>=4.1)", "pytest-mock (>=3.12)", "pytest-xdist (>=3.5)", "re-assert (>=1.1)", "time-machine (>=2.13)", "wheel (>=0.42)"]
 
 [[package]]
 name = "typing-extensions"
-version = "4.9.0"
+version = "4.11.0"
 description = "Backported and Experimental Type Hints for Python 3.8+"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "typing_extensions-4.9.0-py3-none-any.whl", hash = "sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd"},
-    {file = "typing_extensions-4.9.0.tar.gz", hash = "sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.25.0"
+version = "20.26.1"
 description = "Virtual Python Environment builder"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "virtualenv-20.25.0-py3-none-any.whl", hash = "sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3"},
-    {file = "virtualenv-20.25.0.tar.gz", hash = "sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b"},
+    {file = "virtualenv-20.26.1-py3-none-any.whl", hash = "sha256:7aa9982a728ae5892558bff6a2839c00b9ed145523ece2274fad6f414690ae75"},
+    {file = "virtualenv-20.26.1.tar.gz", hash = "sha256:604bfdceaeece392802e6ae48e69cec49168b9c5f4a44e483963f9242eb0e78b"},
 ]
 
 [package.dependencies]
 distlib = ">=0.3.7,<1"
 filelock = ">=3.12.2,<4"
 platformdirs = ">=3.9.1,<5"
 
 [package.extras]
-docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.2)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
+docs = ["furo (>=2023.7.26)", "proselint (>=0.13)", "sphinx (>=7.1.2,!=7.3)", "sphinx-argparse (>=0.4)", "sphinxcontrib-towncrier (>=0.2.1a0)", "towncrier (>=23.6)"]
 test = ["covdefaults (>=2.3)", "coverage (>=7.2.7)", "coverage-enable-subprocess (>=1)", "flaky (>=3.7)", "packaging (>=23.1)", "pytest (>=7.4)", "pytest-env (>=0.8.2)", "pytest-freezer (>=0.4.8)", "pytest-mock (>=3.11.1)", "pytest-randomly (>=3.12)", "pytest-timeout (>=2.1)", "setuptools (>=68)", "time-machine (>=2.10)"]
 
 [[package]]
 name = "ziglang"
-version = "0.11.0"
+version = "0.12.0"
 description = "Zig is a general-purpose programming language and toolchain for maintaining robust, optimal, and reusable software."
 optional = false
 python-versions = "~=3.5"
 files = [
-    {file = "ziglang-0.11.0-py3-none-macosx_10_9_x86_64.whl", hash = "sha256:bd046eeab97ad51048575768f6dae10468b3a4449f4467ed61dae621faf6ee55"},
-    {file = "ziglang-0.11.0-py3-none-macosx_11_0_arm64.whl", hash = "sha256:038b95cac9adef0c6dce9b72bdad895a0e4e0654c77c4a8f84fe79d2909a366e"},
-    {file = "ziglang-0.11.0-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:4f848c8cca520cb12357cfa3d303bf1149a30566f4c1e5999284dbdf921cc2b8"},
-    {file = "ziglang-0.11.0-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:45e8116428267e20529b9ee43a7e7364791c1a092845d2143b248a1dbf6760b0"},
-    {file = "ziglang-0.11.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:d6372bada34714a5395539cc4d76e9cc6062739cee5ce9949a250f7c525ceb94"},
-    {file = "ziglang-0.11.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:5fe81f91fd872fc32ed0f82807df6c680a82cbea56a9f24f818e9da299049022"},
-    {file = "ziglang-0.11.0-py3-none-win_amd64.whl", hash = "sha256:a7edc7020e7ffbbb3af3a40c17a9bda65d5a65132ff933e153ffa80d8f5ad731"},
+    {file = "ziglang-0.12.0-py3-none-macosx_10_9_x86_64.whl", hash = "sha256:c6d1053f0e1d486cdf374f33b7ed00d99040d03f45eed5122a7522b0b7a75946"},
+    {file = "ziglang-0.12.0-py3-none-macosx_11_0_arm64.whl", hash = "sha256:1f9291fd98c4e1ece04285ddf019b9999b2e81fb4f785b550b6d91b1e1699bc9"},
+    {file = "ziglang-0.12.0-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:1cb9e6938ec8cddba124ebf2dcaf950e19b5b807eaa18cb976c569e6edef5ae3"},
+    {file = "ziglang-0.12.0-py3-none-manylinux_2_12_x86_64.manylinux2010_x86_64.musllinux_1_1_x86_64.whl", hash = "sha256:0c777f1d5d9be32d0edffc79956d03ed35f868a8db7b0552da0984182aa10ff0"},
+    {file = "ziglang-0.12.0-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.musllinux_1_1_aarch64.whl", hash = "sha256:8da631bfb5e49390f0551a4412111c8a14671fd7f151e1adcc420317b02efcf6"},
+    {file = "ziglang-0.12.0-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.musllinux_1_1_armv7l.whl", hash = "sha256:ccec405a443016647c47edcd48faf15be9d3add21c2c13bc77217b8fe87a1508"},
+    {file = "ziglang-0.12.0-py3-none-win32.whl", hash = "sha256:9373c68cf654d69f46411eff2fd48cb8495b8d9bcd6e88b65783ef8ab4bfe4ae"},
+    {file = "ziglang-0.12.0-py3-none-win_amd64.whl", hash = "sha256:044136e276e80dfdc7cfaada80efe8679d0ba9f8abf911f8c68afa44ca259148"},
 ]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.9"
-content-hash = "e3c0fd16810f9c1c687bb2bd1d73d9b2d6abb0ac4f1e38b57405833a9cc6d380"
+content-hash = "8f2b831d510d23f81d4653fa10b5f4f12760af39658298843b7abc2a727af281"
```

### Comparing `starknet_crypto_py-0.1.0/python/tests/test_starknet_crypto.py` & `starknet_crypto_py-0.2.0/python/tests/test_starknet_crypto.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,27 +49,11 @@
         ),
     ],
 )
 def test_pedersen_hash(first: int, second: int, msg_hash: int) -> None:
     assert pedersen_hash(first, second) == msg_hash
 
 
-def test_sign() -> None:
-    (r, s) = sign(private_key=TEST_PRIVATE_KEY, msg_hash=4660, k=32)
-    assert (
-        r
-        == 1977703130303461992863803129734853218488251484396280000763960303272760326570
-    )
-    assert (
-        s
-        == 2724513698511531566681485513041952149126560643963807389721140128271700252419
-    )
-
-
-def test_verify() -> None:
-    is_valid = verify(
-        public_key=TEST_PUBLIC_KEY,
-        msg_hash=4660,
-        r=1977703130303461992863803129734853218488251484396280000763960303272760326570,
-        s=2724513698511531566681485513041952149126560643963807389721140128271700252419,
-    )
+def test_sign_and_verify() -> None:
+    (r, s) = sign(private_key=TEST_PRIVATE_KEY, msg_hash=4660, seed=123)
+    is_valid = verify(public_key=TEST_PUBLIC_KEY, msg_hash=4660, r=r, s=s)
     assert is_valid
```

### Comparing `starknet_crypto_py-0.1.0/src/lib.rs` & `starknet_crypto_py-0.2.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use pyo3::prelude::*;
 use starknet_crypto::{
     FieldElement,
     pedersen_hash as pedersen_hash_rs,
     sign as sign_rs,
+    rfc6979_generate_k as rfc6979_generate_k_rs,
 };
 
 fn _fe_from_str(s: &str) -> FieldElement {
     FieldElement::from_hex_be(s).unwrap()
 }
 
 #[pyfunction]
@@ -21,18 +22,19 @@
     let left: FieldElement = _fe_from_str(left);
     let right: FieldElement = _fe_from_str(right);
     let hash: String = pedersen_hash_rs(&left, &right).to_string();
     Ok(hash)
 }
 
 #[pyfunction]
-fn rs_sign(priv_key: &str, msg_hash: &str, k: &str) -> PyResult<(String, String)> {
+fn rs_sign(priv_key: &str, msg_hash: &str, seed: &str) -> PyResult<(String, String)> {
     let msg_hash: FieldElement = _fe_from_str(msg_hash);
     let priv_key: FieldElement = _fe_from_str(priv_key);
-    let k: FieldElement = _fe_from_str(k);
+    let seed: FieldElement = _fe_from_str(seed);
+    let k: FieldElement = rfc6979_generate_k_rs(&msg_hash, &priv_key, Some(&seed));
     let hash: starknet_crypto::ExtendedSignature = sign_rs(&priv_key, &msg_hash, &k).unwrap();
     let r: String = hash.r.to_string();
     let s: String = hash.s.to_string();
     Ok((r, s))
 }
 
 #[pyfunction]
```

### Comparing `starknet_crypto_py-0.1.0/Cargo.lock` & `starknet_crypto_py-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -527,15 +527,15 @@
  "starknet-curve",
  "starknet-ff",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "starknet-crypto-py"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "cc",
  "pyo3",
  "pyo3-build-config",
  "starknet-crypto",
 ]
```

### Comparing `starknet_crypto_py-0.1.0/pyproject.toml` & `starknet_crypto_py-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 
 [tool.maturin]
 python-source = "python"
 features = ["pyo3/extension-module"]
 
 [tool.poetry]
 name = "starknet-crypto-py"
-version = "0.1.0"
+version = "0.2.0"
 description = "starknet-crypto python module"
 authors = ["Paradex"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+ziglang = "^0.12.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
-maturin = "^1.4.0"
+maturin = "^1.5.1"
 mypy = "^1.8.0"
 ruff = "^0.1.13"
-ziglang = "^0.11.0"
+ziglang = "^0.12.0"
 tox = "^4.12.0"
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
```

