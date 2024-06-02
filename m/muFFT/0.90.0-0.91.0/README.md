# Comparing `tmp/mufft-0.90.0.tar.gz` & `tmp/mufft-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mufft-0.90.0.tar", last modified: Thu May 23 06:34:41 2024, max compression
+gzip compressed data, was "mufft-0.91.0.tar", last modified: Sun Jun  2 21:36:22 2024, max compression
```

## Comparing `mufft-0.90.0.tar` & `mufft-0.91.0.tar`

### file list

```diff
@@ -1,100 +1,88 @@
--rw-r--r--   0        0        0      195 2024-05-23 06:28:29.000000 mufft-0.90.0/.clang-format
--rw-r--r--   0        0        0      148 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitattributes
--rw-r--r--   0        0        0      224 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/.install_netcdf.sh
--rw-r--r--   0        0        0      666 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/install_netcdf4.sh
--rw-r--r--   0        0        0     1091 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2563 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/ubuntu.yml
--rw-r--r--   0        0        0     2171 2024-05-23 06:28:29.000000 mufft-0.90.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       93 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitignore
--rw-r--r--   0        0        0      324 2024-05-23 06:28:29.000000 mufft-0.90.0/.gitmodules
--rw-r--r--   0        0        0     7056 2024-05-23 06:28:29.000000 mufft-0.90.0/CHANGELOG.md
--rw-r--r--   0        0        0      210 2024-05-23 06:28:29.000000 mufft-0.90.0/CPPLINT.cfg
--rw-r--r--   0        0        0    35149 2024-05-23 06:28:29.000000 mufft-0.90.0/LICENSE
--rw-r--r--   0        0        0     2526 2024-05-23 06:28:29.000000 mufft-0.90.0/README.md
--rw-r--r--   0        0        0     5765 2024-05-23 06:28:29.000000 mufft-0.90.0/discover_version.py
--rw-r--r--   0        0        0     2548 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/CMakeLists.txt
--rw-r--r--   0        0        0    94508 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/MainSchema.png
--rw-r--r--   0        0        0      608 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/Makefile
--rw-r--r--   0        0        0    58298 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/logo_flat.png
--rw-r--r--   0        0        0    37122 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/logo_square.png
--rw-r--r--   0        0        0       86 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/requirements.txt
--rw-r--r--   0        0        0     3962 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/CellSplit.rst
--rw-r--r--   0        0        0   175727 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/CodingConvention.rst
--rw-r--r--   0        0        0     4357 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/ConstitutiveLaws.rst
--rw-r--r--   0        0        0      858 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Doxyfile
--rw-r--r--   0        0        0     5836 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/GettingStarted.rst
--rw-r--r--   0        0        0    41053 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/License.rst
--rw-r--r--   0        0        0     5181 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/MaterialLaminate.rst
--rw-r--r--   0        0        0     2515 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/MaterialLinearElasticGeneric.rst
--rw-r--r--   0        0        0    10554 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/NewMaterial.rst
--rw-r--r--   0        0        0     1011 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/OrganisationOfCode.rst
--rw-r--r--   0        0        0       78 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Reference.rst
--rw-r--r--   0        0        0     3871 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Summary.rst
--rw-r--r--   0        0        0      154 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/Tutorials.rst
--rw-r--r--   0        0        0     6793 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/conf.py
--rw-r--r--   0        0        0     1126 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/index.rst
--rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/input_def
--rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/input_def.in
--rw-r--r--   0        0        0     1934 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/macosx14_bash_profile
--rw-r--r--   0        0        0    19363 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/muGrid.rst
--rw-r--r--   0        0        0       30 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/xml_output_def
--rw-r--r--   0        0        0       50 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/dev-docs/source/xml_output_def.in
--rw-r--r--   0        0        0     3327 2024-05-23 06:28:29.000000 mufft-0.90.0/doc/summary.rmk
--rw-r--r--   0        0        0       16 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/meson.build
--rw-r--r--   0        0        0     4849 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_common_mufft.cc
--rw-r--r--   0        0        0     1710 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_declarations.hh
--rw-r--r--   0        0        0     9806 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_derivatives.cc
--rw-r--r--   0        0        0    22658 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_fftengine.cc
--rw-r--r--   0        0        0     1519 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_module.cc
--rw-r--r--   0        0        0     1357 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/bind_py_version.cc.skeleton
--rw-r--r--   0        0        0      389 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/meson.build
--rw-r--r--   0        0        0    17601 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/NetCDF.py
--rw-r--r--   0        0        0     1746 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils1D.py
--rw-r--r--   0        0        0     4275 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils2D.py
--rw-r--r--   0        0        0    11152 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/Stencils3D.py
--rw-r--r--   0        0        0     6841 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/__init__.py
--rw-r--r--   0        0        0      230 2024-05-23 06:28:29.000000 mufft-0.90.0/language_bindings/python/muFFT/meson.build
--rw-r--r--   0        0        0     2845 2024-05-23 06:28:29.000000 mufft-0.90.0/meson.build
--rw-r--r--   0        0        0     1909 2024-05-23 06:28:29.000000 mufft-0.90.0/pyproject.toml
--rw-r--r--   0        0        0      114 2024-05-23 06:28:29.000000 mufft-0.90.0/renovate.json
--rw-r--r--   0        0        0     7182 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/derivative.cc
--rw-r--r--   0        0        0    13170 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/derivative.hh
--rw-r--r--   0        0        0    38967 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_engine_base.cc
--rw-r--r--   0        0        0    17691 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_engine_base.hh
--rw-r--r--   0        0        0     1997 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_utils.cc
--rw-r--r--   0        0        0     7278 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fft_utils.hh
--rw-r--r--   0        0        0     9608 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftw_engine.cc
--rw-r--r--   0        0        0     5130 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftw_engine.hh
--rw-r--r--   0        0        0    15704 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftwmpi_engine.cc
--rw-r--r--   0        0        0     5950 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/fftwmpi_engine.hh
--rw-r--r--   0        0        0      601 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/meson.build
--rw-r--r--   0        0        0     3138 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/mufft_common.hh
--rw-r--r--   0        0        0    14560 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pfft_engine.cc
--rw-r--r--   0        0        0     5595 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pfft_engine.hh
--rw-r--r--   0        0        0    14089 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pocketfft_engine.cc
--rw-r--r--   0        0        0     4559 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/pocketfft_engine.hh
--rw-r--r--   0        0        0     2631 2024-05-23 06:28:29.000000 mufft-0.90.0/src/libmufft/version.cc
--rw-r--r--   0        0        0      163 2024-05-23 06:28:29.000000 mufft-0.90.0/src/meson.build
--rw-r--r--   0        0        0      590 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/eigen.wrap
--rw-r--r--   0        0        0      139 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/mugrid.wrap
--rw-r--r--   0        0        0     1498 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/LICENSE.md
--rw-r--r--   0        0        0      265 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/POCKETFFT.md
--rw-r--r--   0        0        0    10843 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/README.md
--rw-r--r--   0        0        0      116 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/meson.build
--rw-r--r--   0        0        0   110573 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pocketfft/pocketfft_hdronly.h
--rw-r--r--   0        0        0      616 2024-05-23 06:28:29.000000 mufft-0.90.0/subprojects/pybind11.wrap
--rw-r--r--   0        0        0     1564 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/main_test_suite.cc
--rw-r--r--   0        0        0     2404 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/meson.build
--rw-r--r--   0        0        0     2329 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_context.hh
--rw-r--r--   0        0        0     1633 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_main_test_suite.cc
--rw-r--r--   0        0        0     8189 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/mpi_test_fft_engine.cc
--rw-r--r--   0        0        0     1657 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_binding_tests.py
--rw-r--r--   0        0        0    47442 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_derivative_tests.py
--rw-r--r--   0        0        0    36055 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_fft_tests.py
--rw-r--r--   0        0        0     1482 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_mpi_binding_tests.py
--rw-r--r--   0        0        0     5682 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_muFFT_license_test.py
--rw-r--r--   0        0        0     7223 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/python_netcdf_tests.py
--rw-r--r--   0        0        0     3653 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/test_fft_utils.cc
--rw-r--r--   0        0        0     7651 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/test_serial_fft_engines.cc
--rw-r--r--   0        0        0     1880 2024-05-23 06:28:29.000000 mufft-0.90.0/tests/tests.hh
--rw-r--r--   0        0        0    43893 2024-05-23 06:34:41.621605 mufft-0.90.0/PKG-INFO
+-rw-r--r--   0        0        0      195 2024-06-02 21:30:29.000000 mufft-0.91.0/.clang-format
+-rw-r--r--   0        0        0      148 2024-06-02 21:30:29.000000 mufft-0.91.0/.gitattributes
+-rw-r--r--   0        0        0      666 2024-06-02 21:30:29.000000 mufft-0.91.0/.github/install_netcdf4.sh
+-rw-r--r--   0        0        0     1551 2024-06-02 21:30:29.000000 mufft-0.91.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1091 2024-06-02 21:30:29.000000 mufft-0.91.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3113 2024-06-02 21:30:29.000000 mufft-0.91.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2171 2024-06-02 21:30:29.000000 mufft-0.91.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       93 2024-06-02 21:30:29.000000 mufft-0.91.0/.gitignore
+-rw-r--r--   0        0        0      324 2024-06-02 21:30:29.000000 mufft-0.91.0/.gitmodules
+-rw-r--r--   0        0        0     7457 2024-06-02 21:30:29.000000 mufft-0.91.0/CHANGELOG.md
+-rw-r--r--   0        0        0      210 2024-06-02 21:30:29.000000 mufft-0.91.0/CPPLINT.cfg
+-rw-r--r--   0        0        0    35149 2024-06-02 21:30:29.000000 mufft-0.91.0/LICENSE
+-rw-r--r--   0        0        0     1496 2024-06-02 21:30:29.000000 mufft-0.91.0/README.md
+-rw-r--r--   0        0        0     5765 2024-06-02 21:30:29.000000 mufft-0.91.0/discover_version.py
+-rw-r--r--   0        0        0      725 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/Doxyfile
+-rw-r--r--   0        0        0    94508 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/MainSchema.png
+-rw-r--r--   0        0        0      608 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/Makefile
+-rw-r--r--   0        0        0    58298 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/logo_flat.png
+-rw-r--r--   0        0        0    37122 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/logo_square.png
+-rw-r--r--   0        0        0       34 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/requirements.txt
+-rw-r--r--   0        0        0   175699 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/CodingConvention.rst
+-rw-r--r--   0        0        0       55 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/CplusplusAPI.rst
+-rw-r--r--   0        0        0     3304 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/GettingStarted.rst
+-rw-r--r--   0        0        0     5024 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/Python.rst
+-rw-r--r--   0        0        0     1019 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/Summary.rst
+-rw-r--r--   0        0        0     6568 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/conf.py
+-rw-r--r--   0        0        0     1069 2024-06-02 21:30:29.000000 mufft-0.91.0/doc/source/index.rst
+-rw-r--r--   0        0        0      611 2024-06-02 21:30:29.000000 mufft-0.91.0/examples/convenience_interface.py
+-rw-r--r--   0        0        0     1176 2024-06-02 21:30:29.000000 mufft-0.91.0/examples/gradient.py
+-rw-r--r--   0        0        0      819 2024-06-02 21:30:29.000000 mufft-0.91.0/examples/meson.build
+-rw-r--r--   0        0        0      645 2024-06-02 21:30:29.000000 mufft-0.91.0/examples/transform.py
+-rwxr-xr-x   0        0        0     1357 2024-06-02 21:30:29.000000 mufft-0.91.0/install.sh
+-rw-r--r--   0        0        0       16 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/meson.build
+-rw-r--r--   0        0        0     4849 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/bind_py_common_mufft.cc
+-rw-r--r--   0        0        0     1710 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/bind_py_declarations.hh
+-rw-r--r--   0        0        0     9806 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/bind_py_derivatives.cc
+-rw-r--r--   0        0        0    22513 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/bind_py_fftengine.cc
+-rw-r--r--   0        0        0     1519 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/bind_py_module.cc
+-rw-r--r--   0        0        0      389 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/meson.build
+-rw-r--r--   0        0        0     1746 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/muFFT/Stencils1D.py
+-rw-r--r--   0        0        0     4275 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/muFFT/Stencils2D.py
+-rw-r--r--   0        0        0    11152 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/muFFT/Stencils3D.py
+-rw-r--r--   0        0        0     6896 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/muFFT/__init__.py
+-rw-r--r--   0        0        0      213 2024-06-02 21:30:29.000000 mufft-0.91.0/language_bindings/python/muFFT/meson.build
+-rw-r--r--   0        0        0     2876 2024-06-02 21:30:29.000000 mufft-0.91.0/meson.build
+-rw-r--r--   0        0        0     1900 2024-06-02 21:30:29.000000 mufft-0.91.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-06-02 21:30:29.000000 mufft-0.91.0/renovate.json
+-rw-r--r--   0        0        0     7182 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/derivative.cc
+-rw-r--r--   0        0        0    19745 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/derivative.hh
+-rw-r--r--   0        0        0    38562 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fft_engine_base.cc
+-rw-r--r--   0        0        0    18362 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fft_engine_base.hh
+-rw-r--r--   0        0        0     1997 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fft_utils.cc
+-rw-r--r--   0        0        0    13235 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fft_utils.hh
+-rw-r--r--   0        0        0     9608 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fftw_engine.cc
+-rw-r--r--   0        0        0     6281 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fftw_engine.hh
+-rw-r--r--   0        0        0    15704 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fftwmpi_engine.cc
+-rw-r--r--   0        0        0     6579 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/fftwmpi_engine.hh
+-rw-r--r--   0        0        0      648 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/meson.build
+-rw-r--r--   0        0        0     4757 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/mufft_common.hh
+-rw-r--r--   0        0        0    14560 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/pfft_engine.cc
+-rw-r--r--   0        0        0     5595 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/pfft_engine.hh
+-rw-r--r--   0        0        0    13643 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/pocketfft_engine.cc
+-rw-r--r--   0        0        0     5665 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/pocketfft_engine.hh
+-rw-r--r--   0        0        0     2631 2024-06-02 21:30:29.000000 mufft-0.91.0/src/libmufft/version.cc
+-rw-r--r--   0        0        0      163 2024-06-02 21:30:29.000000 mufft-0.91.0/src/meson.build
+-rw-r--r--   0        0        0      590 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/eigen.wrap
+-rw-r--r--   0        0        0      141 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/mugrid.wrap
+-rw-r--r--   0        0        0     1498 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pocketfft/LICENSE.md
+-rw-r--r--   0        0        0      265 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pocketfft/POCKETFFT.md
+-rw-r--r--   0        0        0    10843 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pocketfft/README.md
+-rw-r--r--   0        0        0      116 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pocketfft/meson.build
+-rw-r--r--   0        0        0   112746 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pocketfft/pocketfft_hdronly.h
+-rw-r--r--   0        0        0      616 2024-06-02 21:30:29.000000 mufft-0.91.0/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0     1564 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/main_test_suite.cc
+-rw-r--r--   0        0        0     2404 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/meson.build
+-rw-r--r--   0        0        0     2329 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/mpi_context.hh
+-rw-r--r--   0        0        0     1633 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/mpi_main_test_suite.cc
+-rw-r--r--   0        0        0     8189 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/mpi_test_fft_engine.cc
+-rw-r--r--   0        0        0     1657 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_binding_tests.py
+-rw-r--r--   0        0        0    47442 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_derivative_tests.py
+-rw-r--r--   0        0        0    36299 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_fft_tests.py
+-rw-r--r--   0        0        0     1482 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_mpi_binding_tests.py
+-rw-r--r--   0        0        0     5682 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_muFFT_license_test.py
+-rw-r--r--   0        0        0     7226 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/python_netcdf_tests.py
+-rw-r--r--   0        0        0     3653 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/test_fft_utils.cc
+-rw-r--r--   0        0        0     7651 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/test_serial_fft_engines.cc
+-rw-r--r--   0        0        0     1880 2024-06-02 21:30:29.000000 mufft-0.91.0/tests/tests.hh
+-rw-r--r--   0        0        0    42861 2024-06-02 21:36:22.359075 mufft-0.91.0/PKG-INFO
```

### Comparing `mufft-0.90.0/.github/install_netcdf4.sh` & `mufft-0.91.0/.github/install_netcdf4.sh`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/.github/workflows/publish.yml` & `mufft-0.91.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/.github/workflows/ubuntu.yml` & `mufft-0.91.0/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test code functionality
+name: Tests
 
 on:
   push:
     branches:
       - '**'
     tags:
       - '**'
@@ -12,14 +12,18 @@
   schedule:
     - cron: "0 2 * * 5"  
 jobs:
   tests:
     runs-on: ubuntu-22.04
     timeout-minutes: 45
 
+    env:
+      WORKDIR: ${{ github.workspace }}/workdir
+      PREFIX: ${{ github.workspace }}/install
+
     strategy:
       matrix:
         mpi: ['no', 'yes']
         compiler: ['gcc', 'clang']
         python-version: ['3.8', '3.9', '3.10', '3.11' , '3.12']
         numpy-version: ['<2.0.0']
         mpi4py-version: ['==3.1.6']
@@ -53,15 +57,23 @@
             sudo apt-get install -y \
               ninja-build \
               libboost-test-dev \
               openmpi-bin \
               libopenmpi-dev \
               libpnetcdf-dev \
               libfftw3-dev \
-              libfftw3-mpi-dev
+              libfftw3-mpi-dev \
+              autoconf automake libtool
+            # Install pfft
+            git clone https://github.com/mpip/pfft.git ${WORKDIR}/pfft
+            cd ${WORKDIR}/pfft
+            ./bootstrap.sh
+            CFLAGS="-O3" ./configure --disable-shared --enable-static --with-pic --disable-fortran --prefix=${PREFIX}
+            make -j 4
+            make install
             # Install mpi4py
             echo "Installing mpi4py${{ matrix.mpi4py-version }}"
             CC=mpicc python3 -m pip install -v \
               --no-binary mpi4py \
               "mpi4py${{ matrix.mpi4py-version }}"
           else
             sudo apt-get install -y \
@@ -76,14 +88,16 @@
       - name: Compile with Meson
         run: |
           if [ "${{ matrix.compiler }}" == "clang" ]; then
             export CC=clang
             export CXX=clang++
           fi
           source venv/bin/activate
+          LD_LIBRARY_PATH=${PREFIX}/lib:${LD_LIBRARY_PATH}
+          CPATH=${PREFIX}/include:${CPATH}
           meson setup builddir
           cd builddir
           meson compile
 
       - name: Run tests
         run: |
           source venv/bin/activate
```

### Comparing `mufft-0.90.0/.github/workflows/wheels.yml` & `mufft-0.91.0/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/CHANGELOG.md` & `mufft-0.91.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 Change log for µFFT
 ===================
 
-0.90.0 (not yet released)
--------------------------
+0.91.0 (02June2024)
+-------------------
+
+- ENH: Convenience filed accessor function `real_space_field` and
+  `fourier_space_field`, etc. that create fields if they don't exist but
+  return them if they do
+- ENH: Added `coords` convenience property which returns domain local
+  fractional real space coordinates (like `fftfreq` for the Fourier space)G
+- DOC: Documentation of Python bindings
+- DOC: Python examples
+
+0.90.0 (23May2024)
+------------------
 
 - Split code into three repositories: muGrid, muFFT and
 
 0.27.0 (30Jan2024)
 ------------------
 
 - muSpectre: Sensitivity analysis for 3D problems
```

### Comparing `mufft-0.90.0/LICENSE` & `mufft-0.91.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/discover_version.py` & `mufft-0.91.0/discover_version.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/doc/dev-docs/MainSchema.png` & `mufft-0.91.0/doc/MainSchema.png`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/doc/dev-docs/Makefile` & `mufft-0.91.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/doc/dev-docs/logo_flat.png` & `mufft-0.91.0/doc/logo_flat.png`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/doc/dev-docs/logo_square.png` & `mufft-0.91.0/doc/logo_square.png`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/doc/dev-docs/source/CodingConvention.rst` & `mufft-0.91.0/doc/source/CodingConvention.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-
 Coding Convention
 ~~~~~~~~~~~~~~~~~
 
-.. contents::
-   :local:
-
-
 Objectives of the Convention
 ****************************
 *µ*\Spectre is a collaborative project and these coding conventions aim to make reading and understanding its code as pain-free as possible, while ensuring the four main requirements of the library
  #. Versatility
  #. Efficiency
  #. Reliability
  #. Ease-of-use
```

### Comparing `mufft-0.90.0/doc/dev-docs/source/Doxyfile` & `mufft-0.91.0/doc/Doxyfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-\PROJECT_NAME           = muSpectre
+PROJECT_NAME           = libmufft
 ## this is for read the docs, which builds in-place
-INPUT                  = ../../../src
+INPUT                  = ../src
 ## this overwrites the INPUT path for local builds
-@INCLUDE               = input_def
 RECURSIVE              = YES
 
 EXTRACT_ALL            = No
 
 SOURCE_BROWSER         = YES
 
 GENERATE_HTML          = YES
 GENERATE_LATEX         = NO
 GENERATE_XML           = YES
 ## this is for read the docs, which builds in-place
-XML_OUTPUT             = doxygenxml
+XML_OUTPUT             = xml
 ## this overwrites the XML_OUTPUT path for local builds
-@INCLUDE               =  xml_output_def
 XML_PROGRAMLISTING     = YES
 
 ALIASES                = "rst=\verbatim embed:rst"
 ALIASES               += "endrst=\endverbatim"
 
 QUIET                  = YES
 WARNINGS               = YES
 WARN_IF_UNDOCUMENTED   = YES
 SHOW_NAMESPACES        = NO
-
-EXCLUDE_PATTERNS       = */CMakeLists.txt
```

### Comparing `mufft-0.90.0/doc/dev-docs/source/License.rst` & `mufft-0.91.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,400 +1,734 @@
-License
--------
-
-*µ*\Spectre is free software; you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3, or (at your option) any later version.
-
-*µ*\Spectre is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-
-You are **not** allowed to use *µ*\Spectre in commercial products.
-
-GNU LESSER GENERAL PUBLIC LICENSE
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Version 3, 29 June 2007
-
-`Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>`_
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-This version of the GNU Lesser General Public License incorporates the
-terms and conditions of version 3 of the GNU General Public License,
-supplemented by the additional permissions listed below.
-
-0. Additional Definitions.
-##########################
-
-As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the
-GNU General Public License.
-
-"The Library" refers to a covered work governed by this License, other
-than an Application or a Combined Work as defined below.
-
-An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-A "Combined Work" is a work produced by combining or linking an
-Application with the Library. The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-1. Exception to Section 3 of the GNU GPL.
-#########################################
-
-You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-2. Conveying Modified Versions.
-###############################
-
-If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
--   a) under this License, provided that you make a good faith effort
-    to ensure that, in the event an Application does not supply the
-    function or data, the facility still operates, and performs
-    whatever part of its purpose remains meaningful, or
--   b) under the GNU GPL, with none of the additional permissions of
-    this License applicable to that copy.
-
-3. Object Code Incorporating Material from Library Header Files.
-################################################################
-
-The object code form of an Application may incorporate material from a
-header file that is part of the Library. You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
--   a) Give prominent notice with each copy of the object code that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the object code with a copy of the GNU GPL and this
-    license document.
-
-4. Combined Works.
-##################
-
-You may convey a Combined Work under terms of your choice that, taken
-together, effectively do not restrict modification of the portions of
-the Library contained in the Combined Work and reverse engineering for
-debugging such modifications, if you also do each of the following:
-
--   a) Give prominent notice with each copy of the Combined Work that
-    the Library is used in it and that the Library and its use are
-    covered by this License.
--   b) Accompany the Combined Work with a copy of the GNU GPL and this
-    license document.
--   c) For a Combined Work that displays copyright notices during
-    execution, include the copyright notice for the Library among
-    these notices, as well as a reference directing the user to the
-    copies of the GNU GPL and this license document.
--   d) Do one of the following:
-    -   0) Convey the Minimal Corresponding Source under the terms of
-        this License, and the Corresponding Application Code in a form
-        suitable for, and under terms that permit, the user to
-        recombine or relink the Application with a modified version of
-        the Linked Version to produce a modified Combined Work, in the
-        manner specified by section 6 of the GNU GPL for conveying
-        Corresponding Source.
-    -   1) Use a suitable shared library mechanism for linking with
-        the Library. A suitable mechanism is one that (a) uses at run
-        time a copy of the Library already present on the user's
-        computer system, and (b) will operate properly with a modified
-        version of the Library that is interface-compatible with the
-        Linked Version.
--   e) Provide Installation Information, but only if you would
-    otherwise be required to provide such information under section 6
-    of the GNU GPL, and only to the extent that such information is
-    necessary to install and execute a modified version of the
-    Combined Work produced by recombining or relinking the Application
-    with a modified version of the Linked Version. (If you use option
-    4d0, the Installation Information must accompany the Minimal
-    Corresponding Source and Corresponding Application Code. If you
-    use option 4d1, you must provide the Installation Information in
-    the manner specified by section 6 of the GNU GPL for conveying
-    Corresponding Source.)
-
-5. Combined Libraries.
-######################
-
-You may place library facilities that are a work based on the Library
-side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
--   a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities, conveyed under the terms of this License.
--   b) Give prominent notice with the combined library that part of it
-    is a work based on the Library, and explaining where to find the
-    accompanying uncombined form of the same work.
-
-6. Revised Versions of the GNU Lesser General Public License.
-#############################################################
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Library
-as you received it specifies that a certain numbered version of the
-GNU Lesser General Public License "or any later version" applies to
-it, you have the option of following the terms and conditions either
-of that published version or of any later version published by the
-Free Software Foundation. If the Library as you received it does not
-specify a version number of the GNU Lesser General Public License, you
-may choose any version of the GNU Lesser General Public License ever
-published by the Free Software Foundation.
-
-If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
-Library.
-
-GNU GENERAL PUBLIC LICENSE
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Version 3, 29 June 2007
-
-`Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>`_
-
-Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
-Preamble
-
-The GNU General Public License is a free, copyleft license for software and other kinds of works.
-
-The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
-
-When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
-
-To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
-
-For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
-
-Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
-
-For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
-
-Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
-
-Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
-
-The precise terms and conditions for copying, distribution and modification follow.
-TERMS AND CONDITIONS
-
-0. Definitions.
-###############
-
-“This License” refers to version 3 of the GNU General Public License.
-
-“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
-
-“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
-
-To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
-
-A “covered work” means either the unmodified Program or a work based on the Program.
-
-To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
-
-To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
-
-An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
-
-1. Source Code.
-###############
-
-The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
-
-A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
-
-The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
-
-The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same work.
-
-2. Basic Permissions.
-#####################
-
-All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
-
-3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-##############################################################
-
-No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
-
-When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
-
-4. Conveying Verbatim Copies.
-#############################
-
-You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
-
-5. Conveying Modified Source Versions.
-######################################
-
-You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
-    b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
-    c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
-    d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
-
-A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
-
-6. Conveying Non-Source Forms.
-##############################
-
-You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
-    b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
-    c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
-    d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
-    e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
-
-A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
-
-“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
-
-The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
-
-Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
-
-7. Additional Terms.
-####################
-
-“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
-    b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
-    c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
-    d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
-    e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
-    f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
-
-All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
-
-8. Termination.
-###############
-
-You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
-
-However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
-
-Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
-
-9. Acceptance Not Required for Having Copies.
-#############################################
-
-You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
-
-10. Automatic Licensing of Downstream Recipients.
-#################################################
-
-Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
-
-An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
-
-11. Patents.
-############
-
-A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
-
-A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
-
-In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
-
-A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
-
-12. No Surrender of Others' Freedom.
-####################################
-
-If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
-
-13. Use with the GNU Affero General Public License.
-###################################################
-
-Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
-
-14. Revised Versions of this License.
-#####################################
-
-The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
-
-Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
-
-15. Disclaimer of Warranty.
-###########################
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-16. Limitation of Liability.
-############################
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-17. Interpretation of Sections 15 and 16.
-#########################################
-
-If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
+Metadata-Version: 2.1
+Name: muFFT
+Version: 0.91.0
+Summary: Unified interface to MPI-parallel FFT libraries
+Author-Email: Ali Falsafi <ali.falsafi@epfl.ch>, Till Junge <till.junge@altermail.ch>, Richard Leute <richard.leute@imtek.uni-freiburg.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
+License:                     GNU GENERAL PUBLIC LICENSE
+                               Version 3, 29 June 2007
+        
+         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+         Everyone is permitted to copy and distribute verbatim copies
+         of this license document, but changing it is not allowed.
+        
+                                    Preamble
+        
+          The GNU General Public License is a free, copyleft license for
+        software and other kinds of works.
+        
+          The licenses for most software and other practical works are designed
+        to take away your freedom to share and change the works.  By contrast,
+        the GNU General Public License is intended to guarantee your freedom to
+        share and change all versions of a program--to make sure it remains free
+        software for all its users.  We, the Free Software Foundation, use the
+        GNU General Public License for most of our software; it applies also to
+        any other work released this way by its authors.  You can apply it to
+        your programs, too.
+        
+          When we speak of free software, we are referring to freedom, not
+        price.  Our General Public Licenses are designed to make sure that you
+        have the freedom to distribute copies of free software (and charge for
+        them if you wish), that you receive source code or can get it if you
+        want it, that you can change the software or use pieces of it in new
+        free programs, and that you know you can do these things.
+        
+          To protect your rights, we need to prevent others from denying you
+        these rights or asking you to surrender the rights.  Therefore, you have
+        certain responsibilities if you distribute copies of the software, or if
+        you modify it: responsibilities to respect the freedom of others.
+        
+          For example, if you distribute copies of such a program, whether
+        gratis or for a fee, you must pass on to the recipients the same
+        freedoms that you received.  You must make sure that they, too, receive
+        or can get the source code.  And you must show them these terms so they
+        know their rights.
+        
+          Developers that use the GNU GPL protect your rights with two steps:
+        (1) assert copyright on the software, and (2) offer you this License
+        giving you legal permission to copy, distribute and/or modify it.
+        
+          For the developers' and authors' protection, the GPL clearly explains
+        that there is no warranty for this free software.  For both users' and
+        authors' sake, the GPL requires that modified versions be marked as
+        changed, so that their problems will not be attributed erroneously to
+        authors of previous versions.
+        
+          Some devices are designed to deny users access to install or run
+        modified versions of the software inside them, although the manufacturer
+        can do so.  This is fundamentally incompatible with the aim of
+        protecting users' freedom to change the software.  The systematic
+        pattern of such abuse occurs in the area of products for individuals to
+        use, which is precisely where it is most unacceptable.  Therefore, we
+        have designed this version of the GPL to prohibit the practice for those
+        products.  If such problems arise substantially in other domains, we
+        stand ready to extend this provision to those domains in future versions
+        of the GPL, as needed to protect the freedom of users.
+        
+          Finally, every program is threatened constantly by software patents.
+        States should not allow patents to restrict development and use of
+        software on general-purpose computers, but in those that do, we wish to
+        avoid the special danger that patents applied to a free program could
+        make it effectively proprietary.  To prevent this, the GPL assures that
+        patents cannot be used to render the program non-free.
+        
+          The precise terms and conditions for copying, distribution and
+        modification follow.
+        
+                               TERMS AND CONDITIONS
+        
+          0. Definitions.
+        
+          "This License" refers to version 3 of the GNU General Public License.
+        
+          "Copyright" also means copyright-like laws that apply to other kinds of
+        works, such as semiconductor masks.
+        
+          "The Program" refers to any copyrightable work licensed under this
+        License.  Each licensee is addressed as "you".  "Licensees" and
+        "recipients" may be individuals or organizations.
+        
+          To "modify" a work means to copy from or adapt all or part of the work
+        in a fashion requiring copyright permission, other than the making of an
+        exact copy.  The resulting work is called a "modified version" of the
+        earlier work or a work "based on" the earlier work.
+        
+          A "covered work" means either the unmodified Program or a work based
+        on the Program.
+        
+          To "propagate" a work means to do anything with it that, without
+        permission, would make you directly or secondarily liable for
+        infringement under applicable copyright law, except executing it on a
+        computer or modifying a private copy.  Propagation includes copying,
+        distribution (with or without modification), making available to the
+        public, and in some countries other activities as well.
+        
+          To "convey" a work means any kind of propagation that enables other
+        parties to make or receive copies.  Mere interaction with a user through
+        a computer network, with no transfer of a copy, is not conveying.
+        
+          An interactive user interface displays "Appropriate Legal Notices"
+        to the extent that it includes a convenient and prominently visible
+        feature that (1) displays an appropriate copyright notice, and (2)
+        tells the user that there is no warranty for the work (except to the
+        extent that warranties are provided), that licensees may convey the
+        work under this License, and how to view a copy of this License.  If
+        the interface presents a list of user commands or options, such as a
+        menu, a prominent item in the list meets this criterion.
+        
+          1. Source Code.
+        
+          The "source code" for a work means the preferred form of the work
+        for making modifications to it.  "Object code" means any non-source
+        form of a work.
+        
+          A "Standard Interface" means an interface that either is an official
+        standard defined by a recognized standards body, or, in the case of
+        interfaces specified for a particular programming language, one that
+        is widely used among developers working in that language.
+        
+          The "System Libraries" of an executable work include anything, other
+        than the work as a whole, that (a) is included in the normal form of
+        packaging a Major Component, but which is not part of that Major
+        Component, and (b) serves only to enable use of the work with that
+        Major Component, or to implement a Standard Interface for which an
+        implementation is available to the public in source code form.  A
+        "Major Component", in this context, means a major essential component
+        (kernel, window system, and so on) of the specific operating system
+        (if any) on which the executable work runs, or a compiler used to
+        produce the work, or an object code interpreter used to run it.
+        
+          The "Corresponding Source" for a work in object code form means all
+        the source code needed to generate, install, and (for an executable
+        work) run the object code and to modify the work, including scripts to
+        control those activities.  However, it does not include the work's
+        System Libraries, or general-purpose tools or generally available free
+        programs which are used unmodified in performing those activities but
+        which are not part of the work.  For example, Corresponding Source
+        includes interface definition files associated with source files for
+        the work, and the source code for shared libraries and dynamically
+        linked subprograms that the work is specifically designed to require,
+        such as by intimate data communication or control flow between those
+        subprograms and other parts of the work.
+        
+          The Corresponding Source need not include anything that users
+        can regenerate automatically from other parts of the Corresponding
+        Source.
+        
+          The Corresponding Source for a work in source code form is that
+        same work.
+        
+          2. Basic Permissions.
+        
+          All rights granted under this License are granted for the term of
+        copyright on the Program, and are irrevocable provided the stated
+        conditions are met.  This License explicitly affirms your unlimited
+        permission to run the unmodified Program.  The output from running a
+        covered work is covered by this License only if the output, given its
+        content, constitutes a covered work.  This License acknowledges your
+        rights of fair use or other equivalent, as provided by copyright law.
+        
+          You may make, run and propagate covered works that you do not
+        convey, without conditions so long as your license otherwise remains
+        in force.  You may convey covered works to others for the sole purpose
+        of having them make modifications exclusively for you, or provide you
+        with facilities for running those works, provided that you comply with
+        the terms of this License in conveying all material for which you do
+        not control copyright.  Those thus making or running the covered works
+        for you must do so exclusively on your behalf, under your direction
+        and control, on terms that prohibit them from making any copies of
+        your copyrighted material outside their relationship with you.
+        
+          Conveying under any other circumstances is permitted solely under
+        the conditions stated below.  Sublicensing is not allowed; section 10
+        makes it unnecessary.
+        
+          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+        
+          No covered work shall be deemed part of an effective technological
+        measure under any applicable law fulfilling obligations under article
+        11 of the WIPO copyright treaty adopted on 20 December 1996, or
+        similar laws prohibiting or restricting circumvention of such
+        measures.
+        
+          When you convey a covered work, you waive any legal power to forbid
+        circumvention of technological measures to the extent such circumvention
+        is effected by exercising rights under this License with respect to
+        the covered work, and you disclaim any intention to limit operation or
+        modification of the work as a means of enforcing, against the work's
+        users, your or third parties' legal rights to forbid circumvention of
+        technological measures.
+        
+          4. Conveying Verbatim Copies.
+        
+          You may convey verbatim copies of the Program's source code as you
+        receive it, in any medium, provided that you conspicuously and
+        appropriately publish on each copy an appropriate copyright notice;
+        keep intact all notices stating that this License and any
+        non-permissive terms added in accord with section 7 apply to the code;
+        keep intact all notices of the absence of any warranty; and give all
+        recipients a copy of this License along with the Program.
+        
+          You may charge any price or no price for each copy that you convey,
+        and you may offer support or warranty protection for a fee.
+        
+          5. Conveying Modified Source Versions.
+        
+          You may convey a work based on the Program, or the modifications to
+        produce it from the Program, in the form of source code under the
+        terms of section 4, provided that you also meet all of these conditions:
+        
+            a) The work must carry prominent notices stating that you modified
+            it, and giving a relevant date.
+        
+            b) The work must carry prominent notices stating that it is
+            released under this License and any conditions added under section
+            7.  This requirement modifies the requirement in section 4 to
+            "keep intact all notices".
+        
+            c) You must license the entire work, as a whole, under this
+            License to anyone who comes into possession of a copy.  This
+            License will therefore apply, along with any applicable section 7
+            additional terms, to the whole of the work, and all its parts,
+            regardless of how they are packaged.  This License gives no
+            permission to license the work in any other way, but it does not
+            invalidate such permission if you have separately received it.
+        
+            d) If the work has interactive user interfaces, each must display
+            Appropriate Legal Notices; however, if the Program has interactive
+            interfaces that do not display Appropriate Legal Notices, your
+            work need not make them do so.
+        
+          A compilation of a covered work with other separate and independent
+        works, which are not by their nature extensions of the covered work,
+        and which are not combined with it such as to form a larger program,
+        in or on a volume of a storage or distribution medium, is called an
+        "aggregate" if the compilation and its resulting copyright are not
+        used to limit the access or legal rights of the compilation's users
+        beyond what the individual works permit.  Inclusion of a covered work
+        in an aggregate does not cause this License to apply to the other
+        parts of the aggregate.
+        
+          6. Conveying Non-Source Forms.
+        
+          You may convey a covered work in object code form under the terms
+        of sections 4 and 5, provided that you also convey the
+        machine-readable Corresponding Source under the terms of this License,
+        in one of these ways:
+        
+            a) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by the
+            Corresponding Source fixed on a durable physical medium
+            customarily used for software interchange.
+        
+            b) Convey the object code in, or embodied in, a physical product
+            (including a physical distribution medium), accompanied by a
+            written offer, valid for at least three years and valid for as
+            long as you offer spare parts or customer support for that product
+            model, to give anyone who possesses the object code either (1) a
+            copy of the Corresponding Source for all the software in the
+            product that is covered by this License, on a durable physical
+            medium customarily used for software interchange, for a price no
+            more than your reasonable cost of physically performing this
+            conveying of source, or (2) access to copy the
+            Corresponding Source from a network server at no charge.
+        
+            c) Convey individual copies of the object code with a copy of the
+            written offer to provide the Corresponding Source.  This
+            alternative is allowed only occasionally and noncommercially, and
+            only if you received the object code with such an offer, in accord
+            with subsection 6b.
+        
+            d) Convey the object code by offering access from a designated
+            place (gratis or for a charge), and offer equivalent access to the
+            Corresponding Source in the same way through the same place at no
+            further charge.  You need not require recipients to copy the
+            Corresponding Source along with the object code.  If the place to
+            copy the object code is a network server, the Corresponding Source
+            may be on a different server (operated by you or a third party)
+            that supports equivalent copying facilities, provided you maintain
+            clear directions next to the object code saying where to find the
+            Corresponding Source.  Regardless of what server hosts the
+            Corresponding Source, you remain obligated to ensure that it is
+            available for as long as needed to satisfy these requirements.
+        
+            e) Convey the object code using peer-to-peer transmission, provided
+            you inform other peers where the object code and Corresponding
+            Source of the work are being offered to the general public at no
+            charge under subsection 6d.
+        
+          A separable portion of the object code, whose source code is excluded
+        from the Corresponding Source as a System Library, need not be
+        included in conveying the object code work.
+        
+          A "User Product" is either (1) a "consumer product", which means any
+        tangible personal property which is normally used for personal, family,
+        or household purposes, or (2) anything designed or sold for incorporation
+        into a dwelling.  In determining whether a product is a consumer product,
+        doubtful cases shall be resolved in favor of coverage.  For a particular
+        product received by a particular user, "normally used" refers to a
+        typical or common use of that class of product, regardless of the status
+        of the particular user or of the way in which the particular user
+        actually uses, or expects or is expected to use, the product.  A product
+        is a consumer product regardless of whether the product has substantial
+        commercial, industrial or non-consumer uses, unless such uses represent
+        the only significant mode of use of the product.
+        
+          "Installation Information" for a User Product means any methods,
+        procedures, authorization keys, or other information required to install
+        and execute modified versions of a covered work in that User Product from
+        a modified version of its Corresponding Source.  The information must
+        suffice to ensure that the continued functioning of the modified object
+        code is in no case prevented or interfered with solely because
+        modification has been made.
+        
+          If you convey an object code work under this section in, or with, or
+        specifically for use in, a User Product, and the conveying occurs as
+        part of a transaction in which the right of possession and use of the
+        User Product is transferred to the recipient in perpetuity or for a
+        fixed term (regardless of how the transaction is characterized), the
+        Corresponding Source conveyed under this section must be accompanied
+        by the Installation Information.  But this requirement does not apply
+        if neither you nor any third party retains the ability to install
+        modified object code on the User Product (for example, the work has
+        been installed in ROM).
+        
+          The requirement to provide Installation Information does not include a
+        requirement to continue to provide support service, warranty, or updates
+        for a work that has been modified or installed by the recipient, or for
+        the User Product in which it has been modified or installed.  Access to a
+        network may be denied when the modification itself materially and
+        adversely affects the operation of the network or violates the rules and
+        protocols for communication across the network.
+        
+          Corresponding Source conveyed, and Installation Information provided,
+        in accord with this section must be in a format that is publicly
+        documented (and with an implementation available to the public in
+        source code form), and must require no special password or key for
+        unpacking, reading or copying.
+        
+          7. Additional Terms.
+        
+          "Additional permissions" are terms that supplement the terms of this
+        License by making exceptions from one or more of its conditions.
+        Additional permissions that are applicable to the entire Program shall
+        be treated as though they were included in this License, to the extent
+        that they are valid under applicable law.  If additional permissions
+        apply only to part of the Program, that part may be used separately
+        under those permissions, but the entire Program remains governed by
+        this License without regard to the additional permissions.
+        
+          When you convey a copy of a covered work, you may at your option
+        remove any additional permissions from that copy, or from any part of
+        it.  (Additional permissions may be written to require their own
+        removal in certain cases when you modify the work.)  You may place
+        additional permissions on material, added by you to a covered work,
+        for which you have or can give appropriate copyright permission.
+        
+          Notwithstanding any other provision of this License, for material you
+        add to a covered work, you may (if authorized by the copyright holders of
+        that material) supplement the terms of this License with terms:
+        
+            a) Disclaiming warranty or limiting liability differently from the
+            terms of sections 15 and 16 of this License; or
+        
+            b) Requiring preservation of specified reasonable legal notices or
+            author attributions in that material or in the Appropriate Legal
+            Notices displayed by works containing it; or
+        
+            c) Prohibiting misrepresentation of the origin of that material, or
+            requiring that modified versions of such material be marked in
+            reasonable ways as different from the original version; or
+        
+            d) Limiting the use for publicity purposes of names of licensors or
+            authors of the material; or
+        
+            e) Declining to grant rights under trademark law for use of some
+            trade names, trademarks, or service marks; or
+        
+            f) Requiring indemnification of licensors and authors of that
+            material by anyone who conveys the material (or modified versions of
+            it) with contractual assumptions of liability to the recipient, for
+            any liability that these contractual assumptions directly impose on
+            those licensors and authors.
+        
+          All other non-permissive additional terms are considered "further
+        restrictions" within the meaning of section 10.  If the Program as you
+        received it, or any part of it, contains a notice stating that it is
+        governed by this License along with a term that is a further
+        restriction, you may remove that term.  If a license document contains
+        a further restriction but permits relicensing or conveying under this
+        License, you may add to a covered work material governed by the terms
+        of that license document, provided that the further restriction does
+        not survive such relicensing or conveying.
+        
+          If you add terms to a covered work in accord with this section, you
+        must place, in the relevant source files, a statement of the
+        additional terms that apply to those files, or a notice indicating
+        where to find the applicable terms.
+        
+          Additional terms, permissive or non-permissive, may be stated in the
+        form of a separately written license, or stated as exceptions;
+        the above requirements apply either way.
+        
+          8. Termination.
+        
+          You may not propagate or modify a covered work except as expressly
+        provided under this License.  Any attempt otherwise to propagate or
+        modify it is void, and will automatically terminate your rights under
+        this License (including any patent licenses granted under the third
+        paragraph of section 11).
+        
+          However, if you cease all violation of this License, then your
+        license from a particular copyright holder is reinstated (a)
+        provisionally, unless and until the copyright holder explicitly and
+        finally terminates your license, and (b) permanently, if the copyright
+        holder fails to notify you of the violation by some reasonable means
+        prior to 60 days after the cessation.
+        
+          Moreover, your license from a particular copyright holder is
+        reinstated permanently if the copyright holder notifies you of the
+        violation by some reasonable means, this is the first time you have
+        received notice of violation of this License (for any work) from that
+        copyright holder, and you cure the violation prior to 30 days after
+        your receipt of the notice.
+        
+          Termination of your rights under this section does not terminate the
+        licenses of parties who have received copies or rights from you under
+        this License.  If your rights have been terminated and not permanently
+        reinstated, you do not qualify to receive new licenses for the same
+        material under section 10.
+        
+          9. Acceptance Not Required for Having Copies.
+        
+          You are not required to accept this License in order to receive or
+        run a copy of the Program.  Ancillary propagation of a covered work
+        occurring solely as a consequence of using peer-to-peer transmission
+        to receive a copy likewise does not require acceptance.  However,
+        nothing other than this License grants you permission to propagate or
+        modify any covered work.  These actions infringe copyright if you do
+        not accept this License.  Therefore, by modifying or propagating a
+        covered work, you indicate your acceptance of this License to do so.
+        
+          10. Automatic Licensing of Downstream Recipients.
+        
+          Each time you convey a covered work, the recipient automatically
+        receives a license from the original licensors, to run, modify and
+        propagate that work, subject to this License.  You are not responsible
+        for enforcing compliance by third parties with this License.
+        
+          An "entity transaction" is a transaction transferring control of an
+        organization, or substantially all assets of one, or subdividing an
+        organization, or merging organizations.  If propagation of a covered
+        work results from an entity transaction, each party to that
+        transaction who receives a copy of the work also receives whatever
+        licenses to the work the party's predecessor in interest had or could
+        give under the previous paragraph, plus a right to possession of the
+        Corresponding Source of the work from the predecessor in interest, if
+        the predecessor has it or can get it with reasonable efforts.
+        
+          You may not impose any further restrictions on the exercise of the
+        rights granted or affirmed under this License.  For example, you may
+        not impose a license fee, royalty, or other charge for exercise of
+        rights granted under this License, and you may not initiate litigation
+        (including a cross-claim or counterclaim in a lawsuit) alleging that
+        any patent claim is infringed by making, using, selling, offering for
+        sale, or importing the Program or any portion of it.
+        
+          11. Patents.
+        
+          A "contributor" is a copyright holder who authorizes use under this
+        License of the Program or a work on which the Program is based.  The
+        work thus licensed is called the contributor's "contributor version".
+        
+          A contributor's "essential patent claims" are all patent claims
+        owned or controlled by the contributor, whether already acquired or
+        hereafter acquired, that would be infringed by some manner, permitted
+        by this License, of making, using, or selling its contributor version,
+        but do not include claims that would be infringed only as a
+        consequence of further modification of the contributor version.  For
+        purposes of this definition, "control" includes the right to grant
+        patent sublicenses in a manner consistent with the requirements of
+        this License.
+        
+          Each contributor grants you a non-exclusive, worldwide, royalty-free
+        patent license under the contributor's essential patent claims, to
+        make, use, sell, offer for sale, import and otherwise run, modify and
+        propagate the contents of its contributor version.
+        
+          In the following three paragraphs, a "patent license" is any express
+        agreement or commitment, however denominated, not to enforce a patent
+        (such as an express permission to practice a patent or covenant not to
+        sue for patent infringement).  To "grant" such a patent license to a
+        party means to make such an agreement or commitment not to enforce a
+        patent against the party.
+        
+          If you convey a covered work, knowingly relying on a patent license,
+        and the Corresponding Source of the work is not available for anyone
+        to copy, free of charge and under the terms of this License, through a
+        publicly available network server or other readily accessible means,
+        then you must either (1) cause the Corresponding Source to be so
+        available, or (2) arrange to deprive yourself of the benefit of the
+        patent license for this particular work, or (3) arrange, in a manner
+        consistent with the requirements of this License, to extend the patent
+        license to downstream recipients.  "Knowingly relying" means you have
+        actual knowledge that, but for the patent license, your conveying the
+        covered work in a country, or your recipient's use of the covered work
+        in a country, would infringe one or more identifiable patents in that
+        country that you have reason to believe are valid.
+        
+          If, pursuant to or in connection with a single transaction or
+        arrangement, you convey, or propagate by procuring conveyance of, a
+        covered work, and grant a patent license to some of the parties
+        receiving the covered work authorizing them to use, propagate, modify
+        or convey a specific copy of the covered work, then the patent license
+        you grant is automatically extended to all recipients of the covered
+        work and works based on it.
+        
+          A patent license is "discriminatory" if it does not include within
+        the scope of its coverage, prohibits the exercise of, or is
+        conditioned on the non-exercise of one or more of the rights that are
+        specifically granted under this License.  You may not convey a covered
+        work if you are a party to an arrangement with a third party that is
+        in the business of distributing software, under which you make payment
+        to the third party based on the extent of your activity of conveying
+        the work, and under which the third party grants, to any of the
+        parties who would receive the covered work from you, a discriminatory
+        patent license (a) in connection with copies of the covered work
+        conveyed by you (or copies made from those copies), or (b) primarily
+        for and in connection with specific products or compilations that
+        contain the covered work, unless you entered into that arrangement,
+        or that patent license was granted, prior to 28 March 2007.
+        
+          Nothing in this License shall be construed as excluding or limiting
+        any implied license or other defenses to infringement that may
+        otherwise be available to you under applicable patent law.
+        
+          12. No Surrender of Others' Freedom.
+        
+          If conditions are imposed on you (whether by court order, agreement or
+        otherwise) that contradict the conditions of this License, they do not
+        excuse you from the conditions of this License.  If you cannot convey a
+        covered work so as to satisfy simultaneously your obligations under this
+        License and any other pertinent obligations, then as a consequence you may
+        not convey it at all.  For example, if you agree to terms that obligate you
+        to collect a royalty for further conveying from those to whom you convey
+        the Program, the only way you could satisfy both those terms and this
+        License would be to refrain entirely from conveying the Program.
+        
+          13. Use with the GNU Affero General Public License.
+        
+          Notwithstanding any other provision of this License, you have
+        permission to link or combine any covered work with a work licensed
+        under version 3 of the GNU Affero General Public License into a single
+        combined work, and to convey the resulting work.  The terms of this
+        License will continue to apply to the part which is the covered work,
+        but the special requirements of the GNU Affero General Public License,
+        section 13, concerning interaction through a network will apply to the
+        combination as such.
+        
+          14. Revised Versions of this License.
+        
+          The Free Software Foundation may publish revised and/or new versions of
+        the GNU General Public License from time to time.  Such new versions will
+        be similar in spirit to the present version, but may differ in detail to
+        address new problems or concerns.
+        
+          Each version is given a distinguishing version number.  If the
+        Program specifies that a certain numbered version of the GNU General
+        Public License "or any later version" applies to it, you have the
+        option of following the terms and conditions either of that numbered
+        version or of any later version published by the Free Software
+        Foundation.  If the Program does not specify a version number of the
+        GNU General Public License, you may choose any version ever published
+        by the Free Software Foundation.
+        
+          If the Program specifies that a proxy can decide which future
+        versions of the GNU General Public License can be used, that proxy's
+        public statement of acceptance of a version permanently authorizes you
+        to choose that version for the Program.
+        
+          Later license versions may give you additional or different
+        permissions.  However, no additional obligations are imposed on any
+        author or copyright holder as a result of your choosing to follow a
+        later version.
+        
+          15. Disclaimer of Warranty.
+        
+          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+        
+          16. Limitation of Liability.
+        
+          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+        SUCH DAMAGES.
+        
+          17. Interpretation of Sections 15 and 16.
+        
+          If the disclaimer of warranty and limitation of liability provided
+        above cannot be given local legal effect according to their terms,
+        reviewing courts shall apply local law that most closely approximates
+        an absolute waiver of all civil liability in connection with the
+        Program, unless a warranty or assumption of liability accompanies a
+        copy of the Program in return for a fee.
+        
+                             END OF TERMS AND CONDITIONS
+        
+                    How to Apply These Terms to Your New Programs
+        
+          If you develop a new program, and you want it to be of the greatest
+        possible use to the public, the best way to achieve this is to make it
+        free software which everyone can redistribute and change under these terms.
+        
+          To do so, attach the following notices to the program.  It is safest
+        to attach them to the start of each source file to most effectively
+        state the exclusion of warranty; and each file should have at least
+        the "copyright" line and a pointer to where the full notice is found.
+        
+            <one line to give the program's name and a brief idea of what it does.>
+            Copyright (C) <year>  <name of author>
+        
+            This program is free software: you can redistribute it and/or modify
+            it under the terms of the GNU General Public License as published by
+            the Free Software Foundation, either version 3 of the License, or
+            (at your option) any later version.
+        
+            This program is distributed in the hope that it will be useful,
+            but WITHOUT ANY WARRANTY; without even the implied warranty of
+            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+            GNU General Public License for more details.
+        
+            You should have received a copy of the GNU General Public License
+            along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        
+        Also add information on how to contact you by electronic and paper mail.
+        
+          If the program does terminal interaction, make it output a short
+        notice like this when it starts in an interactive mode:
+        
+            <program>  Copyright (C) <year>  <name of author>
+            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+            This is free software, and you are welcome to redistribute it
+            under certain conditions; type `show c' for details.
+        
+        The hypothetical commands `show w' and `show c' should show the appropriate
+        parts of the General Public License.  Of course, your program's commands
+        might be different; for a GUI interface, you would use an "about box".
+        
+          You should also get your employer (if you work as a programmer) or school,
+        if any, to sign a "copyright disclaimer" for the program, if necessary.
+        For more information on this, and how to apply and follow the GNU GPL, see
+        <https://www.gnu.org/licenses/>.
+        
+          The GNU General Public License does not permit incorporating your program
+        into proprietary programs.  If your program is a subroutine library, you
+        may consider it more useful to permit linking proprietary applications with
+        the library.  If this is what you want to do, use the GNU Lesser General
+        Public License instead of this License.  But first, please read
+        <https://www.gnu.org/licenses/why-not-lgpl.html>.
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Project-URL: Documentation, https://muspectre.github.io/muFFT/
+Project-URL: Repository, https://github.com/muSpectre/muFFT
+Project-URL: Changelog, https://github.com/muSpectre/muFFT/blob/main/CHANGELOG.md
+Requires-Python: >=3.8.0
+Requires-Dist: muGrid==0.91.1
+Requires-Dist: numpy
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: test
+Description-Content-Type: text/markdown
+
+# µFFT
+
+µFFT is a unified interface to serial and MPI-parallel FFT libraries, build on
+top of [µGrid](https://github.com/muSpectre/muGrid).
+µGrid and µFFT make it easy to implement algorithms that operate on fields,
+such as solving partial  differential equations. It supports parallelization
+using domain decomposition  implemented using the Message Passing Interface (MPI).
+
+µFFT is written in C++ and currently has language bindings for
+[Python](https://www.python.org/).
+
+This README contains only a small quick start guide. Please refer to the
+[full documentation](https://muspectre.github.io/muFFT/) for more help.
+
+## Quick start
+
+To install µFFT, run
+
+    pip install muFFT
+
+Note that on most platforms this will install a binary wheel, that was
+compiled with a minimal configuration. To compile for your specific platform
+use
+
+    pip install -v --no-binary muFFT muFFT
+
+which will compile the code. µFFT will autodetect
+µFFT will autodetect
+[MPI](https://www.mpi-forum.org/),
+[FFTW](https://www.fftw.org/),
+[MPIFFTW](https://www.fftw.org/fftw3_doc/FFTW-MPI-Installation.html)
+and
+[PFFT](https://github.com/mpip/pfft).
+Monitor output to see which of these options were automatically detected.
+
+## Funding
+
+This development has received funding from the
+[Swiss National Science Foundation](https://www.snf.ch/en)
+within an Ambizione Project and by the
+[European Research Council](https://erc.europa.eu) within
+[Starting Grant 757343](https://cordis.europa.eu/project/id/757343).
```

### Comparing `mufft-0.90.0/doc/dev-docs/source/conf.py` & `mufft-0.91.0/doc/source/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,151 +1,141 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
-# µSpectre documentation build configuration file, created by
+# µFFT documentation build configuration file, created by
 # sphinx-quickstart on Thu Feb  1 12:01:24 2018.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#
 import os
+import pathlib
 import subprocess
+
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.autodoc',
+extensions = ['breathe',
+              'sphinx.ext.autodoc',
               'sphinx.ext.intersphinx',
               'sphinx.ext.todo',
               'sphinx.ext.coverage',
               'sphinx.ext.mathjax',
               'sphinx.ext.viewcode',
-              'sphinx.ext.ifconfig',
-              'breathe']
+              'sphinx.ext.ifconfig']
 read_the_docs_build = os.environ.get('READTHEDOCS', None) == 'True'
 if os.environ.get('READTHEDOCS', None) is not None:
     print("${READTHEDOCS} = " + os.environ.get('READTHEDOCS', None))
 
-if read_the_docs_build:
-    muspectre_path = "."
-else:
-    muspectre_path = "@CMAKE_CURRENT_BINARY_DIR@"
-    os.makedirs("@CMAKE_CURRENT_BINARY_DIR@/_static", exist_ok=True)
-
-print("muspectre_path = '{}'".format(muspectre_path))
-subprocess.call('ls; pwd', shell=True)
-subprocess.call("cd {} && doxygen".format(muspectre_path), shell=True)
+# Get version of Doxygen and save it as a tuple
+
+doxygen_test = subprocess.run(["doxygen", "--version"], capture_output=True)
+if doxygen_test.returncode < 0:
+    raise RuntimeError(
+        "doxygen --version reported the following error:\n\t"
+        + str(doxygen_test.stderr, encoding="utf-8")
+    )
+doxygen_version = tuple(
+    int(x) for x in str(doxygen_test.stdout, encoding="utf-8").split()[0].split(".")
+)
+print("Using Doxygen v%d.%d.%d" % doxygen_version)
+
+# Get a description of the current position. Use Popen for 2.6 compat
+git_tag = subprocess.Popen(["git", "describe", "--tags"], stdout=subprocess.PIPE).communicate()[0]
+
+# convert from bytes to string
+git_tag = git_tag.decode("ascii")
 
-breathe_projects = {"µSpectre": os.path.join(muspectre_path, "doxygenxml")}
-breathe_default_project = "µSpectre"
+breathe_projects = {
+    "libmufft": "../xml"
+}
+breathe_default_project = "libmufft"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'µSpectre'
-copyright = '2018, Till Junge'
-author = 'Till Junge'
+project = 'µFFT'
+copyright = '2017-2022 Till Junge, 2018-2024 Lars Pastewka'
+author = 'Till Junge, Lars Pastewka'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = 'v0.1'
+version = git_tag
 # The full version, including alpha/beta/rc tags.
-release = 'v0.1 α'
+release = git_tag
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["CmakeLists.txt"]
+exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
-
 # -- Options for HTML output ----------------------------------------------
 
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-on_rtd = os.environ.get('READTHEDOCS') == 'True'
-if on_rtd:
-    html_theme = 'default'
-else:
-    html_theme = 'sphinx_rtd_theme'
+html_theme = 'furo'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
-# Custom sidebar templates, must be a dictionary that maps document names
-# to template names.
-#
-# This is required for the alabaster theme
-# refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
-html_sidebars = {
-    '**': [
-        'relations.html',  # needs 'show_related': True theme option to display
-        'searchbox.html',
-    ]
-}
-
-
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'Spectredoc'
-
+htmlhelp_basename = 'FFTdoc'
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
@@ -165,42 +155,38 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'Spectre.tex', 'µSpectre Documentation',
+    (master_doc, 'FFT.tex', 'µFFT Documentation',
      'Till Junge', 'manual'),
 ]
 
-
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'spectre', 'µSpectre Documentation',
+    (master_doc, 'fft', 'µFFT Documentation',
      [author], 1)
 ]
 
-
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'Spectre', 'µSpectre Documentation',
-     author, 'Spectre', 'One line description of project.',
+    (master_doc, 'FFT', 'µFFT Documentation',
+     author, 'FFT', 'Unified interface to MPI-parallel FFT libraries',
      'Miscellaneous'),
 ]
 
-
-
 # -- Options for Epub output ----------------------------------------------
 
 # Bibliographic Dublin Core info.
 epub_title = project
 epub_author = author
 epub_publisher = author
 epub_copyright = copyright
@@ -213,13 +199,11 @@
 # A unique identification for the text.
 #
 # epub_uid = ''
 
 # A list of files that should not be packed into the epub file.
 epub_exclude_files = ['search.html']
 
-
-
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'https://docs.python.org/': None}
+intersphinx_mapping = {'python': ('https://docs.python.org/', None)}
 primary_domain = 'cpp'
 highlight_language = 'cpp'
```

### Comparing `mufft-0.90.0/language_bindings/python/bind_py_common_mufft.cc` & `mufft-0.91.0/language_bindings/python/bind_py_common_mufft.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/bind_py_declarations.hh` & `mufft-0.91.0/language_bindings/python/bind_py_declarations.hh`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/bind_py_derivatives.cc` & `mufft-0.91.0/language_bindings/python/bind_py_derivatives.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/bind_py_fftengine.cc` & `mufft-0.91.0/language_bindings/python/bind_py_fftengine.cc`

 * *Files 12% similar despite different names*

```diff
@@ -139,116 +139,111 @@
              FFTEngineBase             // trampoline base
              >
       fft_engine(mod, name.c_str());
   fft_engine
       .def(py::init([](std::vector<Index_t> nb_grid_pts,
                        muFFT::Communicator & comm,
                        const muFFT::FFT_PlanFlags & plan_flags,
-                       bool allow_temporary_buffer,
-                       bool allow_destroy_input) {
+                       bool allow_temporary_buffer, bool allow_destroy_input) {
              // Initialise with muFFT Communicator object
              return new Engine(DynCcoord_t(nb_grid_pts), comm, plan_flags,
                                allow_temporary_buffer, allow_destroy_input);
            }),
            "nb_grid_pts"_a, "communicator"_a = muFFT::Communicator(),
            "flags"_a = muFFT::FFT_PlanFlags::estimate,
            "allow_temporary_buffer"_a = true, "allow_destroy_input"_a = false)
 #ifdef WITH_MPI
       .def(py::init([](std::vector<Index_t> nb_grid_pts,
                        const muFFT::FFT_PlanFlags & plan_flags,
-                       bool allow_temporary_buffer,
-                       bool allow_destroy_input,
+                       bool allow_temporary_buffer, bool allow_destroy_input,
                        size_t comm) {
              // Initialise with bare MPI handle
              return new Engine(DynCcoord_t(nb_grid_pts),
-                               muFFT::Communicator(MPI_Comm(comm)),
-                               plan_flags,
-                               allow_temporary_buffer,
-                               allow_destroy_input);
+                               muFFT::Communicator(MPI_Comm(comm)), plan_flags,
+                               allow_temporary_buffer, allow_destroy_input);
            }),
            "nb_grid_pts"_a, "communicator"_a = size_t(MPI_COMM_SELF),
            "flags"_a = muFFT::FFT_PlanFlags::estimate,
-           "allow_temporary_buffer"_a = true,
-           "allow_destroy_input"_a = false)
+           "allow_temporary_buffer"_a = true, "allow_destroy_input"_a = false)
 #endif
       .def("fft", &Engine::fft)
       .def("ifft", &Engine::ifft)
       .def("hcfft", &Engine::hcfft)
       .def("ihcfft", &Engine::ihcfft)
       .def("create_plan", &Engine::create_plan, "nb_dof_per_pixel"_a)
       .def("register_real_space_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Index_t &)) &
                Engine::register_real_space_field,
-           "unique_name"_a, "nb_dof_per_pixel"_a,
+           "unique_name"_a, "nb_dof_per_pixel"_a = 1,
            py::return_value_policy::reference_internal)
       .def("register_real_space_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Shape_t &)) &
                Engine::register_real_space_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_real_space_field",
+      .def("real_space_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Index_t &)) &
-               Engine::fetch_or_register_real_space_field,
-           "unique_name"_a, "nb_dof_per_pixel"_a,
+               Engine::real_space_field,
+           "unique_name"_a, "nb_dof_per_pixel"_a = 1,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_real_space_field",
+      .def("real_space_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Shape_t &)) &
-               Engine::fetch_or_register_real_space_field,
+               Engine::real_space_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
       .def("register_halfcomplex_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Index_t &)) &
                Engine::register_halfcomplex_field,
-           "unique_name"_a, "nb_dof_per_pixel"_a,
+           "unique_name"_a, "nb_dof_per_pixel"_a = 1,
            py::return_value_policy::reference_internal)
       .def("register_halfcomplex_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Shape_t &)) &
                Engine::register_halfcomplex_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_halfcomplex_field",
+      .def("halfcomplex_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Index_t &)) &
-               Engine::fetch_or_register_halfcomplex_field,
+               Engine::halfcomplex_field,
            "unique_name"_a, "nb_dof_per_pixel"_a,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_halfcomplex_field",
+      .def("halfcomplex_field",
            (FFTEngineBase::RealField_t &
             (Engine::*)(const std::string &, const Shape_t &)) &
-               Engine::fetch_or_register_halfcomplex_field,
+               Engine::halfcomplex_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
       .def("register_fourier_space_field",
            (muGrid::ComplexField &
             (Engine::*)(const std::string &, const Index_t &)) &
                Engine::register_fourier_space_field,
-           "unique_name"_a, "nb_dof_per_pixel"_a,
+           "unique_name"_a, "nb_dof_per_pixel"_a = 1,
            py::return_value_policy::reference_internal)
       .def("register_fourier_space_field",
            (muGrid::ComplexField &
             (Engine::*)(const std::string &, const Shape_t &)) &
                Engine::register_fourier_space_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_fourier_space_field",
+      .def("fourier_space_field",
            (FFTEngineBase::FourierField_t &
             (Engine::*)(const std::string &, const Index_t &)) &
-               Engine::fetch_or_register_fourier_space_field,
-           "unique_name"_a, "nb_dof_per_pixel"_a,
+               Engine::fourier_space_field,
+           "unique_name"_a, "nb_dof_per_pixel"_a = 1,
            py::return_value_policy::reference_internal)
-      .def("fetch_or_register_fourier_space_field",
+      .def("fourier_space_field",
            (FFTEngineBase::FourierField_t &
             (Engine::*)(const std::string &, const Shape_t &)) &
-               Engine::fetch_or_register_fourier_space_field,
+               Engine::fourier_space_field,
            "unique_name"_a, "shape"_a,
            py::return_value_policy::reference_internal)
       .def_property_readonly("normalisation", &Engine::normalisation)
       .def_property_readonly("communicator", &Engine::get_communicator)
       .def_property_readonly(
           "nb_subdomain_grid_pts",
           [](const Engine & eng) {
@@ -313,183 +308,189 @@
               t[dim] = py::slice(locs[dim], locs[dim] + nb_pts[dim], 1);
             }
             return t;
           },
           py::return_value_policy::reference)
       .def_property_readonly("spatial_dim", &Engine::get_spatial_dim)
       .def("has_plan_for", &Engine::has_plan_for, "nb_dof_per_pixel"_a)
-      .def_property_readonly("fftfreq", [](const Engine & eng) {
-        std::vector<Index_t> shape{}, strides{};
-        Index_t dim{eng.get_spatial_dim()};
-        shape.push_back(dim);
-        strides.push_back(sizeof(Real));
-        for (auto && n : eng.get_nb_fourier_grid_pts()) {
-          shape.push_back(n);
-        }
-        for (auto && s : eng.get_fourier_pixels().get_strides()) {
-          strides.push_back(s * dim * sizeof(Real));
-        }
-        py::array_t<Real> fftfreqs(shape, strides);
-        Real * ptr{static_cast<Real *>(fftfreqs.request().ptr)};
-        auto & nb_domain_grid_pts{eng.get_nb_domain_grid_pts()};
-        for (auto && pix : eng.get_fourier_pixels()) {
-          for (int i = 0; i < dim; ++i) {
-            ptr[i] =
-                static_cast<Real>(fft_freq(pix[i], nb_domain_grid_pts[i])) /
-                nb_domain_grid_pts[i];
-          }
-          ptr += dim;
-        }
-        return fftfreqs;
-      })
+      .def_property_readonly(
+          "coords",
+          [](const Engine & eng) {
+            std::vector<Index_t> shape{}, strides{};
+            Index_t dim{eng.get_spatial_dim()};
+            shape.push_back(dim);
+            strides.push_back(sizeof(Real));
+            for (auto && n : eng.get_nb_subdomain_grid_pts()) {
+              shape.push_back(n);
+            }
+            for (auto && s : eng.get_real_pixels().get_strides()) {
+              strides.push_back(s * dim * sizeof(Real));
+            }
+            py::array_t<Real> coords(shape, strides);
+            Real * ptr{static_cast<Real *>(coords.request().ptr)};
+            auto & nb_domain_grid_pts{eng.get_nb_domain_grid_pts()};
+            for (auto && pix : eng.get_real_pixels()) {
+              for (int i = 0; i < dim; ++i) {
+                ptr[i] = static_cast<Real>(pix[i]) / nb_domain_grid_pts[i];
+              }
+              ptr += dim;
+            }
+            return coords;
+          })
+      .def_property_readonly(
+          "fftfreq",
+          [](const Engine & eng) {
+            std::vector<Index_t> shape{}, strides{};
+            Index_t dim{eng.get_spatial_dim()};
+            shape.push_back(dim);
+            strides.push_back(sizeof(Real));
+            for (auto && n : eng.get_nb_fourier_grid_pts()) {
+              shape.push_back(n);
+            }
+            for (auto && s : eng.get_fourier_pixels().get_strides()) {
+              strides.push_back(s * dim * sizeof(Real));
+            }
+            py::array_t<Real> fftfreqs(shape, strides);
+            Real * ptr{static_cast<Real *>(fftfreqs.request().ptr)};
+            auto & nb_domain_grid_pts{eng.get_nb_domain_grid_pts()};
+            for (auto && pix : eng.get_fourier_pixels()) {
+              for (int i = 0; i < dim; ++i) {
+                ptr[i] =
+                    static_cast<Real>(fft_freq(pix[i], nb_domain_grid_pts[i])) /
+                    nb_domain_grid_pts[i];
+              }
+              ptr += dim;
+            }
+            return fftfreqs;
+          })
       .def(
           "fft",
-          [](Engine & eng,
-             py::array_t<Real> & input_array,
+          [](Engine & eng, py::array_t<Real> & input_array,
              py::array_t<Complex> & output_array) {
             const py::buffer_info & info = input_array.request();
             auto & dim{eng.get_fourier_pixels().get_dim()};
             if (info.shape.size() < static_cast<size_t>(dim)) {
               std::stringstream s;
               s << "Input array has " << info.shape.size() << " dimensions "
                 << "but FFT engine was set up for " << dim << " dimensions.";
               throw muFFT::FFTEngineError(s.str());
             }
-            auto nb_dof_per_pixel{
-                std::accumulate(info.shape.begin(), info.shape.end()-dim, 1,
-                                std::multiplies<Index_t>())};
-            NumpyProxy<Real> input_proxy(eng.get_nb_domain_grid_pts(),
-                                         eng.get_nb_subdomain_grid_pts(),
-                                         eng.get_subdomain_locations(),
-                                         nb_dof_per_pixel, input_array);
-            NumpyProxy<Complex> output_proxy(eng.get_nb_domain_grid_pts(),
-                                             eng.get_nb_fourier_grid_pts(),
-                                             eng.get_fourier_locations(),
-                                             nb_dof_per_pixel, output_array);
+            auto nb_dof_per_pixel{std::accumulate(info.shape.begin(),
+                                                  info.shape.end() - dim, 1,
+                                                  std::multiplies<Index_t>())};
+            NumpyProxy<Real> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, input_array);
+            NumpyProxy<Complex> output_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_fourier_grid_pts(),
+                eng.get_fourier_locations(), nb_dof_per_pixel, output_array);
             eng.fft(input_proxy.get_field(), output_proxy.get_field());
           },
           "real_input_array"_a, "complex_output_array"_a,
           "Perform forward FFT of the input array into the output array")
       .def(
           "ifft",
-          [](Engine & eng,
-             py::array_t<Complex> & input_array,
+          [](Engine & eng, py::array_t<Complex> & input_array,
              py::array_t<Real> & output_array) {
             const py::buffer_info & info = input_array.request();
             auto & dim{eng.get_fourier_pixels().get_dim()};
             if (info.shape.size() < static_cast<size_t>(dim)) {
               std::stringstream s;
               s << "Input array has " << info.shape.size() << " dimensions "
                 << "but FFT engine was set up for " << dim << " dimensions.";
               throw muFFT::FFTEngineError(s.str());
             }
-            auto nb_dof_per_pixel{
-                std::accumulate(info.shape.begin(), info.shape.end()-dim, 1,
-                                std::multiplies<Index_t>())};
-            NumpyProxy<Complex> input_proxy(eng.get_nb_domain_grid_pts(),
-                                            eng.get_nb_fourier_grid_pts(),
-                                            eng.get_fourier_locations(),
-                                            nb_dof_per_pixel, input_array);
-            NumpyProxy<Real> output_proxy(eng.get_nb_domain_grid_pts(),
-                                          eng.get_nb_subdomain_grid_pts(),
-                                          eng.get_subdomain_locations(),
-                                          nb_dof_per_pixel, output_array);
+            auto nb_dof_per_pixel{std::accumulate(info.shape.begin(),
+                                                  info.shape.end() - dim, 1,
+                                                  std::multiplies<Index_t>())};
+            NumpyProxy<Complex> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_fourier_grid_pts(),
+                eng.get_fourier_locations(), nb_dof_per_pixel, input_array);
+            NumpyProxy<Real> output_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, output_array);
             eng.ifft(input_proxy.get_field(), output_proxy.get_field());
           },
           "fourier_input_array"_a, "real_output_array"_a,
           "Perform inverse FFT of the input array into the output array.")
       .def(
           "fft",
-          [](Engine & eng,
-             py::array_t<Real> & input_array) {
+          [](Engine & eng, py::array_t<Real> & input_array) {
             const py::buffer_info & info = input_array.request();
             auto & dim{eng.get_fourier_pixels().get_dim()};
             if (info.shape.size() < static_cast<size_t>(dim)) {
               std::stringstream s;
               s << "Input array has " << info.shape.size() << " dimensions "
                 << "but FFT engine was set up for " << dim << " dimensions.";
               throw muFFT::FFTEngineError(s.str());
             }
-            auto nb_dof_per_pixel{
-                std::accumulate(info.shape.begin(), info.shape.end()-dim, 1,
-                                std::multiplies<Index_t>())};
-            NumpyProxy<Real> input_proxy(eng.get_nb_domain_grid_pts(),
-                                         eng.get_nb_subdomain_grid_pts(),
-                                         eng.get_subdomain_locations(),
-                                         nb_dof_per_pixel, input_array);
-            auto & output_field{
-                eng.fetch_or_register_fourier_space_field(
-                    "fft return buffer",
-                    input_proxy.get_components_shape())};
+            auto nb_dof_per_pixel{std::accumulate(info.shape.begin(),
+                                                  info.shape.end() - dim, 1,
+                                                  std::multiplies<Index_t>())};
+            NumpyProxy<Real> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, input_array);
+            auto & output_field{eng.fourier_space_field(
+                "fft return buffer", input_proxy.get_components_shape())};
             eng.fft(input_proxy.get_field(), output_field);
             return numpy_wrap(output_field, IterUnit::Pixel);
           },
           "real_input_array"_a,
           "Perform forward FFT of the input array into the output array")
       .def(
           "ifft",
-          [](Engine & eng,
-             py::array_t<Complex> & input_array) {
+          [](Engine & eng, py::array_t<Complex> & input_array) {
             const py::buffer_info & info = input_array.request();
             auto & dim{eng.get_fourier_pixels().get_dim()};
             if (info.shape.size() < static_cast<size_t>(dim)) {
               std::stringstream s;
               s << "Input array has " << info.shape.size() << " dimensions "
                 << "but FFT engine was set up for " << dim << " dimensions.";
               throw muFFT::FFTEngineError(s.str());
             }
-            auto nb_dof_per_pixel{
-                std::accumulate(info.shape.begin(), info.shape.end()-dim, 1,
-                                std::multiplies<Index_t>())};
-            NumpyProxy<Complex> input_proxy(eng.get_nb_domain_grid_pts(),
-                                            eng.get_nb_fourier_grid_pts(),
-                                            eng.get_fourier_locations(),
-                                            nb_dof_per_pixel, input_array);
-            auto & output_field{
-                eng.fetch_or_register_real_space_field(
-                    "ifft return buffer",
-                    input_proxy.get_components_shape())};
+            auto nb_dof_per_pixel{std::accumulate(info.shape.begin(),
+                                                  info.shape.end() - dim, 1,
+                                                  std::multiplies<Index_t>())};
+            NumpyProxy<Complex> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_fourier_grid_pts(),
+                eng.get_fourier_locations(), nb_dof_per_pixel, input_array);
+            auto & output_field{eng.real_space_field(
+                "ifft return buffer", input_proxy.get_components_shape())};
             eng.ifft(input_proxy.get_field(), output_field);
             return numpy_wrap(output_field, IterUnit::Pixel);
           },
           "fourier_input_array"_a,
           "Perform inverse FFT of the input array into the output array.")
       .def(
           "hcfft",
-          [](Engine & eng,
-             py::array_t<Real> & input_array,
+          [](Engine & eng, py::array_t<Real> & input_array,
              py::array_t<Real> & output_array) {
             auto nb_dof_per_pixel{input_array.size() / eng.size()};
-            NumpyProxy<Real> input_proxy(eng.get_nb_domain_grid_pts(),
-                                         eng.get_nb_subdomain_grid_pts(),
-                                         eng.get_subdomain_locations(),
-                                         nb_dof_per_pixel, input_array);
-            NumpyProxy<Real> output_proxy(eng.get_nb_domain_grid_pts(),
-                                          eng.get_nb_subdomain_grid_pts(),
-                                          eng.get_subdomain_locations(),
-                                          nb_dof_per_pixel, output_array);
+            NumpyProxy<Real> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, input_array);
+            NumpyProxy<Real> output_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, output_array);
             auto && input_proxy_field{input_proxy.get_field()};
             eng.hcfft(input_proxy_field, output_proxy.get_field());
           },
           "real_input_array"_a, "real_output_array"_a,
           "Perform forward FFT of the input array into the output array")
       .def(
           "ihcfft",
-          [](Engine & eng,
-             py::array_t<Real> & input_array,
+          [](Engine & eng, py::array_t<Real> & input_array,
              py::array_t<Real> & output_array) {
             auto nb_dof_per_pixel{output_array.size() / eng.size()};
-            NumpyProxy<Real> input_proxy(eng.get_nb_domain_grid_pts(),
-                                         eng.get_nb_subdomain_grid_pts(),
-                                         eng.get_subdomain_locations(),
-                                         nb_dof_per_pixel, input_array);
-            NumpyProxy<Real> output_proxy(eng.get_nb_domain_grid_pts(),
-                                          eng.get_nb_subdomain_grid_pts(),
-                                          eng.get_subdomain_locations(),
-                                          nb_dof_per_pixel, output_array);
+            NumpyProxy<Real> input_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, input_array);
+            NumpyProxy<Real> output_proxy(
+                eng.get_nb_domain_grid_pts(), eng.get_nb_subdomain_grid_pts(),
+                eng.get_subdomain_locations(), nb_dof_per_pixel, output_array);
             eng.ihcfft(input_proxy.get_field(), output_proxy.get_field());
           },
           "real_input_array"_a, "real_output_array"_a,
           "Perform inverse FFT of the input array into the output array.");
 }
 
 void add_fft_engines(py::module & mod) {
```

### Comparing `mufft-0.90.0/language_bindings/python/bind_py_module.cc` & `mufft-0.91.0/language_bindings/python/bind_py_module.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/muFFT/Stencils1D.py` & `mufft-0.91.0/language_bindings/python/muFFT/Stencils1D.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/muFFT/Stencils2D.py` & `mufft-0.91.0/language_bindings/python/muFFT/Stencils2D.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/muFFT/Stencils3D.py` & `mufft-0.91.0/language_bindings/python/muFFT/Stencils3D.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/language_bindings/python/muFFT/__init__.py` & `mufft-0.91.0/language_bindings/python/muFFT/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
     """
     Exception used to indicate and unknown FFT engine identifier.
     """
     pass
 
 
 # This is a list of FFT engines that are potentially available.
-#              |--------------------------------- String identifier for 'FFT' class
-#              |             |------------------- Name of engine class
-#              |             |          |-------- Is output transposed?
-#              v             v          v      v- Supports MPI parallel calculations?
+#             |----------------------------------- String identifier for 'FFT' class
+#             |             |--------------------- Name of engine class
+#             |             |            |-------- Is output transposed?
+#             v             v            v      v- Supports MPI parallel calculations?
 _factories = {'pocketfft': ('PocketFFT', False, False),
               'fftw': ('FFTW', False, False),
               'fftwmpi': ('FFTWMPI', True, True),
               'pfft': ('PFFT', True, True)}
 
 
 # Detect FFT engines. This is a convenience dictionary that allows enumeration
@@ -86,105 +86,105 @@
             pass  # FFT engine is not compiled into the C++ code
     return fft_engines
 
 
 fft_engines = _find_fft_engines()
 
 
-def mangle_engine_identifier(fft, communicator=None):
+def mangle_engine_identifier(engine, communicator=None):
     """
     Return normalized engine identifier. This will turn 'serial' and 'mpi'
     engine identifiers into the respective best-performing engine compiled
     into the code.
 
     Parameters
     ----------
-    fft : string
+    engine : string
         FFT engine to use. Use 'mpi' if you want a parallel engine and 'serial'
         if you need a serial engine. It is also possible to specifically
         choose 'pocketfft', 'fftw', 'fftwmpi' or 'pfft'.
     communicator : mpi4py or muGrid communicator
         communicator object passed to parallel FFT engines. Note that
         the 'pocketfft' and 'fftw' engines do not support parallel execution.
         Default: None
     """
     communicator = Communicator(communicator)
-    if fft == 'mpi' and communicator.size == 1:
-        fft = 'serial'
-    if fft == 'serial':
+    if engine == 'mpi' and communicator.size == 1:
+        engine = 'serial'
+    if engine == 'serial':
         if 'fftw' in fft_engines:
             # Use FFTW for serial calculations if available since it is more
             # optimized than PocketFFT.
             return 'fftw', communicator
         else:
             return 'pocketfft', communicator
-    elif fft == 'mpi':
+    elif engine == 'mpi':
         if 'fftwmpi' in fft_engines:
             return 'fftwmpi', communicator
         elif 'pfft' in fft_engines:
             # This is a fallback in case there is not FFTWMPI. May not work
             # in all cases.
             return 'pfft', communicator
         else:
             raise RuntimeError('No MPI parallel FFT engine was compiled into the code.')
 
-    return fft, communicator
+    return engine, communicator
 
 
-def get_engine_factory(fft, communicator=None):
+def get_engine_factory(engine, communicator=None):
     """
     Get engine factory given factory string identifier.
 
     Parameters
     ----------
-    fft : string
+    engine : string
         FFT engine to use. Use 'mpi' if you want a parallel engine and 'serial'
         if you need a serial engine. It is also possible to specifically
         choose 'pocketfft', 'fftw', 'fftwmpi' or 'pfft'.
     communicator : mpi4py or muGrid communicator
         communicator object passed to parallel FFT engines. Note that
         the 'pocketfft' and 'fftw' engines do not support parallel execution.
         Default: None
     """
-    original_identifier = fft
-    fft, communicator = mangle_engine_identifier(fft, communicator)
+    original_identifier = engine
+    engine, communicator = mangle_engine_identifier(engine, communicator)
 
     try:
-        factory, is_transposed, is_parallel = fft_engines[fft]
+        factory, is_transposed, is_parallel = fft_engines[engine]
     except KeyError:
         factory = None
 
     if factory is None:
         raise UnknownFFTEngineError(
             "FFT engine with identifier '{}' (internally mangled to '{}') "
             "does not exist. If you believe this engine should exist, check "
             "that the code has been compiled with support for it."
-            .format(original_identifier, fft))
+            .format(original_identifier, engine))
 
     return factory, communicator
 
 
-def FFT(nb_grid_pts, fft='serial', communicator=None, **kwargs):
+def FFT(nb_grid_pts, engine='serial', communicator=None, **kwargs):
     """
     The FFT class handles forward and inverse transforms and instantiates
     the correct engine object to carry out the transform.
 
     The class holds the plan for the transform. It can only carry out
     transforms of the size specified upon instantiation. All transforms are
     real-to-complex. if
 
     Parameters
     ----------
     nb_grid_pts : list
         Grid nb_grid_pts in the Cartesian directions.
-    fft : string
+    engine : string
         FFT engine to use. Use 'mpi' if you want a parallel engine and 'serial'
         if you need a serial engine. It is also possible to specifically
         choose 'pocketfft', 'fftw', 'fftwmpi' or 'pfft'.
         Default: 'serial'.
     communicator : mpi4py or muGrid communicator
         communicator object passed to parallel FFT engines. Note that
         the 'pocketfft' and 'fftw' engines do not support parallel execution.
         Default: None
     """
-    factory, communicator = get_engine_factory(fft, communicator)
+    factory, communicator = get_engine_factory(engine, communicator)
     return factory(nb_grid_pts, communicator, **kwargs)
```

### Comparing `mufft-0.90.0/meson.build` & `mufft-0.91.0/meson.build`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,87 @@
 project(
     'muFFT', # Project name
     'c', 'cpp', # Project type. We need a C and C++ compiler.
     default_options : ['cpp_std=c++17'], # Yes, we need C++17, at least for std::optional
-    version: run_command('python3', 'discover_version.py', check: true).stdout().strip()
+    version : run_command('python3', 'discover_version.py', check : true).stdout().strip()
 )
 
 pymod = import('python')
 python = pymod.find_installation('python3',
-    required: true,
+                                 required : true,
 )
 
-version = run_command(python, 'discover_version.py', '--full', check: true).stdout().strip().split()
+version = run_command(python, 'discover_version.py', '--full', check : true).stdout().strip().split()
 version_dirty = version[0]
 version_str = version[1]
 version_hash = version[2]
 
 mufft_dependencies = []
 
-fftw3 = dependency('fftw3', required: false)
+fftw3 = dependency('fftw3', required : false)
 if fftw3.found()
-    message('muFFT FFTW: *** YES ***')
-    mu_with_fftw3 = true
     add_project_arguments('-DWITH_FFTW', language : ['c', 'cpp'])
     mufft_dependencies += [fftw3]
-else
-    message('muFFT FFTW: no')
-    mu_with_fftw3 = false
 endif
 
 # Those are requirements on *some* systems, hence optional
 cc = meson.get_compiler('c')
 #dl = cc.find_library('dl', required: false)
 #execinfo = cc.find_library('execinfo', required: false)
 
 #muspectre_dependencies = [dl, execinfo, fftw3]
 
 # This produces lots of Warning from Eigen3. Disabling for now.
 # add_project_arguments('-Weffc++', language: 'cpp')
 
-mpi = dependency('mpi', language: 'cpp', required: false)
+mpi = dependency('mpi', language : 'cpp', required : false)
 mu_with_mpi = false
 if mpi.found()
     fftw3mpi = cc.find_library(
         'fftw3_mpi',
-        dirs: ['/usr/lib', '/usr/lib/x86_64-linux-gnu'],
-        required: false)
-    if fftw3mpi.found() and cc.has_header('fftw3-mpi.h')
-        message('muFFT FFTW3 MPI: *** YES ***')
-        mu_with_fftw3mpi = true
+        dirs : ['/usr/lib', '/usr/lib/x86_64-linux-gnu'],
+        has_headers : ['fftw3-mpi.h'],
+        required : false)
+    if fftw3mpi.found()
         add_project_arguments('-DWITH_FFTWMPI', language : ['c', 'cpp'])
         mufft_dependencies += [fftw3mpi]
-    else
-        message('muFFT FFTW3 MPI: no')
-        mu_with_fftw3mpi = false
     endif
-    pfft = cc.find_library('pfft', required: false)
-    if pfft.found() and cc.has_header('pfft.h')
-        message('muFFT PFFT: *** YES ***')
-        mu_with_pfft = true
+    pfft = cc.find_library(
+        'pfft',
+        dirs : ['/usr/lib', '/usr/lib/x86_64-linux-gnu'],
+        has_headers : ['pfft.h'],
+        required : false)
+    if pfft.found()
         add_project_arguments('-DWITH_PFFT', language : ['c', 'cpp'])
         mufft_dependencies += [pfft]
-    else
-        message('muFFT PFFT: no')
-        mu_with_pfft = false
     endif
-    if mu_with_fftw3mpi or mu_with_pfft
+    if fftw3mpi.found() or pfft.found()
         mu_with_mpi = true  # We found MPI and a parallel FFT library
         mpi_processes = ['1', '2']  # MPI processes to use for parallel tests
     endif
 
-    message('muFFT MPI: *** YES ***')
     add_project_arguments('-DWITH_MPI', language : ['c', 'cpp'])
     mufft_dependencies += [mpi]
-else
-    message('muFFT MPI: no')
-    mu_with_fftw3mpi = false
-    mu_with_pfft = false
 endif
 
-eigen3 = dependency('eigen3', required: true)
-mugrid = dependency('mugrid', required: true)
+eigen3 = dependency('eigen3', required : true)
+mugrid = dependency('mugrid', required : true)
 mufft_dependencies += [eigen3, mugrid]
 
+message('  -------------------')
+message('  muFFT configuration')
+message('    MPI      : ' + (mpi.found() ? '*** YES ***' : 'no'))
+message('    pocketfft: *** YES ***')
+message('    FFTW3    : ' + (fftw3.found() ? '*** YES ***' : 'no'))
+if mpi.found()
+    message('    FFTW3 MPI: ' + (fftw3mpi.found() ? '*** YES ***' : 'no'))
+    message('    PFFT     : ' + (pfft.found() ? '*** YES ***' : 'no'))
+endif
+message('  -------------------')
+
 subdir('src')
 subdir('language_bindings')
 
 test_timeout = 300  # timeout in seconds for long running tests
 
 subdir('tests')
+subdir('examples')
```

### Comparing `mufft-0.90.0/pyproject.toml` & `mufft-0.91.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [build-system]
 requires = ["meson>=1.0.0", "meson-python>=0.15.0", "ninja", "numpy>=1.20.0"]
 build-backend = "mesonpy"
 
 [project]
 name = "muFFT"
-description = "µFFT is a unified interface to various FFT libraries"
+description = "Unified interface to MPI-parallel FFT libraries"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Ali Falsafi", email = "ali.falsafi@epfl.ch" },
     { name = "Till Junge", email = "till.junge@altermail.ch" },
     { name = "Richard Leute", email = "richard.leute@imtek.uni-freiburg.de" },
     { name = "Lars Pastewka", email = "lars.pastewka@imtek.uni-freiburg.de" }
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python"
 ]
-requires-python = ">=3.5.0"
+requires-python = ">=3.8.0"
 dynamic = [ "version" ]
 dependencies = [
+    "muGrid==0.91.1",
     "numpy"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov"
 ]
 
 [project.urls]
-documentation = "https://muspectre.gitlab.io/muspectre/index.html"
-repository = "https://gitlab.com/muspectre/muspectre"
-changelog = "https://gitlab.com/muspectre/muspectre/-/blob/master/CHANGELOG.md"
+documentation = "https://muspectre.github.io/muFFT/"
+repository = "https://github.com/muSpectre/muFFT"
+changelog = "https://github.com/muSpectre/muFFT/blob/main/CHANGELOG.md"
 
 [[tool.cibuildwheel.overrides]]
 select = "*manylinux*"
 # Build static NetCDF library
 before-all = [
     "NETCDF_VERSION='4.9.0'",
     "curl -L https://github.com/Unidata/netcdf-c/archive/refs/tags/v${NETCDF_VERSION}.tar.gz | tar -xzC /tmp",
@@ -48,8 +49,8 @@
     "rm -rf /tmp/build-netcdf /tmp/netcdf-c-${NETCDF_VERSION}"
 ]
 
 [[tool.cibuildwheel.overrides]]
 select = "*musllinux*"
 before-all = [
     "apk add libexecinfo libexecinfo-dev"
-]
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mufft-0.90.0/src/libmufft/derivative.cc` & `mufft-0.91.0/src/libmufft/derivative.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/src/libmufft/fft_engine_base.cc` & `mufft-0.91.0/src/libmufft/fft_engine_base.cc`

 * *Files 2% similar despite different names*

```diff
@@ -128,44 +128,44 @@
     bool output_copy_necessary{!this->check_fourier_space_field(output_field)};
     if (this->allow_temporary_buffer and
         (input_copy_necessary or output_copy_necessary)) {
       if (input_copy_necessary and output_copy_necessary) {
         std::stringstream iname, oname;
         iname << "temp_real_space_" << input_field.get_nb_dof_per_pixel();
         oname << "temp_fourier_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ifield{this->real_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
-        FourierField_t & tmp_ofield{this->fetch_or_register_fourier_space_field(
+        FourierField_t & tmp_ofield{this->fourier_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_fft(tmp_ifield, tmp_ofield);
         output_field = tmp_ofield;
       } else if (input_copy_necessary) {
         std::stringstream iname;
         iname << "temp_real_space_" << input_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ifield{this->real_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
         this->compute_fft(tmp_ifield, output_field);
       } else {  // output_copy_necessary
         std::stringstream oname;
         oname << "temp_fourier_space_" << output_field.get_nb_dof_per_pixel();
-        FourierField_t & tmp_ofield{this->fetch_or_register_fourier_space_field(
+        FourierField_t & tmp_ofield{this->fourier_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_fft(input_field, tmp_ofield);
         output_field = tmp_ofield;
@@ -240,44 +240,44 @@
     bool output_copy_necessary{not this->check_real_space_field(output_field)};
     if (this->allow_temporary_buffer and
         (input_copy_necessary or output_copy_necessary)) {
       if (input_copy_necessary and output_copy_necessary) {
         std::stringstream iname, oname;
         iname << "temp_fourier_space_" << input_field.get_nb_dof_per_pixel();
         oname << "temp_real_space_" << output_field.get_nb_dof_per_pixel();
-        FourierField_t & tmp_ifield{this->fetch_or_register_fourier_space_field(
+        FourierField_t & tmp_ifield{this->fourier_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
-        RealField_t & tmp_ofield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ofield{this->real_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_ifft(tmp_ifield, tmp_ofield);
         output_field = tmp_ofield;
       } else if (input_copy_necessary) {
         std::stringstream iname;
         iname << "temp_fourier_space_" << input_field.get_nb_dof_per_pixel();
-        FourierField_t & tmp_ifield{this->fetch_or_register_fourier_space_field(
+        FourierField_t & tmp_ifield{this->fourier_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
         this->compute_ifft(tmp_ifield, output_field);
       } else {  // output_copy_necessary
         std::stringstream oname;
         oname << "temp_real_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ofield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ofield{this->real_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_ifft(input_field, tmp_ofield);
         output_field = tmp_ofield;
@@ -352,44 +352,44 @@
     bool output_copy_necessary{!this->check_halfcomplex_field(output_field)};
     if (this->allow_temporary_buffer and
         (input_copy_necessary or output_copy_necessary)) {
       if (input_copy_necessary and output_copy_necessary) {
         std::stringstream iname, oname;
         iname << "temp_real_space_" << input_field.get_nb_dof_per_pixel();
         oname << "temp_fourier_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ifield{this->real_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
-        RealField_t & tmp_ofield{this->fetch_or_register_halfcomplex_field(
+        RealField_t & tmp_ofield{this->halfcomplex_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_hcfft(tmp_ifield, tmp_ofield);
         output_field = tmp_ofield;
       } else if (input_copy_necessary) {
         std::stringstream iname;
         iname << "temp_real_space_" << input_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ifield{this->real_space_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
         this->compute_hcfft(tmp_ifield, output_field);
       } else {  // output_copy_necessary
         std::stringstream oname;
         oname << "temp_fourier_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ofield{this->fetch_or_register_halfcomplex_field(
+        RealField_t & tmp_ofield{this->halfcomplex_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_hcfft(input_field, tmp_ofield);
         output_field = tmp_ofield;
@@ -464,44 +464,44 @@
     bool output_copy_necessary{not this->check_real_space_field(output_field)};
     if (this->allow_temporary_buffer and
         (input_copy_necessary or output_copy_necessary)) {
       if (input_copy_necessary and output_copy_necessary) {
         std::stringstream iname, oname;
         iname << "temp_fourier_space_" << input_field.get_nb_dof_per_pixel();
         oname << "temp_real_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_halfcomplex_field(
+        RealField_t & tmp_ifield{this->halfcomplex_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
-        RealField_t & tmp_ofield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ofield{this->real_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_ihcfft(tmp_ifield, tmp_ofield);
         output_field = tmp_ofield;
       } else if (input_copy_necessary) {
         std::stringstream iname;
         iname << "temp_fourier_space_" << input_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ifield{this->fetch_or_register_halfcomplex_field(
+        RealField_t & tmp_ifield{this->halfcomplex_field(
             iname.str(), input_field.get_nb_dof_per_pixel())};
         tmp_ifield.get_collection().set_nb_sub_pts(
             input_field.get_sub_division_tag(), input_field.get_nb_sub_pts());
         tmp_ifield.reshape(input_field.get_components_shape(),
                            input_field.get_sub_division_tag());
         tmp_ifield = input_field;
         this->compute_ihcfft(tmp_ifield, output_field);
       } else {  // output_copy_necessary
         std::stringstream oname;
         oname << "temp_real_space_" << output_field.get_nb_dof_per_pixel();
-        RealField_t & tmp_ofield{this->fetch_or_register_real_space_field(
+        RealField_t & tmp_ofield{this->real_space_field(
             oname.str(), output_field.get_nb_dof_per_pixel())};
         tmp_ofield.get_collection().set_nb_sub_pts(
             output_field.get_sub_division_tag(), output_field.get_nb_sub_pts());
         tmp_ofield.reshape(output_field.get_components_shape(),
                            output_field.get_sub_division_tag());
         this->compute_ihcfft(input_field, tmp_ofield);
         output_field = tmp_ofield;
@@ -518,36 +518,34 @@
                              "field and no temporary copies are allowed.");
       }
       this->compute_ihcfft(input_field, output_field);
     }
   }
 
   /* ---------------------------------------------------------------------- */
-  auto
-  FFTEngineBase::register_fourier_space_field(const std::string & unique_name,
-                                              const Index_t & nb_dof_per_pixel)
-      -> muGrid::ComplexField & {
+  auto FFTEngineBase::register_fourier_space_field(
+      const std::string & unique_name,
+      const Index_t & nb_dof_per_pixel) -> muGrid::ComplexField & {
     this->create_plan(nb_dof_per_pixel);
     return this->fourier_field_collection.register_complex_field(
         unique_name, nb_dof_per_pixel, PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto
-  FFTEngineBase::register_fourier_space_field(const std::string & unique_name,
-                                              const Shape_t & shape)
-      -> muGrid::ComplexField & {
+  auto FFTEngineBase::register_fourier_space_field(
+      const std::string & unique_name,
+      const Shape_t & shape) -> muGrid::ComplexField & {
     this->create_plan(shape);
     return this->fourier_field_collection.register_complex_field(
         unique_name, shape, PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_fourier_space_field(
-      const std::string & unique_name, const Index_t & nb_dof_per_pixel)
+  auto FFTEngineBase::fourier_space_field(const std::string & unique_name,
+                                          const Index_t & nb_dof_per_pixel)
       -> FourierField_t & {
     this->create_plan(nb_dof_per_pixel);
     if (this->fourier_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<FourierField_t &>(
           this->fourier_field_collection.get_field(unique_name))};
       if (field.get_nb_dof_per_pixel() != nb_dof_per_pixel) {
         std::stringstream message{};
@@ -559,16 +557,16 @@
       }
       return field;
     }
     return this->register_fourier_space_field(unique_name, nb_dof_per_pixel);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_fourier_space_field(
-      const std::string & unique_name, const Shape_t & shape)
+  auto FFTEngineBase::fourier_space_field(const std::string & unique_name,
+                                          const Shape_t & shape)
       -> FourierField_t & {
     this->create_plan(shape);
     if (this->fourier_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<FourierField_t &>(
           this->fourier_field_collection.get_field(unique_name))};
       if (field.get_components_shape() != shape) {
         std::stringstream message{};
@@ -578,34 +576,33 @@
         throw FFTEngineError{message.str()};
       }
       return field;
     }
     return this->register_fourier_space_field(unique_name, shape);
   }
 
-  auto
-  FFTEngineBase::register_halfcomplex_field(const std::string & unique_name,
-                                            const Index_t & nb_dof_per_pixel)
-      -> RealField_t & {
+  auto FFTEngineBase::register_halfcomplex_field(
+      const std::string & unique_name,
+      const Index_t & nb_dof_per_pixel) -> RealField_t & {
     this->create_plan(nb_dof_per_pixel);
     return this->halfcomplex_field_collection.register_real_field(
         unique_name, nb_dof_per_pixel, PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
   auto FFTEngineBase::register_halfcomplex_field(
       const std::string & unique_name, const Shape_t & shape) -> RealField_t & {
     this->create_plan(shape);
     return this->halfcomplex_field_collection.register_real_field(
         unique_name, shape, PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_halfcomplex_field(
-      const std::string & unique_name, const Index_t & nb_dof_per_pixel)
+  auto FFTEngineBase::halfcomplex_field(const std::string & unique_name,
+                                        const Index_t & nb_dof_per_pixel)
       -> RealField_t & {
     this->create_plan(nb_dof_per_pixel);
     if (this->halfcomplex_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<RealField_t &>(
           this->halfcomplex_field_collection.get_field(unique_name))};
       if (field.get_nb_dof_per_pixel() != nb_dof_per_pixel) {
         std::stringstream message{};
@@ -617,16 +614,17 @@
       }
       return field;
     }
     return this->register_halfcomplex_field(unique_name, nb_dof_per_pixel);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_halfcomplex_field(
-      const std::string & unique_name, const Shape_t & shape) -> RealField_t & {
+  auto
+  FFTEngineBase::halfcomplex_field(const std::string & unique_name,
+                                   const Shape_t & shape) -> RealField_t & {
     this->create_plan(shape);
     if (this->halfcomplex_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<RealField_t &>(
           this->halfcomplex_field_collection.get_field(unique_name))};
       if (field.get_components_shape() != shape) {
         std::stringstream message{};
         message << "Field '" << unique_name << "' exists, but it has shape of "
@@ -638,35 +636,33 @@
     }
     return this->register_halfcomplex_field(unique_name, shape);
   }
 
   /* ---------------------------------------------------------------------- */
 
   /* ---------------------------------------------------------------------- */
-  auto
-  FFTEngineBase::register_real_space_field(const std::string & unique_name,
-                                           const Index_t & nb_dof_per_pixel)
-      -> RealField_t & {
+  auto FFTEngineBase::register_real_space_field(
+      const std::string & unique_name,
+      const Index_t & nb_dof_per_pixel) -> RealField_t & {
     this->create_plan(nb_dof_per_pixel);
     return this->real_field_collection.register_real_field(
         unique_name, nb_dof_per_pixel, PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::register_real_space_field(const std::string & unique_name,
-                                                const Shape_t & shape)
-      -> RealField_t & {
+  auto FFTEngineBase::register_real_space_field(
+      const std::string & unique_name, const Shape_t & shape) -> RealField_t & {
     this->create_plan(shape);
     return this->real_field_collection.register_real_field(unique_name, shape,
                                                            PixelTag);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_real_space_field(
-      const std::string & unique_name, const Index_t & nb_dof_per_pixel)
+  auto FFTEngineBase::real_space_field(const std::string & unique_name,
+                                       const Index_t & nb_dof_per_pixel)
       -> RealField_t & {
     this->create_plan(nb_dof_per_pixel);
     if (this->real_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<RealField_t &>(
           this->real_field_collection.get_field(unique_name))};
       if (field.get_nb_dof_per_pixel() != nb_dof_per_pixel) {
         std::stringstream message{};
@@ -678,16 +674,16 @@
       }
       return field;
     }
     return this->register_real_space_field(unique_name, nb_dof_per_pixel);
   }
 
   /* ---------------------------------------------------------------------- */
-  auto FFTEngineBase::fetch_or_register_real_space_field(
-      const std::string & unique_name, const Shape_t & shape) -> RealField_t & {
+  auto FFTEngineBase::real_space_field(const std::string & unique_name,
+                                       const Shape_t & shape) -> RealField_t & {
     this->create_plan(shape);
     if (this->real_field_collection.field_exists(unique_name)) {
       auto & field{dynamic_cast<RealField_t &>(
           this->real_field_collection.get_field(unique_name))};
       if (field.get_components_shape() != shape) {
         std::stringstream message{};
         message << "Field '" << unique_name << "' exists, but it has shape of "
```

### Comparing `mufft-0.90.0/src/libmufft/fft_engine_base.hh` & `mufft-0.91.0/src/libmufft/fft_engine_base.hh`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,15 @@
 
   /**
    * base class for FFTEngine-related exceptions
    */
   class FFTEngineError : public RuntimeError {
    public:
     //! constructor
-    explicit FFTEngineError(const std::string & what)
-        : RuntimeError(what) {}
+    explicit FFTEngineError(const std::string & what) : RuntimeError(what) {}
     //! constructor
     explicit FFTEngineError(const char * what) : RuntimeError(what) {}
   };
 
   /**
    * Virtual base class for FFT engines. To be implemented by all
    * FFT_engine implementations.
@@ -86,22 +85,35 @@
      */
     using iterator = typename GFieldCollection_t::DynamicPixels::iterator;
 
     //! Default constructor
     FFTEngineBase() = delete;
 
     /**
-     * Constructor with the domain's number of grid points in each direction and
-     * the communicator
-     * @param nb_grid_pts number of grid points of the global grid
-     * @comm MPI communicator object
-     * @param allow_temporary_buffer allow the creation of temporary buffers
-     *        if the input buffer has the wrong memory layout
-     * @param allow_destroy_input allow that the input buffers are invalidated
-     *        during the FFT
+     * @brief Constructs an FFTEngineBase object with the specified parameters.
+     *
+     * This constructor initializes an FFTEngineBase object with the given
+     * number of grid points, communicator, FFT planner flags, and buffer
+     * options. The constructor does not perform any FFT computations; it merely
+     * sets up the object for future FFT operations.
+     *
+     * @param nb_grid_pts A DynCcoord_t object representing the number of grid
+     * points in each dimension of the global grid.
+     * @param comm An optional Communicator object for MPI communication.
+     * Defaults to an empty Communicator.
+     * @param plan_flags An optional FFT_PlanFlags object representing the FFT
+     * planner flags. Defaults to FFT_PlanFlags::estimate.
+     * @param allow_temporary_buffer An optional boolean flag indicating whether
+     * the creation of temporary buffers is allowed if the input buffer has the
+     * wrong memory layout. Defaults to true.
+     * @param allow_destroy_input An optional boolean flag indicating whether
+     * the input buffers can be invalidated during the FFT. Defaults to false.
+     * @param engine_has_rigid_memory_layout An optional boolean flag indicating
+     * whether the underlying FFT engine requires a fixed memory layout.
+     * Defaults to true.
      */
     FFTEngineBase(const DynCcoord_t & nb_grid_pts,
                   Communicator comm = Communicator(),
                   const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
                   bool allow_temporary_buffer = true,
                   bool allow_destroy_input = false,
                   bool engine_has_rigid_memory_layout = true);
@@ -168,65 +180,60 @@
                                  const Shape_t & shape);
 
     /**
      * Fetches a Fourier-space field with the ideal strides and dimensions for
      * this engine. If the field does not exist, it is created using
      * `register_fourier_space_field`.
      */
-    FourierField_t &
-    fetch_or_register_fourier_space_field(const std::string & unique_name,
-                                          const Index_t & nb_dof_per_pixel);
+    FourierField_t & fourier_space_field(const std::string & unique_name,
+                                         const Index_t & nb_dof_per_pixel);
 
     /**
      * Fetches a Fourier-space field with the ideal strides and dimensions for
      * this engine. If the field does not exist, it is created using
      * `register_fourier_space_field`.
      */
-    FourierField_t &
-    fetch_or_register_fourier_space_field(const std::string & unique_name,
-                                          const Shape_t & shape);
+    FourierField_t & fourier_space_field(const std::string & unique_name,
+                                         const Shape_t & shape);
 
     /**
      * Create a Fourier-space field with the ideal strides and dimensions for
      * this engine. Fields created this way are meant to be reused again and
      * again, and they will stay in the memory of the `muFFT::FFTEngineBase`'s
      * field collection until the engine is destroyed.
      */
     virtual RealField_t &
     register_halfcomplex_field(const std::string & unique_name,
-                                 const Index_t & nb_dof_per_pixel);
+                               const Index_t & nb_dof_per_pixel);
 
     /**
      * Create a Fourier-space field with the ideal strides and dimensions for
      * this engine. Fields created this way are meant to be reused again and
      * again, and they will stay in the memory of the `muFFT::FFTEngineBase`'s
      * field collection until the engine is destroyed.
      */
     virtual RealField_t &
     register_halfcomplex_field(const std::string & unique_name,
-                                 const Shape_t & shape);
+                               const Shape_t & shape);
 
     /**
      * Fetches a Fourier-space field with the ideal strides and dimensions for
      * this engine. If the field does not exist, it is created using
      * `register_fourier_space_field`.
      */
-    RealField_t &
-    fetch_or_register_halfcomplex_field(const std::string & unique_name,
-                                        const Index_t & nb_dof_per_pixel);
+    RealField_t & halfcomplex_field(const std::string & unique_name,
+                                    const Index_t & nb_dof_per_pixel);
 
     /**
      * Fetches a Fourier-space field with the ideal strides and dimensions for
      * this engine. If the field does not exist, it is created using
      * `register_fourier_space_field`.
      */
-    RealField_t &
-    fetch_or_register_halfcomplex_field(const std::string & unique_name,
-                                        const Shape_t & shape);
-
+    RealField_t & halfcomplex_field(const std::string & unique_name,
+                                    const Shape_t & shape);
 
     /**
      * Create a real-space field with the ideal strides and dimensions for this
      * engine. Fields created this way are meant to be reused again and again,
      * and they will stay in the memory of the `muFFT::FFTEngineBase`'s field
      * collection until the engine is destroyed.
      */
@@ -245,26 +252,24 @@
                               const Shape_t & shape);
 
     /**
      * Fetches a real-space field with the ideal strides and dimensions for this
      * engine. If the field does not exist, it is created using
      * `register_real_space_field`.
      */
-    RealField_t &
-    fetch_or_register_real_space_field(const std::string & unique_name,
-                                       const Index_t & nb_dof_per_pixel);
+    RealField_t & real_space_field(const std::string & unique_name,
+                                   const Index_t & nb_dof_per_pixel);
 
     /**
      * Fetches a real-space field with the ideal strides and dimensions for this
      * engine. If the field does not exist, it is created using
      * `register_real_space_field`.
      */
-    RealField_t &
-    fetch_or_register_real_space_field(const std::string & unique_name,
-                                       const Shape_t & shape);
+    RealField_t & real_space_field(const std::string & unique_name,
+                                   const Shape_t & shape);
 
     //! return whether this engine is active
     virtual bool has_grid_pts() const { return true; }
 
     /**
      * iterators over only those pixels that exist in real space
      */
@@ -323,15 +328,14 @@
       return this->fourier_locations;
     }
     //! returns the data layout of the cell in Fourier space
     const DynCcoord_t & get_fourier_strides() const {
       return this->fourier_strides;
     }
 
-
     //! returns the field collection handling fields in real space
     GFieldCollection_t & get_real_field_collection() {
       return this->real_field_collection;
     }
 
     //! returns the field collection handling fields confirming with
     // the data layout required for half-complex transforms
@@ -353,38 +357,36 @@
     //! loop), FFT engines provide this value so it can be used in the
     //! projection operator (where no additional loop is required)
     inline Real normalisation() const { return norm_factor; }
 
     //! return the number of spatial dimensions
     const Index_t & get_spatial_dim() const;
 
-
     //! perform a deep copy of the engine (this should never be necessary in
     //! c++)
     virtual std::unique_ptr<FFTEngineBase> clone() const = 0;
 
     //! check whether a plan for nb_dof_per_pixel exists
     bool has_plan_for(const Index_t & nb_dof_per_pixel) const;
 
-
    protected:
     //! calls initialize of the real, hc and fourier field collections
     void initialise_field_collections();
 
     //! forward transform, assumes that the buffer has the correct memory layout
     virtual void compute_fft(const RealField_t & input_field,
                              FourierField_t & output_field) = 0;
 
     //! inverse transform, assumes that the buffer has the correct memory layout
     virtual void compute_ifft(const FourierField_t & input_field,
                               RealField_t & output_field) = 0;
 
     //! forward half complex transform
     virtual void compute_hcfft(const RealField_t & input_field,
-                                RealField_t & output_field);
+                               RealField_t & output_field);
 
     //! inverse half complex transform
     virtual void compute_ihcfft(const RealField_t & input_field,
                                 RealField_t & output_field);
 
     //! check whether real-space buffer has the correct memory layout
     virtual bool check_real_space_field(const RealField_t & field) const;
@@ -412,44 +414,44 @@
     //! In serial the hc_field is identical to the real field,
     //! But in parallel, the hc_field has no padding region.
     GFieldCollection_t halfcomplex_field_collection;
 
     //! nb_grid_pts of the full domain of the cell
     const DynCcoord_t nb_domain_grid_pts;
 
-    //!< nb_grid_pts of the process-local (subdomain) portion of the cell
+    //! nb_grid_pts of the process-local (subdomain) portion of the cell
     DynCcoord_t nb_subdomain_grid_pts;
-    //!< location of the process-local (subdomain) portion of the cell
+    //! location of the process-local (subdomain) portion of the cell
     DynCcoord_t subdomain_locations;
-    //!< data layout of the porcess-local portion of the cell
+    //! data layout of the porcess-local portion of the cell
     DynCcoord_t subdomain_strides;
-    //!< nb_grid_pts of the process-local (subdomain) portion of the Fourier
-    //!< transformed data
+    //! nb_grid_pts of the process-local (subdomain) portion of the Fourier
+    //! transformed data
     DynCcoord_t nb_fourier_grid_pts;
-    //!< location of the process-local (subdomain) portion of the Fourier
-    //!< transformed data
+    //! location of the process-local (subdomain) portion of the Fourier
+    //! transformed data
     DynCcoord_t fourier_locations;
-    //!< data layout of the process-local (subdomain) portion of the Fourier
-    //!< transformed data
+    //! data layout of the process-local (subdomain) portion of the Fourier
+    //! transformed data
     DynCcoord_t fourier_strides;
 
     //! allow the FFTEngine to create temporary copies (if it cannot work with
     //! a specific memory layout)
     bool allow_temporary_buffer;
 
     //! allow the FFTEngine to destroy input buffers
     bool allow_destroy_input;
 
     //! the underlying FFT engine requires a fixed memory layout
     bool engine_has_rigid_memory_layout;
 
-    //!< normalisation coefficient of fourier transform
+    //! normalisation coefficient of fourier transform
     const Real norm_factor;
 
-    //!< FFT planner flags
+    //! FFT planner flags
     const FFT_PlanFlags plan_flags;
 
     //! number of degrees of freedom per pixel for which this field collection
     //! has been primed. Can be queried. Corresponds to the number of sub-points
     //! per pixel multiplied by the number of components per sub-point
     std::set<Index_t> planned_nb_dofs{};
   };
```

### Comparing `mufft-0.90.0/src/libmufft/fft_utils.cc` & `mufft-0.91.0/src/libmufft/fft_utils.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/src/libmufft/fftw_engine.cc` & `mufft-0.91.0/src/libmufft/fftw_engine.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/src/libmufft/fftw_engine.hh` & `mufft-0.91.0/src/libmufft/pfft_engine.hh`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-
 /**
- * @file   fftw_engine.hh
+ * @file   pfft_engine.hh
  *
- * @author Till Junge <till.junge@altermail.ch>
+ * @author Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
  *
- * @date   03 Dec 2017
+ * @date   06 Mar 2017
  *
- * @brief  FFT engine using FFTW
+ * @brief  FFT engine using MPI-parallel PFFT
  *
  * Copyright © 2017 Till Junge
  *
  * µFFT is free software; you can redistribute it and/or
  * modify it under the terms of the GNU Lesser General Public License as
  * published by the Free Software Foundation, either version 3, or (at
  * your option) any later version.
@@ -30,116 +29,127 @@
  * If you modify this Program, or any covered work, by linking or combining it
  * with proprietary FFT implementations or numerical libraries, containing parts
  * covered by the terms of those libraries' licenses, the licensors of this
  * Program grant you additional permission to convey the resulting work.
  *
  */
 
-#ifndef SRC_LIBMUFFT_FFTW_ENGINE_HH_
-#define SRC_LIBMUFFT_FFTW_ENGINE_HH_
+#ifndef SRC_LIBMUFFT_PFFT_ENGINE_HH_
+#define SRC_LIBMUFFT_PFFT_ENGINE_HH_
 
 #include "fft_engine_base.hh"
 
-#include <fftw3.h>
+#include <pfft.h>
 
 namespace muFFT {
 
   /**
-   * implements the `muFFT::FftEngine_Base` interface using the
+   * implements the `muFFT::FFTEngineBase` interface using the
    * FFTW library
    */
-  class FFTWEngine : public FFTEngineBase {
+  class PFFTEngine : public FFTEngineBase {
    public:
     using Parent = FFTEngineBase;  //!< base class
     //! field for Fourier transform of second-order tensor
     using FourierField_t = typename Parent::FourierField_t;
     //! real-valued second-order tensor
     using RealField_t = typename Parent::RealField_t;
     //! Default constructor
-    FFTWEngine() = delete;
+    PFFTEngine() = delete;
 
     /**
-     * Constructor with the domain's number of grid points in each direction,
-     * the communicator, and fft planner flags
+     * Constructor with the domain's number of grid points in each direction and
+     * the communicator
      * @param nb_grid_pts number of grid points of the global grid
+     * @param comm MPI communicator object
+     * @param plan_flags MPI planner flags
      * @param allow_temporary_buffer allow the creation of temporary buffers
      *        if the input buffer has the wrong memory layout
      * @param allow_destroy_input allow that the input buffers are invalidated
      *        during the FFT
-     * @comm MPI communicator object
      */
-    FFTWEngine(const DynCcoord_t & nb_grid_pts,
+    PFFTEngine(const DynCcoord_t & nb_grid_pts,
                Communicator comm = Communicator(),
                const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
                bool allow_temporary_buffer = true,
                bool allow_destroy_input = false);
-    /**
-     * Constructor with the domain's number of grid points in each direction and
-     * the fft planner flags
-     * @param nb_grid_pts number of grid points of the global grid
-     * @param allow_temporary_buffer allow the creation of temporary buffers
-     *        if the input buffer has the wrong memory layout
-     * @param allow_destroy_input allow that the input buffers are invalidated
-     *        during the FFT
-     * @comm MPI communicator object
-     */
-    FFTWEngine(const DynCcoord_t & nb_grid_pts,
-               const FFT_PlanFlags & plan_flags,
-               bool allow_temporary_buffer = true,
-               bool allow_destroy_input = false);
 
     //! Copy constructor
-    FFTWEngine(const FFTWEngine & other) = delete;
+    PFFTEngine(const PFFTEngine & other) = delete;
 
     //! Move constructor
-    FFTWEngine(FFTWEngine && other) = delete;
+    PFFTEngine(PFFTEngine && other) = delete;
 
     //! Destructor
-    virtual ~FFTWEngine() noexcept;
+    virtual ~PFFTEngine() noexcept;
 
     //! Copy assignment operator
-    FFTWEngine & operator=(const FFTWEngine & other) = delete;
+    PFFTEngine & operator=(const PFFTEngine & other) = delete;
 
     //! Move assignment operator
-    FFTWEngine & operator=(FFTWEngine && other) = delete;
+    PFFTEngine & operator=(PFFTEngine && other) = default;
 
     // compute the plan, etc
     void create_plan(const Index_t & nb_dof_per_pixel) override;
 
     //! perform a deep copy of the engine (this should never be necessary in
     //! c++)
     std::unique_ptr<FFTEngineBase> clone() const final;
 
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Index_t & nb_dof_per_pixel) final;
+
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    RealField_t &
+    register_real_space_field(const std::string & unique_name,
+                              const Shape_t & shape) final;
+
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    muGrid::ComplexField &
+    register_fourier_space_field(const std::string & unique_name,
+                                 const Index_t & nb_dof_per_pixel) final;
+
+    /**
+     * need to override this method here, since FFTWMPI requires field padding
+     */
+    muGrid::ComplexField &
+    register_fourier_space_field(const std::string & unique_name,
+                                 const Shape_t & shape) final;
+
    protected:
     //! forward transform
-    void compute_fft(const RealField_t & input_field,
+    void compute_fft(const RealField_t & field,
                      FourierField_t & output_field) override;
 
     //! inverse transform
     void compute_ifft(const FourierField_t & input_field,
                       RealField_t & output_field) override;
 
-    //! forward half complex transform
-    void compute_hcfft(const RealField_t & input_field,
-                 RealField_t & output_field) override;
+    //! check whether real-space buffer has the correct memory layout
+    bool check_real_space_field(const RealField_t & field) const final;
 
-    //! inverse half complex transform
-    void compute_ihcfft(const RealField_t & input_field,
-                      RealField_t & output_field) override;
+    //! check whether Fourier-space buffer has the correct memory layout
+    bool check_fourier_space_field(const FourierField_t & field) const final;
 
+    static int nb_engines;  //!< number of times this engine has
+                            //!< been instantiated
+    MPI_Comm mpi_comm;  //!< MPI communicator
     //! holds the plans for forward fourier transforms
-    std::map<Index_t, fftw_plan> fft_plans{};
+    std::map<Index_t, pfft_plan> fft_plans{};
     //! holds the plans for inversefourier transforms
-    std::map<Index_t, fftw_plan> ifft_plans{};
-
-    //! holds the plans for forward half-complex fourier transforms
-    std::map<Index_t, fftw_plan> hcfft_plans{};
-
-    //! holds the plans for inverse half-complex fourier transforms
-    std::map<Index_t, fftw_plan> ihcfft_plans{};
-
-    static Index_t nb_engines;
+    std::map<Index_t, pfft_plan> ifft_plans{};
+    //! holds the fourier field sizes including padding for different transforms
+    std::map<Index_t, Index_t> required_workspace_sizes{};
+    bool active{true};  //!< PFFT sometimes assigns zero grid points
   };
 
 }  // namespace muFFT
 
-#endif  // SRC_LIBMUFFT_FFTW_ENGINE_HH_
+#endif  // SRC_LIBMUFFT_PFFT_ENGINE_HH_
```

### Comparing `mufft-0.90.0/src/libmufft/fftwmpi_engine.cc` & `mufft-0.91.0/src/libmufft/fftwmpi_engine.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/src/libmufft/fftwmpi_engine.hh` & `mufft-0.91.0/src/libmufft/fftwmpi_engine.hh`

 * *Files 7% similar despite different names*

```diff
@@ -53,23 +53,32 @@
     using FourierField_t = typename Parent::FourierField_t;
     //! real-valued second-order tensor
     using RealField_t = typename Parent::RealField_t;
     //! Default constructor
     FFTWMPIEngine() = delete;
 
     /**
-     * Constructor with the domain's number of grid points in each direction and
-     * the communicator
-     * @param nb_grid_pts number of grid points of the global grid
-     * @param comm MPI communicator object
-     * @param plan_flags MPI planner flags
-     * @param allow_temporary_buffer allow the creation of temporary buffers
-     *        if the input buffer has the wrong memory layout
-     * @param allow_destroy_input allow that the input buffers are invalidated
-     *        during the FFT
+     * @brief Constructs a FFTWMPIEngine object with the specified parameters.
+     *
+     * This constructor initializes a FFTWMPIEngine object with the given number
+     * of grid points, communicator, FFT planner flags, and buffer options. The
+     * constructor does not perform any FFT computations; it merely sets up the
+     * object for future FFT operations.
+     *
+     * @param nb_grid_pts A DynCcoord_t object representing the number of grid
+     * points in each dimension of the global grid.
+     * @param comm An optional Communicator object for MPI communication.
+     * Defaults to an empty Communicator.
+     * @param plan_flags An optional FFT_PlanFlags object representing the FFT
+     * planner flags. Defaults to FFT_PlanFlags::estimate.
+     * @param allow_temporary_buffer An optional boolean flag indicating whether
+     * the creation of temporary buffers is allowed if the input buffer has the
+     * wrong memory layout. Defaults to true.
+     * @param allow_destroy_input An optional boolean flag indicating whether
+     * the input buffers can be invalidated during the FFT. Defaults to false.
      */
     FFTWMPIEngine(const DynCcoord_t & nb_grid_pts,
                   Communicator comm = Communicator(),
                   const FFT_PlanFlags & plan_flags = FFT_PlanFlags::estimate,
                   bool allow_temporary_buffer = true,
                   bool allow_destroy_input = false);
 
@@ -107,17 +116,16 @@
     RealField_t &
     register_real_space_field(const std::string & unique_name,
                               const Index_t & nb_dof_per_pixel) final;
 
     /**
      * need to override this method here, since FFTWMPI requires field padding
      */
-    RealField_t &
-    register_real_space_field(const std::string & unique_name,
-                              const Shape_t & shape) final;
+    RealField_t & register_real_space_field(const std::string & unique_name,
+                                            const Shape_t & shape) final;
 
     /**
      * need to override this method here, since FFTWMPI requires field padding
      */
     muGrid::ComplexField &
     register_fourier_space_field(const std::string & unique_name,
                                  const Index_t & nb_dof_per_pixel) final;
```

### Comparing `mufft-0.90.0/src/libmufft/meson.build` & `mufft-0.91.0/src/libmufft/meson.build`

 * *Files 20% similar despite different names*

```diff
@@ -5,25 +5,27 @@
     'version.cc',
     'derivative.cc',
     'fft_engine_base.cc',
     'fft_utils.cc',
     'pocketfft_engine.cc'
 ]
 
-if mu_with_fftw3
+if fftw3.found()
     mufft_sources += ['fftw_engine.cc']
 endif
 
-if mu_with_fftw3mpi
-    mufft_sources += ['fftwmpi_engine.cc']
-endif
+if mpi.found()
+    if fftw3mpi.found()
+        mufft_sources += ['fftwmpi_engine.cc']
+    endif
 
-if mu_with_pfft
-    mufft_sources += ['pfft_engine.cc']
+    if pfft.found()
+        mufft_sources += ['pfft_engine.cc']
+    endif
 endif
 
 libmufft = shared_library(
     'muFFT',
     mufft_sources,
-    dependencies: [mufft_dependencies, pocketfft],
-    install: true  # needed, otherwise it is not copied to wheel
+    dependencies : [mufft_dependencies, pocketfft],
+    install : true  # needed, otherwise it is not copied to wheel
 )
```

### Comparing `mufft-0.90.0/src/libmufft/pfft_engine.cc` & `mufft-0.91.0/src/libmufft/pfft_engine.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/src/libmufft/pocketfft_engine.cc` & `mufft-0.91.0/src/libmufft/pocketfft_engine.cc`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 namespace muFFT {
 
   PocketFFTEngine::PocketFFTEngine(const DynCcoord_t & nb_grid_pts,
                                    Communicator comm,
                                    const FFT_PlanFlags & plan_flags,
                                    bool allow_temporary_buffer,
                                    bool allow_destroy_input)
-      : Parent{nb_grid_pts, comm, plan_flags, allow_temporary_buffer,
+      : Parent{nb_grid_pts,         comm, plan_flags, allow_temporary_buffer,
                allow_destroy_input, false} {
     this->initialise_field_collections();
   }
 
   /* ---------------------------------------------------------------------- */
   PocketFFTEngine::PocketFFTEngine(const DynCcoord_t & nb_grid_pts,
                                    const FFT_PlanFlags & plan_flags,
@@ -157,59 +157,47 @@
     // Resize sub-point strides
     sub_pt_input_strides.resize(nb_input_dof_dim);
     sub_pt_output_strides.resize(nb_output_dof_dim);
 
     if (nb_dim == 1) {
       // One dimensional transforms can be carried out directly
       for (Index_t i{0}; i < nb_dof; ++i) {
-        pocketfft::r2c(real_shape,
-                       pixel_input_strides,
-                       pixel_output_strides,
-                       0,
+        pocketfft::r2c(real_shape, pixel_input_strides, pixel_output_strides, 0,
                        pocketfft::FORWARD,  // forward transform
-                       input_field.data() +
-                           _get_offset(i, sub_pt_input_shape,
-                                       sub_pt_input_strides),
-                       output_field.data() +
-                           _get_offset(i, sub_pt_output_shape,
-                                       sub_pt_output_strides),
+                       input_field.data() + _get_offset(i, sub_pt_input_shape,
+                                                        sub_pt_input_strides),
+                       output_field.data() + _get_offset(i, sub_pt_output_shape,
+                                                         sub_pt_output_strides),
                        1.0);  // additional multiplicative factor
       }
     } else {
       // For n-dimensional transforms we need to carry out n-transforms in the
       // respective directions
-      FourierField_t & tmp_field{
-          this->fetch_or_register_fourier_space_field("pocketfft_tmp", 1)};
+      FourierField_t & tmp_field{this->fourier_space_field("pocketfft_tmp", 1)};
       pocketfft::stride_t tmp_strides{
           tmp_field.get_strides(muGrid::IterUnit::Pixel, sizeof(Complex))};
 
       // Prepare axes array -> 1, 2, 3, ..., nb_dim-1
       pocketfft::shape_t axes(nb_dim - 1);
       std::iota(axes.begin(), axes.end(), 1);
 
       // Loop over all components and sub-points and carry out transform
       for (Index_t i{0}; i < nb_dof; ++i) {
-        pocketfft::r2c(real_shape,
-                       pixel_input_strides,
-                       tmp_strides,
+        pocketfft::r2c(real_shape, pixel_input_strides, tmp_strides,
                        0,  // see comment above on Hermitian index
                        pocketfft::FORWARD,  // forward transform
-                       input_field.data() +
-                           _get_offset(i, sub_pt_input_shape,
-                                       sub_pt_input_strides),
+                       input_field.data() + _get_offset(i, sub_pt_input_shape,
+                                                        sub_pt_input_strides),
                        tmp_field.data(),
                        1.0);  // additional multiplicative factor
-        pocketfft::c2c(fourier_shape,
-                       tmp_strides,
-                       pixel_output_strides, axes,
+        pocketfft::c2c(fourier_shape, tmp_strides, pixel_output_strides, axes,
                        pocketfft::FORWARD,  // forward transform
                        tmp_field.data(),
-                       output_field.data() +
-                           _get_offset(i, sub_pt_output_shape,
-                                       sub_pt_output_strides),
+                       output_field.data() + _get_offset(i, sub_pt_output_shape,
+                                                         sub_pt_output_strides),
                        1.0);  // additional multiplicative factor
       }
     }
   }
 
   /* ---------------------------------------------------------------------- */
   void PocketFFTEngine::compute_ifft(const FourierField_t & input_field,
@@ -261,60 +249,48 @@
     // Resize sub-point strides
     sub_pt_input_strides.resize(nb_input_dof_dim);
     sub_pt_output_strides.resize(nb_output_dof_dim);
 
     if (nb_dim == 1) {
       // One dimensional transforms can be carried out directly
       for (Index_t i{0}; i < nb_dof; ++i) {
-        pocketfft::c2r(real_shape,
-                       pixel_input_strides,
-                       pixel_output_strides, 0,
+        pocketfft::c2r(real_shape, pixel_input_strides, pixel_output_strides, 0,
                        pocketfft::BACKWARD,  // backward transform
-                       input_field.data() +
-                           _get_offset(i, sub_pt_input_shape,
-                                       sub_pt_input_strides),
-                       output_field.data() +
-                           _get_offset(i, sub_pt_output_shape,
-                                       sub_pt_output_strides),
+                       input_field.data() + _get_offset(i, sub_pt_input_shape,
+                                                        sub_pt_input_strides),
+                       output_field.data() + _get_offset(i, sub_pt_output_shape,
+                                                         sub_pt_output_strides),
                        1.0);  // additional multiplicative factor
       }
     } else {
       // For n-dimensional transforms we need to carry out n-transforms in the
       // respective directions
-      FourierField_t & tmp_field{
-          this->fetch_or_register_fourier_space_field("pocketfft_tmp", 1)};
+      FourierField_t & tmp_field{this->fourier_space_field("pocketfft_tmp", 1)};
       pocketfft::stride_t tmp_strides{
           tmp_field.get_strides(muGrid::IterUnit::Pixel, sizeof(Complex))};
 
       // Prepare axes array -> 1, 2, 3, ..., nb_dim-1
       pocketfft::shape_t axes(nb_dim - 1);
       auto n{nb_dim - 1};
-      std::generate(axes.begin(), axes.end(), [&n]{ return n--;});
+      std::generate(axes.begin(), axes.end(), [&n] { return n--; });
 
       // Loop over all components and sub-points and carry out transform
       for (Index_t i{0}; i < nb_dof; ++i) {
-        pocketfft::c2c(fourier_shape,
-                       pixel_input_strides,
-                       tmp_strides,
-                       axes,
+        pocketfft::c2c(fourier_shape, pixel_input_strides, tmp_strides, axes,
                        pocketfft::BACKWARD,  // backward transform
-                       input_field.data() +
-                           _get_offset(i, sub_pt_input_shape,
-                                       sub_pt_input_strides),
+                       input_field.data() + _get_offset(i, sub_pt_input_shape,
+                                                        sub_pt_input_strides),
                        tmp_field.data(),
                        1.0);  // additional multiplicative factor
-        pocketfft::c2r(real_shape,
-                       tmp_strides,
-                       pixel_output_strides,
+        pocketfft::c2r(real_shape, tmp_strides, pixel_output_strides,
                        0,  // see comment above on Hermitian index
                        pocketfft::BACKWARD,  // backward transform
                        tmp_field.data(),
-                       output_field.data() +
-                           _get_offset(i, sub_pt_output_shape,
-                                       sub_pt_output_strides),
+                       output_field.data() + _get_offset(i, sub_pt_output_shape,
+                                                         sub_pt_output_strides),
                        1.0);  // additional multiplicative factor
       }
     }
   }
 
   /* ---------------------------------------------------------------------- */
   std::unique_ptr<FFTEngineBase> PocketFFTEngine::clone() const {
```

### Comparing `mufft-0.90.0/src/libmufft/version.cc` & `mufft-0.91.0/src/libmufft/version.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/subprojects/eigen.wrap` & `mufft-0.91.0/subprojects/eigen.wrap`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/subprojects/pocketfft/LICENSE.md` & `mufft-0.91.0/subprojects/pocketfft/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/subprojects/pocketfft/README.md` & `mufft-0.91.0/subprojects/pocketfft/README.md`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/subprojects/pocketfft/pocketfft_hdronly.h` & `mufft-0.91.0/subprojects/pocketfft/pocketfft_hdronly.h`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 Copyright (C) 2010-2022 Max-Planck-Society
 Copyright (C) 2019-2020 Peter Bell
 
 For the odd-sized DCT-IV transforms:
   Copyright (C) 2003, 2007-14 Matteo Frigo
   Copyright (C) 2003, 2007-14 Massachusetts Institute of Technology
+  
+For the prev_good_size search:
+  Copyright (C) 2024 Tan Ping Liang, Peter Bell
 
 Authors: Martin Reinecke, Peter Bell
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -39,15 +42,15 @@
 #ifndef POCKETFFT_HDRONLY_H
 #define POCKETFFT_HDRONLY_H
 
 #ifndef __cplusplus
 #error This file is C++ and requires a C++ compiler.
 #endif
 
-#if !(__cplusplus >= 201103L || _MSVC_LANG+0L >= 201103L)
+#if !(__cplusplus >= 201103L || (defined(_MSVC_LANG) && _MSVC_LANG >= 201103L))
 #error This file requires at least C++11 support.
 #endif
 
 #ifndef POCKETFFT_CACHE_SIZE
 #define POCKETFFT_CACHE_SIZE 0
 #endif
 
@@ -145,20 +148,19 @@
 template<> struct VLEN<float> { static constexpr size_t val=4; };
 template<> struct VLEN<double> { static constexpr size_t val=2; };
 #else
 #define POCKETFFT_NO_VECTORS
 #endif
 #endif
 
-// the __MINGW32__ part in the conditional below works around the problem that
-// the standard C++ library on Windows does not provide aligned_alloc() even
-// though the MinGW compiler advertises C++17 compliance.
-// MSVC does not trigger this problem, since it apparently always sets
-// __cplusplus to 199711L ...
-#if (__cplusplus >= 201703L) && (!defined(__MINGW32__))
+// std::aligned_alloc is a bit cursed ... it doesn't exist on MacOS < 10.15
+// and in musl, and other OSes seem to have even more peculiarities.
+// Let's unconditionally work around it for now.
+# if 0
+//#if (__cplusplus >= 201703L) && (!defined(__MINGW32__)) && (!defined(_MSC_VER)) && (__MAC_OS_X_VERSION_MIN_REQUIRED >= MAC_OS_X_VERSION_10_15)
 inline void *aligned_alloc(size_t align, size_t size)
   {
   // aligned_alloc() requires that the requested size is a multiple of "align"
   void *ptr = ::aligned_alloc(align,(size+align-1)&(~(align-1)));
   if (!ptr) throw std::bad_alloc();
   return ptr;
   }
@@ -423,14 +425,23 @@
               }
             else
               return n;
             }
           }
     return bestfac;
     }
+  /* returns the smallest composite of 2, 3, 5, 7 and 11 which is >= n
+     and a multiple of required_factor. */
+  static POCKETFFT_NOINLINE size_t good_size_cmplx(size_t n,
+    size_t required_factor)
+    {
+    if (required_factor<1)
+      throw std::runtime_error("required factor must not be 0");
+    return good_size_cmplx((n+required_factor-1)/required_factor) * required_factor;
+    }
 
   /* returns the smallest composite of 2, 3, 5 which is >= n */
   static POCKETFFT_NOINLINE size_t good_size_real(size_t n)
     {
     if (n<=6) return n;
 
     size_t bestfac=2*n;
@@ -450,14 +461,71 @@
           }
         else
           return n;
         }
       }
     return bestfac;
     }
+  /* returns the smallest composite of 2, 3, 5 which is >= n
+     and a multiple of required_factor. */
+  static POCKETFFT_NOINLINE size_t good_size_real(size_t n,
+    size_t required_factor)
+    {
+    if (required_factor<1)
+      throw std::runtime_error("required factor must not be 0");
+    return good_size_real((n+required_factor-1)/required_factor) * required_factor;
+    }
+
+  /* returns the largest composite of 2, 3, 5, 7 and 11 which is <= n */
+  static POCKETFFT_NOINLINE size_t prev_good_size_cmplx(size_t n)
+  {
+    if (n<=12) return n;
+
+    size_t bestfound = 1;
+    for (size_t f11 = 1;f11 <= n; f11 *= 11)
+      for (size_t f117 = f11; f117 <= n; f117 *= 7)
+        for (size_t f1175 = f117; f1175 <= n; f1175 *= 5)
+        {
+          size_t x = f1175;
+          while (x*2 <= n) x *= 2;
+          if (x > bestfound) bestfound = x;
+          while (true) 
+          {
+            if (x * 3 <= n) x *= 3;
+            else if (x % 2 == 0) x /= 2;
+            else break;
+              
+            if (x > bestfound) bestfound = x;
+          }
+        }
+    return bestfound;
+  }
+
+  /* returns the largest composite of 2, 3, 5 which is <= n */
+  static POCKETFFT_NOINLINE size_t prev_good_size_real(size_t n)
+  {
+    if (n<=6) return n;
+
+    size_t bestfound = 1;
+    for (size_t f5 = 1; f5 <= n; f5 *= 5)
+    {
+      size_t x = f5;
+      while (x*2 <= n) x *= 2;
+      if (x > bestfound) bestfound = x;
+      while (true) 
+      {
+        if (x * 3 <= n) x *= 3;
+        else if (x % 2 == 0) x /= 2;
+        else break;
+      
+        if (x > bestfound) bestfound = x;
+      }
+    }
+    return bestfound;
+  }
 
   static size_t prod(const shape_t &shape)
     {
     size_t res=1;
     for (auto sz: shape)
       res*=sz;
     return res;
@@ -2631,19 +2699,21 @@
           c[k] = T0(0.5)*(t1+t2); c[kc]=T0(0.5)*(t1-t2);
           }
         if ((N&1)==0)
           c[NS2] *= twiddle[NS2-1];
         if (!cosine)
           for (size_t k=0, kc=N-1; k<kc; ++k, --kc)
             std::swap(c[k], c[kc]);
-        if (ortho) c[0]*=sqrt2*T0(0.5);
+        if (ortho)
+          cosine ? c[0]*=sqrt2*T0(0.5) : c[N-1]*=sqrt2*T0(0.5);
         }
       else
         {
-        if (ortho) c[0]*=sqrt2;
+        if (ortho)
+          cosine ? c[0]*=sqrt2 : c[N-1]*=sqrt2;
         if (!cosine)
           for (size_t k=0, kc=N-1; k<NS2; ++k, --kc)
             std::swap(c[k], c[kc]);
         for (size_t k=1, kc=N-1; k<NS2; ++k, --kc)
           {
           T t1=c[k]+c[kc], t2=c[k]-c[kc];
           c[k] = twiddle[k-1]*t2+twiddle[kc-1]*t1;
```

### Comparing `mufft-0.90.0/subprojects/pybind11.wrap` & `mufft-0.91.0/subprojects/pybind11.wrap`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/main_test_suite.cc` & `mufft-0.91.0/tests/main_test_suite.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/meson.build` & `mufft-0.91.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/mpi_context.hh` & `mufft-0.91.0/tests/mpi_context.hh`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/mpi_main_test_suite.cc` & `mufft-0.91.0/tests/mpi_main_test_suite.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/mpi_test_fft_engine.cc` & `mufft-0.91.0/tests/mpi_test_fft_engine.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/python_binding_tests.py` & `mufft-0.91.0/tests/python_binding_tests.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/python_derivative_tests.py` & `mufft-0.91.0/tests/python_derivative_tests.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/python_fft_tests.py` & `mufft-0.91.0/tests/python_fft_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,27 +72,27 @@
         for engine_str in self.engines:
             if muFFT.has_mpi:
                 # Check initialization with bare MPI communicator
                 from mpi4py import MPI
                 s = MPI.COMM_WORLD.Get_size()
                 try:
                     nb_dof = 6
-                    engine = muFFT.FFT([6 * s, 4 * s], fft=engine_str,
+                    engine = muFFT.FFT([6 * s, 4 * s], engine=engine_str,
                                        communicator=MPI.COMM_WORLD)
                     engine.create_plan(nb_dof)
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
             s = self.communicator.size
             nb_dof = 6
             try:
                 engine = muFFT.FFT([6 * s, 4 * s],
-                                   fft=engine_str,
+                                   engine=engine_str,
                                    communicator=self.communicator)
                 engine.create_plan(nb_dof)
             except muFFT.UnknownFFTEngineError:
                 # This FFT engine has not been compiled into the code. Skip
                 # test.
                 continue
 
@@ -106,25 +106,25 @@
                              comm.size * (comm.size + 1) / 2 + 3 * comm.size,
                              msg='{} engine'.format(engine_str))
 
     # Disable this test for now because it requires a lot of memory. This is
     # because it initializes the pixel_indices array, which is large.
     # def test_large_transform(self):
     #     for engine_str in self.engines:
-    #         muFFT.FFT([65536, 65536], fft=engine_str,
+    #         muFFT.FFT([65536, 65536], engine=engine_str,
     #                   communicator=self.communicator)
 
     def test_forward_transform_numpy_interface(self):
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 s = self.communicator.size
                 nb_grid_pts = s * np.array(nb_grid_pts)
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -157,15 +157,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 s = self.communicator.size
                 nb_grid_pts = list(s * np.array(nb_grid_pts))
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -205,15 +205,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 s = self.communicator.size
                 nb_grid_pts = s * np.array(nb_grid_pts)
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -255,15 +255,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 s = self.communicator.size
                 nb_grid_pts = list(s * np.array(nb_grid_pts))
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -308,15 +308,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 if np.prod(dims) != 1:
                     continue
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -341,15 +341,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 if np.prod(dims) != 1:
                     continue
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -392,15 +392,15 @@
         for engine_str in self.engines:
             for nb_grid_pts, dims in self.grids:
                 if np.prod(dims) != 1:
                     continue
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                     engine.create_plan(np.prod(dims))
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
@@ -429,15 +429,15 @@
                      'MPI parallel FFTs do not support 1D transforms')
     def test_1d_transform(self):
         for fft in ['pocketfft', 'fftw']:
             nb_grid_pts = [128, ]
 
             # Only serial engines support 1d transforms
             try:
-                engine = muFFT.FFT(nb_grid_pts, fft=fft)
+                engine = muFFT.FFT(nb_grid_pts, engine=fft)
             except muFFT.UnknownFFTEngineError:
                 # This FFT engine has not been compiled into the code. Skip
                 # test.
                 continue
 
             nb_dof = 1
             engine.create_plan(nb_dof)
@@ -463,15 +463,15 @@
                     continue
 
                 s = self.communicator.size
                 nb_grid_pts = list(s * np.array(nb_grid_pts))
 
                 try:
                     engine = muFFT.FFT(nb_grid_pts,
-                                       fft=engine_str,
+                                       engine=engine_str,
                                        communicator=self.communicator)
                 except muFFT.UnknownFFTEngineError:
                     # This FFT engine has not been compiled into the code. Skip
                     # test.
                     continue
 
                 freq = np.array(
@@ -482,16 +482,23 @@
                 assert np.allclose(engine.fftfreq, freq)
 
     def test_fftfreq(self):
         # Check that x and y directions are correct
         nb_grid_pts = [7, 4]
         nx, ny = nb_grid_pts
         nb_dof = 1
-        engine = muFFT.FFT(nb_grid_pts, fft='serial')
+        engine = muFFT.FFT(nb_grid_pts, engine='serial')
         engine.create_plan(nb_dof)
+
+        x, y = engine.coords
+        xref, yref = np.mgrid[0:nx, 0:ny]
+
+        np.testing.assert_allclose(x, xref / nx)
+        np.testing.assert_allclose(y, yref / ny)
+
         qx, qy = engine.fftfreq
 
         qarr = np.zeros(engine.nb_fourier_grid_pts, dtype=complex)
         qarr[np.logical_and(np.abs(np.abs(qx) * nx - 1) < 1e-6,
                             np.abs(np.abs(qy) * ny - 0) < 1e-6)] = 0.5
 
         rarr = np.zeros(nb_grid_pts, order='f')
@@ -510,15 +517,15 @@
         res = [2, 3]
         data = np.random.random(res)
         ref = np.fft.rfftn(data.T).T
         # Python will attempt to remove the muFFT.FFT temporary object here
         # right after the call to fft. However, since fft returns a pointer
         # to an *internal* buffer of the object, garbage collection should
         # be deferred until `tested` is destroyed.
-        engine = muFFT.FFT(res, fft="serial")
+        engine = muFFT.FFT(res, engine="serial")
         engine.create_plan(1)
         f_data = engine.register_fourier_space_field("fourier work space", 1)
         self.assertFalse(f_data.array().flags.owndata)
         engine.fft(data, f_data)
         tested = f_data.array()
         gc.collect()
         # It should not own the data, because it reference an internal buffer
@@ -527,15 +534,15 @@
         assert np.allclose(ref.imag, tested.imag)
 
     @unittest.skipIf(communicator.size > 1,
                      'This test only works on a single MPI process')
     def test_strides(self):
         for engine_str in self.engines:
             try:
-                engine = muFFT.FFT([3, 5, 7], fft=engine_str,
+                engine = muFFT.FFT([3, 5, 7], engine=engine_str,
                                    communicator=self.communicator)
                 engine.create_plan(1)
             except muFFT.UnknownFFTEngineError:
                 # This FFT engine has not been compiled into the code. Skip
                 # test.
                 continue
 
@@ -561,15 +568,15 @@
         """
         checks for exception of buffer has incompatible memory layout
         (FFTW only since PocketFFT can deal with any layout)
         """
         for fft in ['fftw']:
             try:
                 engine = muFFT.FFT([3, 2],
-                                   fft=fft, allow_temporary_buffer=False)
+                                   engine=fft, allow_temporary_buffer=False)
             except muFFT.UnknownFFTEngineError:
                 # This FFT engine has not been compiled into the code. Skip
                 # test.
                 continue
 
             engine.create_plan(1)
 
@@ -580,15 +587,15 @@
 
     def test_zero_grid_pts(self):
         nb_grid_pts = [3, 3]  # Gives one CPU with zero points on 4 processes
         axes = (0, 1)
 
         try:
             engine = muFFT.FFT(nb_grid_pts,
-                               fft='fftwmpi',
+                               engine='fftwmpi',
                                communicator=self.communicator)
             engine.create_plan(1)
         except muFFT.UnknownFFTEngineError:
             # This FFT engine has not been compiled into the code. Skip
             # test.
             return
 
@@ -632,15 +639,15 @@
             self.engines += ['pocketfft', 'fftw']
 
     @unittest.skipIf(communicator.size > 1,
                      'fftw only')
     def test_rffth2c_2d_sin(self):
 
         try:
-            engine = muFFT.FFT([5, 5], fft="fftw",
+            engine = muFFT.FFT([5, 5], engine="fftw",
                                allow_temporary_buffer=False,
                                allow_destroy_input=True)
         except muFFT.UnkownFFTEngineError:
             return
 
         in_data = np.cos(np.pi * 2 * np.arange(5) / 5).reshape(1, -1) * np.ones((5, 1))
         out_data = np.zeros((5, 5), dtype=float)
@@ -677,15 +684,15 @@
                      'fftw only')
     def test_rffth2c_2d_roundtrip(self):
 
         for nb_grid_pts in [(5, 5), (4, 4), (4, 5), (5, 4)]:
             nx, ny = nb_grid_pts
 
             try:
-                engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+                engine = muFFT.FFT(nb_grid_pts, engine="fftw",
                                    allow_temporary_buffer=False,
                                    allow_destroy_input=True)
             except muFFT.UnkownFFTEngineError:
                 return
 
             # Allocate buffers and create plan for one degree of freedom
             real_buffer = engine.register_halfcomplex_field(
@@ -704,15 +711,15 @@
     @unittest.skipIf(communicator.size > 1, 'fftw only')
     def test_rffth2c_2d_convenience_interface(self):
 
         nb_grid_pts = (5, 5)
         nx, ny = nb_grid_pts
 
         try:
-            engine = muFFT.FFT(nb_grid_pts, fft="fftw")
+            engine = muFFT.FFT(nb_grid_pts, engine="fftw")
         except muFFT.UnkownFFTEngineError:
             return
         engine.create_plan(1)
 
         original = np.random.normal(size=nb_grid_pts)
         original_backup = original.copy()
         result_real = np.empty(nb_grid_pts,
@@ -730,15 +737,15 @@
     @unittest.skipIf(communicator.size > 1, 'fftw only')
     def test_rffth2c_multiple_dofs(self):
         for nb_grid_pts, dims in self.grids:
             s = self.communicator.size
             nb_grid_pts = s * np.array(nb_grid_pts)
             try:
                 engine = muFFT.FFT(nb_grid_pts,
-                                   fft="fftw",
+                                   engine="fftw",
                                    communicator=self.communicator)
                 engine.create_plan(np.prod(dims))
             except muFFT.UnknownFFTEngineError:
                 # This FFT engine has not been compiled into the code. Skip
                 # test.
                 continue
 
@@ -771,15 +778,15 @@
 
     @unittest.skipIf(communicator.size > 1, 'fftw only')
     def test_rffth2c_1d_roundtrip(self):
 
         for nb_grid_pts in [(5,), (4,)]:
             nx, = nb_grid_pts
 
-            engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+            engine = muFFT.FFT(nb_grid_pts, engine="fftw",
                                allow_temporary_buffer=False,
                                allow_destroy_input=True)
 
             # Allocate buffers and create plan for one degree of freedom
             real_buffer = engine.register_halfcomplex_field(
                 "real-space", 1)
             fourier_buffer = engine.register_halfcomplex_field(
@@ -793,15 +800,15 @@
             real_buffer.array()[...] *= engine.normalisation
             np.testing.assert_allclose(real_buffer, original, atol=1e-14)
 
     @unittest.skipIf(communicator.size > 1, 'fftw only')
     def test_rffth2c_3d_roundtrip(self):
 
         for nb_grid_pts in [(5, 4, 5), (4, 5, 4), (4, 4, 5), (5, 5, 5), (4, 4, 4)]:
-            engine = muFFT.FFT(nb_grid_pts, fft="fftw",
+            engine = muFFT.FFT(nb_grid_pts, engine="fftw",
                                allow_temporary_buffer=False,
                                allow_destroy_input=True)
 
             # Allocate buffers and create plan for one degree of freedom
             real_buffer = engine.register_halfcomplex_field(
                 "real-space", 1)
             fourier_buffer = engine.register_halfcomplex_field(
@@ -816,15 +823,15 @@
             np.testing.assert_allclose(real_buffer, original, atol=1e-14)
 
     @unittest.skipIf(communicator.size > 1,
                      'This test only works on a single MPI process')
     def test_r2hc_incompatible_engines_raise(self):
         for engine in self.engines:
             try:
-                engine = muFFT.FFT([3, 5], fft=engine,
+                engine = muFFT.FFT([3, 5], engine=engine,
                                    allow_temporary_buffer=False,
                                    allow_destroy_input=True)
             except muFFT.UnknownFFTEngineError:  # One of the engines is not installed, skip it
                 continue
             # Allocate buffers and create plan for one degree of freedom
             real_buffer = engine.register_halfcomplex_field(
                 "real-space", 1)
```

### Comparing `mufft-0.90.0/tests/python_mpi_binding_tests.py` & `mufft-0.91.0/tests/python_mpi_binding_tests.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/python_muFFT_license_test.py` & `mufft-0.91.0/tests/python_muFFT_license_test.py`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/python_netcdf_tests.py` & `mufft-0.91.0/tests/python_netcdf_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     .reshape(self.tensor_shape)
 
                 if muFFT.has_mpi:
                     from mpi4py import MPI
                     self.communicator = MPI.COMM_WORLD
                 else:
                     self.communicator = None
-                self.fft = muFFT.FFT(self.nb_grid_pts, fft='mpi',
+                self.fft = muFFT.FFT(self.nb_grid_pts, engine='mpi',
                                      communicator=self.communicator)
 
             def test_write_read_domain(self):
                 if self.communicator is None:
                     nc = NCStructuredGrid('test_{}d.nc'.format(len(self.nb_grid_pts)), mode='w',
                                           nb_domain_grid_pts=self.nb_grid_pts)
                 else:
```

### Comparing `mufft-0.90.0/tests/test_fft_utils.cc` & `mufft-0.91.0/tests/test_fft_utils.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/test_serial_fft_engines.cc` & `mufft-0.91.0/tests/test_serial_fft_engines.cc`

 * *Files identical despite different names*

### Comparing `mufft-0.90.0/tests/tests.hh` & `mufft-0.91.0/tests/tests.hh`

 * *Files identical despite different names*

