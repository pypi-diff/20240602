# Comparing `tmp/mugrid-0.91.0.tar.gz` & `tmp/mugrid-0.91.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mugrid-0.91.0.tar", last modified: Sat Jun  1 21:12:48 2024, max compression
+gzip compressed data, was "mugrid-0.91.1.tar", last modified: Sun Jun  2 14:08:23 2024, max compression
```

## Comparing `mugrid-0.91.0.tar` & `mugrid-0.91.1.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0      195 2024-06-01 21:09:05.000000 mugrid-0.91.0/.clang-format
--rw-r--r--   0        0        0      148 2024-06-01 21:09:05.000000 mugrid-0.91.0/.gitattributes
--rw-r--r--   0        0        0      666 2024-06-01 21:09:05.000000 mugrid-0.91.0/.github/install_netcdf4.sh
--rw-r--r--   0        0        0     1552 2024-06-01 21:09:05.000000 mugrid-0.91.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1091 2024-06-01 21:09:05.000000 mugrid-0.91.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2454 2024-06-01 21:09:05.000000 mugrid-0.91.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     2131 2024-06-01 21:09:05.000000 mugrid-0.91.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       93 2024-06-01 21:09:05.000000 mugrid-0.91.0/.gitignore
--rw-r--r--   0        0        0      324 2024-06-01 21:09:05.000000 mugrid-0.91.0/.gitmodules
--rw-r--r--   0        0        0     7643 2024-06-01 21:09:05.000000 mugrid-0.91.0/CHANGELOG.md
--rw-r--r--   0        0        0      210 2024-06-01 21:09:05.000000 mugrid-0.91.0/CPPLINT.cfg
--rw-r--r--   0        0        0    35149 2024-06-01 21:09:05.000000 mugrid-0.91.0/LICENSE
--rw-r--r--   0        0        0     3031 2024-06-01 21:09:05.000000 mugrid-0.91.0/README.md
--rw-r--r--   0        0        0     5765 2024-06-01 21:09:05.000000 mugrid-0.91.0/discover_version.py
--rw-r--r--   0        0        0      726 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/Doxyfile
--rw-r--r--   0        0        0    94508 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/MainSchema.png
--rw-r--r--   0        0        0      608 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/Makefile
--rw-r--r--   0        0        0    58298 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/logo_flat.png
--rw-r--r--   0        0        0    37122 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/logo_square.png
--rw-r--r--   0        0        0       34 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/requirements.txt
--rw-r--r--   0        0        0   175699 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/CodingConvention.rst
--rw-r--r--   0        0        0    10682 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/Cplusplus.rst
--rw-r--r--   0        0        0       55 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/CplusplusAPI.rst
--rw-r--r--   0        0        0     3331 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/GettingStarted.rst
--rw-r--r--   0        0        0     8509 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/Python.rst
--rw-r--r--   0        0        0      983 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/Summary.rst
--rw-r--r--   0        0        0     6559 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/conf.py
--rw-r--r--   0        0        0     1031 2024-06-01 21:09:05.000000 mugrid-0.91.0/doc/source/index.rst
--rw-r--r--   0        0        0      337 2024-06-01 21:09:05.000000 mugrid-0.91.0/examples/components.py
--rw-r--r--   0        0        0      647 2024-06-01 21:09:05.000000 mugrid-0.91.0/examples/field_collection.py
--rw-r--r--   0        0        0      731 2024-06-01 21:09:05.000000 mugrid-0.91.0/examples/io.py
--rw-r--r--   0        0        0      644 2024-06-01 21:09:05.000000 mugrid-0.91.0/examples/meson.build
--rw-r--r--   0        0        0      595 2024-06-01 21:09:05.000000 mugrid-0.91.0/examples/sub_points.py
--rw-r--r--   0        0        0       16 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/meson.build
--rw-r--r--   0        0        0       56 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/__init__.py
--rw-r--r--   0        0        0     7281 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_common_mugrid.cc
--rw-r--r--   0        0        0     6000 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_communicator.cc
--rw-r--r--   0        0        0     1934 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_declarations.hh
--rw-r--r--   0        0        0     8343 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_field.cc
--rw-r--r--   0        0        0    25546 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_field_collection.cc
--rw-r--r--   0        0        0    13125 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_file_io.cc
--rw-r--r--   0        0        0     1706 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_module.cc
--rw-r--r--   0        0        0     6111 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_options_dictionary.cc
--rw-r--r--   0        0        0     3535 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/bind_py_state_field.cc
--rw-r--r--   0        0        0      512 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/meson.build
--rw-r--r--   0        0        0     3234 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/muGrid/Parallel.py
--rw-r--r--   0        0        0     2009 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/muGrid/__init__.py
--rw-r--r--   0        0        0      170 2024-06-01 21:09:05.000000 mugrid-0.91.0/language_bindings/python/muGrid/meson.build
--rw-r--r--   0        0        0     2139 2024-06-01 21:09:05.000000 mugrid-0.91.0/meson.build
--rw-r--r--   0        0        0     1874 2024-06-01 21:09:05.000000 mugrid-0.91.0/pyproject.toml
--rw-r--r--   0        0        0      114 2024-06-01 21:09:05.000000 mugrid-0.91.0/renovate.json
--rw-r--r--   0        0        0     4386 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/T4_map_proxy.hh
--rw-r--r--   0        0        0    11836 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/ccoord_operations.cc
--rw-r--r--   0        0        0    37927 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/ccoord_operations.hh
--rw-r--r--   0        0        0     1675 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/communicator.cc
--rw-r--r--   0        0        0    14105 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/communicator.hh
--rw-r--r--   0        0        0     7264 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/cpp_compliance.hh
--rw-r--r--   0        0        0    20115 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/eigen_tools.hh
--rw-r--r--   0        0        0     3156 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/exception.cc
--rw-r--r--   0        0        0    10912 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/exception.hh
--rw-r--r--   0        0        0    14731 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field.cc
--rw-r--r--   0        0        0    13078 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field.hh
--rw-r--r--   0        0        0    28663 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection.cc
--rw-r--r--   0        0        0    44908 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection.hh
--rw-r--r--   0        0        0     8208 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection_global.cc
--rw-r--r--   0        0        0    10942 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection_global.hh
--rw-r--r--   0        0        0     4298 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection_local.cc
--rw-r--r--   0        0        0     5045 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_collection_local.hh
--rw-r--r--   0        0        0    10753 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_map.cc
--rw-r--r--   0        0        0    14422 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_map.hh
--rw-r--r--   0        0        0    27124 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_map_static.hh
--rw-r--r--   0        0        0    30081 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_typed.cc
--rw-r--r--   0        0        0    25391 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/field_typed.hh
--rw-r--r--   0        0        0     4334 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/file_io_base.cc
--rw-r--r--   0        0        0    18299 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/file_io_base.hh
--rw-r--r--   0        0        0   136261 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/file_io_netcdf.cc
--rw-r--r--   0        0        0    68866 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/file_io_netcdf.hh
--rw-r--r--   0        0        0     5544 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/gradient_operator_base.hh
--rw-r--r--   0        0        0    15742 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/gradient_operator_default.cc
--rw-r--r--   0        0        0     8116 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/gradient_operator_default.hh
--rw-r--r--   0        0        0     3137 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/grid_common.cc
--rw-r--r--   0        0        0    28182 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/grid_common.hh
--rw-r--r--   0        0        0    12592 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/iterators.hh
--rw-r--r--   0        0        0    13401 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/mapped_field.hh
--rw-r--r--   0        0        0    10428 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/mapped_state_field.hh
--rw-r--r--   0        0        0     1115 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/meson.build
--rw-r--r--   0        0        0    19386 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/numpy_tools.hh
--rw-r--r--   0        0        0     3636 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/optional_mapped_field.hh
--rw-r--r--   0        0        0    11309 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/options_dictionary.cc
--rw-r--r--   0        0        0     6513 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/options_dictionary.hh
--rw-r--r--   0        0        0     4511 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/physics_domain.cc
--rw-r--r--   0        0        0     3630 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/physics_domain.hh
--rw-r--r--   0        0        0     1827 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/raw_memory_operations.cc
--rw-r--r--   0        0        0     5613 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/raw_memory_operations.hh
--rw-r--r--   0        0        0     3458 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/ref_array.hh
--rw-r--r--   0        0        0     3363 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/ref_vector.hh
--rw-r--r--   0        0        0     7857 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/state_field.cc
--rw-r--r--   0        0        0    12121 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/state_field.hh
--rw-r--r--   0        0        0     7284 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/state_field_map.cc
--rw-r--r--   0        0        0     8806 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/state_field_map.hh
--rw-r--r--   0        0        0    19738 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/state_field_map_static.hh
--rw-r--r--   0        0        0    22553 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/tensor_algebra.hh
--rw-r--r--   0        0        0    16900 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/units.cc
--rw-r--r--   0        0        0     9578 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/units.hh
--rw-r--r--   0        0        0     2484 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/libmugrid/version.cc.skeleton
--rw-r--r--   0        0        0      167 2024-06-01 21:09:05.000000 mugrid-0.91.0/src/meson.build
--rw-r--r--   0        0        0      590 2024-06-01 21:09:05.000000 mugrid-0.91.0/subprojects/eigen.wrap
--rw-r--r--   0        0        0      616 2024-06-01 21:09:05.000000 mugrid-0.91.0/subprojects/pybind11.wrap
--rw-r--r--   0        0        0     1654 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/field_test_fixtures.cc
--rw-r--r--   0        0        0     5370 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/field_test_fixtures.hh
--rw-r--r--   0        0        0     8857 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/header_test_ccoord_operations.cc
--rw-r--r--   0        0        0     4611 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/header_test_eigen_tools.cc
--rw-r--r--   0        0        0     1702 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/header_test_ref_array.cc
--rw-r--r--   0        0        0     7334 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/header_test_t4_map.cc
--rw-r--r--   0        0        0    11181 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/header_test_tensor_algebra.cc
--rw-r--r--   0        0        0     4983 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/io_mpi_test_file_io.hh
--rw-r--r--   0        0        0    22974 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/io_mpi_test_file_io_netcdf.cc
--rw-r--r--   0        0        0     6105 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/io_test_file_io.hh
--rw-r--r--   0        0        0     2172 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/io_test_file_io_base.cc
--rw-r--r--   0        0        0    26649 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/io_test_file_io_netcdf.cc
--rw-r--r--   0        0        0     1567 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/main_test_suite.cc
--rw-r--r--   0        0        0     3241 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/meson.build
--rw-r--r--   0        0        0     2758 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/mpi_context.hh
--rw-r--r--   0        0        0     5763 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/mpi_field_test_fixtures.hh
--rw-r--r--   0        0        0     9218 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/mpi_test_communicator.cc
--rw-r--r--   0        0        0    10926 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/mpi_test_field_map.cc
--rw-r--r--   0        0        0     1551 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_binding_tests.py
--rw-r--r--   0        0        0     5285 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_common_tests.py
--rw-r--r--   0        0        0     4509 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_communicator_tests.py
--rw-r--r--   0        0        0     7382 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_field_tests.py
--rw-r--r--   0        0        0    17489 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_file_io_test.py
--rw-r--r--   0        0        0     1472 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_mpi_binding_test.py
--rw-r--r--   0        0        0     5587 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/python_muGrid_license_test.py
--rw-r--r--   0        0        0     5268 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_ccoord_operations.cc
--rw-r--r--   0        0        0     8295 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_discrete_gradient_operator.cc
--rw-r--r--   0        0        0    11196 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_discrete_gradient_operator.hh
--rw-r--r--   0        0        0    16004 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_field.cc
--rw-r--r--   0        0        0    15181 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_field_collection.cc
--rw-r--r--   0        0        0    13400 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_field_map.cc
--rw-r--r--   0        0        0     2439 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_goodies.cc
--rw-r--r--   0        0        0    10326 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_goodies.hh
--rw-r--r--   0        0        0    12583 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_mapped_fields.cc
--rw-r--r--   0        0        0     4122 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_mapped_state_fields.cc
--rw-r--r--   0        0        0     4787 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_options_dictionary.cc
--rw-r--r--   0        0        0     4775 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_raw_memory_operations.cc
--rw-r--r--   0        0        0    10851 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_state_field_maps.cc
--rw-r--r--   0        0        0     3274 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_state_fields.cc
--rw-r--r--   0        0        0     6831 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/test_units.cc
--rw-r--r--   0        0        0     1677 2024-06-01 21:09:05.000000 mugrid-0.91.0/tests/tests.hh
--rw-r--r--   0        0        0    44362 2024-06-01 21:12:48.470390 mugrid-0.91.0/PKG-INFO
+-rw-r--r--   0        0        0      195 2024-06-02 14:04:12.000000 mugrid-0.91.1/.clang-format
+-rw-r--r--   0        0        0      148 2024-06-02 14:04:12.000000 mugrid-0.91.1/.gitattributes
+-rw-r--r--   0        0        0      666 2024-06-02 14:04:12.000000 mugrid-0.91.1/.github/install_netcdf4.sh
+-rw-r--r--   0        0        0     1552 2024-06-02 14:04:12.000000 mugrid-0.91.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1091 2024-06-02 14:04:12.000000 mugrid-0.91.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2454 2024-06-02 14:04:12.000000 mugrid-0.91.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     2131 2024-06-02 14:04:12.000000 mugrid-0.91.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       93 2024-06-02 14:04:12.000000 mugrid-0.91.1/.gitignore
+-rw-r--r--   0        0        0      324 2024-06-02 14:04:12.000000 mugrid-0.91.1/.gitmodules
+-rw-r--r--   0        0        0     7823 2024-06-02 14:04:12.000000 mugrid-0.91.1/CHANGELOG.md
+-rw-r--r--   0        0        0      210 2024-06-02 14:04:12.000000 mugrid-0.91.1/CPPLINT.cfg
+-rw-r--r--   0        0        0    35149 2024-06-02 14:04:12.000000 mugrid-0.91.1/LICENSE
+-rw-r--r--   0        0        0     1514 2024-06-02 14:04:12.000000 mugrid-0.91.1/README.md
+-rw-r--r--   0        0        0     5765 2024-06-02 14:04:12.000000 mugrid-0.91.1/discover_version.py
+-rw-r--r--   0        0        0      726 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/Doxyfile
+-rw-r--r--   0        0        0    94508 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/MainSchema.png
+-rw-r--r--   0        0        0      608 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/Makefile
+-rw-r--r--   0        0        0    58298 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/logo_flat.png
+-rw-r--r--   0        0        0    37122 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/logo_square.png
+-rw-r--r--   0        0        0       34 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/requirements.txt
+-rw-r--r--   0        0        0   175699 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/CodingConvention.rst
+-rw-r--r--   0        0        0    10682 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/Cplusplus.rst
+-rw-r--r--   0        0        0       55 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/CplusplusAPI.rst
+-rw-r--r--   0        0        0     3331 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/GettingStarted.rst
+-rw-r--r--   0        0        0     8488 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/Python.rst
+-rw-r--r--   0        0        0      983 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/Summary.rst
+-rw-r--r--   0        0        0     6559 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/conf.py
+-rw-r--r--   0        0        0     1031 2024-06-02 14:04:12.000000 mugrid-0.91.1/doc/source/index.rst
+-rw-r--r--   0        0        0      337 2024-06-02 14:04:12.000000 mugrid-0.91.1/examples/components.py
+-rw-r--r--   0        0        0      647 2024-06-02 14:04:12.000000 mugrid-0.91.1/examples/field_collection.py
+-rw-r--r--   0        0        0      731 2024-06-02 14:04:12.000000 mugrid-0.91.1/examples/io.py
+-rw-r--r--   0        0        0      644 2024-06-02 14:04:12.000000 mugrid-0.91.1/examples/meson.build
+-rw-r--r--   0        0        0      595 2024-06-02 14:04:12.000000 mugrid-0.91.1/examples/sub_points.py
+-rw-r--r--   0        0        0       16 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/meson.build
+-rw-r--r--   0        0        0       56 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/__init__.py
+-rw-r--r--   0        0        0     7281 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_common_mugrid.cc
+-rw-r--r--   0        0        0     6000 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_communicator.cc
+-rw-r--r--   0        0        0     1934 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_declarations.hh
+-rw-r--r--   0        0        0     8343 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_field.cc
+-rw-r--r--   0        0        0    25546 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_field_collection.cc
+-rw-r--r--   0        0        0    13125 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_file_io.cc
+-rw-r--r--   0        0        0     1706 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_module.cc
+-rw-r--r--   0        0        0     6111 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_options_dictionary.cc
+-rw-r--r--   0        0        0     3535 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/bind_py_state_field.cc
+-rw-r--r--   0        0        0      512 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/meson.build
+-rw-r--r--   0        0        0     3234 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/muGrid/Parallel.py
+-rw-r--r--   0        0        0     2009 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/muGrid/__init__.py
+-rw-r--r--   0        0        0      170 2024-06-02 14:04:12.000000 mugrid-0.91.1/language_bindings/python/muGrid/meson.build
+-rw-r--r--   0        0        0     2139 2024-06-02 14:04:12.000000 mugrid-0.91.1/meson.build
+-rw-r--r--   0        0        0     1861 2024-06-02 14:04:12.000000 mugrid-0.91.1/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-06-02 14:04:12.000000 mugrid-0.91.1/renovate.json
+-rw-r--r--   0        0        0     4386 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/T4_map_proxy.hh
+-rw-r--r--   0        0        0    11836 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/ccoord_operations.cc
+-rw-r--r--   0        0        0    37927 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/ccoord_operations.hh
+-rw-r--r--   0        0        0     1675 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/communicator.cc
+-rw-r--r--   0        0        0    14105 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/communicator.hh
+-rw-r--r--   0        0        0     7264 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/cpp_compliance.hh
+-rw-r--r--   0        0        0    20115 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/eigen_tools.hh
+-rw-r--r--   0        0        0     3156 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/exception.cc
+-rw-r--r--   0        0        0    10912 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/exception.hh
+-rw-r--r--   0        0        0    14731 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field.cc
+-rw-r--r--   0        0        0    13078 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field.hh
+-rw-r--r--   0        0        0    28663 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection.cc
+-rw-r--r--   0        0        0    44908 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection.hh
+-rw-r--r--   0        0        0     8208 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection_global.cc
+-rw-r--r--   0        0        0    10942 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection_global.hh
+-rw-r--r--   0        0        0     4298 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection_local.cc
+-rw-r--r--   0        0        0     5045 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_collection_local.hh
+-rw-r--r--   0        0        0    10753 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_map.cc
+-rw-r--r--   0        0        0    14422 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_map.hh
+-rw-r--r--   0        0        0    27124 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_map_static.hh
+-rw-r--r--   0        0        0    30081 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_typed.cc
+-rw-r--r--   0        0        0    25391 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/field_typed.hh
+-rw-r--r--   0        0        0     4334 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/file_io_base.cc
+-rw-r--r--   0        0        0    18299 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/file_io_base.hh
+-rw-r--r--   0        0        0   136261 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/file_io_netcdf.cc
+-rw-r--r--   0        0        0    68866 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/file_io_netcdf.hh
+-rw-r--r--   0        0        0     5544 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/gradient_operator_base.hh
+-rw-r--r--   0        0        0    15742 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/gradient_operator_default.cc
+-rw-r--r--   0        0        0     8116 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/gradient_operator_default.hh
+-rw-r--r--   0        0        0     3137 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/grid_common.cc
+-rw-r--r--   0        0        0    28182 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/grid_common.hh
+-rw-r--r--   0        0        0    12592 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/iterators.hh
+-rw-r--r--   0        0        0    13401 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/mapped_field.hh
+-rw-r--r--   0        0        0    10428 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/mapped_state_field.hh
+-rw-r--r--   0        0        0     1115 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/meson.build
+-rw-r--r--   0        0        0    19267 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/numpy_tools.hh
+-rw-r--r--   0        0        0     3636 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/optional_mapped_field.hh
+-rw-r--r--   0        0        0    11309 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/options_dictionary.cc
+-rw-r--r--   0        0        0     6513 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/options_dictionary.hh
+-rw-r--r--   0        0        0     4511 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/physics_domain.cc
+-rw-r--r--   0        0        0     3630 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/physics_domain.hh
+-rw-r--r--   0        0        0     1827 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/raw_memory_operations.cc
+-rw-r--r--   0        0        0     5613 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/raw_memory_operations.hh
+-rw-r--r--   0        0        0     3458 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/ref_array.hh
+-rw-r--r--   0        0        0     3363 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/ref_vector.hh
+-rw-r--r--   0        0        0     7857 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/state_field.cc
+-rw-r--r--   0        0        0    12121 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/state_field.hh
+-rw-r--r--   0        0        0     7284 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/state_field_map.cc
+-rw-r--r--   0        0        0     8806 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/state_field_map.hh
+-rw-r--r--   0        0        0    19738 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/state_field_map_static.hh
+-rw-r--r--   0        0        0    22553 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/tensor_algebra.hh
+-rw-r--r--   0        0        0    16900 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/units.cc
+-rw-r--r--   0        0        0     9578 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/units.hh
+-rw-r--r--   0        0        0     2484 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/libmugrid/version.cc.skeleton
+-rw-r--r--   0        0        0      167 2024-06-02 14:04:12.000000 mugrid-0.91.1/src/meson.build
+-rw-r--r--   0        0        0      590 2024-06-02 14:04:12.000000 mugrid-0.91.1/subprojects/eigen.wrap
+-rw-r--r--   0        0        0      616 2024-06-02 14:04:12.000000 mugrid-0.91.1/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0     1654 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/field_test_fixtures.cc
+-rw-r--r--   0        0        0     5370 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/field_test_fixtures.hh
+-rw-r--r--   0        0        0     8857 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/header_test_ccoord_operations.cc
+-rw-r--r--   0        0        0     4611 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/header_test_eigen_tools.cc
+-rw-r--r--   0        0        0     1702 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/header_test_ref_array.cc
+-rw-r--r--   0        0        0     7334 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/header_test_t4_map.cc
+-rw-r--r--   0        0        0    11181 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/header_test_tensor_algebra.cc
+-rw-r--r--   0        0        0     4983 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/io_mpi_test_file_io.hh
+-rw-r--r--   0        0        0    22974 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/io_mpi_test_file_io_netcdf.cc
+-rw-r--r--   0        0        0     6105 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/io_test_file_io.hh
+-rw-r--r--   0        0        0     2172 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/io_test_file_io_base.cc
+-rw-r--r--   0        0        0    26649 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/io_test_file_io_netcdf.cc
+-rw-r--r--   0        0        0     1567 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/main_test_suite.cc
+-rw-r--r--   0        0        0     3241 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/meson.build
+-rw-r--r--   0        0        0     2758 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/mpi_context.hh
+-rw-r--r--   0        0        0     5763 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/mpi_field_test_fixtures.hh
+-rw-r--r--   0        0        0     9218 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/mpi_test_communicator.cc
+-rw-r--r--   0        0        0    10926 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/mpi_test_field_map.cc
+-rw-r--r--   0        0        0     1551 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_binding_tests.py
+-rw-r--r--   0        0        0     5285 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_common_tests.py
+-rw-r--r--   0        0        0     4509 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_communicator_tests.py
+-rw-r--r--   0        0        0     7382 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_field_tests.py
+-rw-r--r--   0        0        0    17489 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_file_io_test.py
+-rw-r--r--   0        0        0     1472 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_mpi_binding_test.py
+-rw-r--r--   0        0        0     5587 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/python_muGrid_license_test.py
+-rw-r--r--   0        0        0     5268 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_ccoord_operations.cc
+-rw-r--r--   0        0        0     8295 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_discrete_gradient_operator.cc
+-rw-r--r--   0        0        0    11196 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_discrete_gradient_operator.hh
+-rw-r--r--   0        0        0    16004 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_field.cc
+-rw-r--r--   0        0        0    15181 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_field_collection.cc
+-rw-r--r--   0        0        0    13400 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_field_map.cc
+-rw-r--r--   0        0        0     2439 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_goodies.cc
+-rw-r--r--   0        0        0    10326 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_goodies.hh
+-rw-r--r--   0        0        0    12583 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_mapped_fields.cc
+-rw-r--r--   0        0        0     4122 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_mapped_state_fields.cc
+-rw-r--r--   0        0        0     4787 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_options_dictionary.cc
+-rw-r--r--   0        0        0     4775 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_raw_memory_operations.cc
+-rw-r--r--   0        0        0    10851 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_state_field_maps.cc
+-rw-r--r--   0        0        0     3274 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_state_fields.cc
+-rw-r--r--   0        0        0     6831 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/test_units.cc
+-rw-r--r--   0        0        0     1677 2024-06-02 14:04:12.000000 mugrid-0.91.1/tests/tests.hh
+-rw-r--r--   0        0        0    42832 2024-06-02 14:08:23.260705 mugrid-0.91.1/PKG-INFO
```

### Comparing `mugrid-0.91.0/.github/install_netcdf4.sh` & `mugrid-0.91.1/.github/install_netcdf4.sh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/.github/workflows/documentation.yml` & `mugrid-0.91.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/.github/workflows/publish.yml` & `mugrid-0.91.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/.github/workflows/tests.yml` & `mugrid-0.91.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/.github/workflows/wheels.yml` & `mugrid-0.91.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/CHANGELOG.md` & `mugrid-0.91.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change log for µSpectre
 =======================
 
+0.91.1 (02June2024)
+-------------------
+
+- BUG: Updated `NumpyProxy` to reflect that a global field collection no
+  longer required number of spatial dimensions as first argument
+
 0.91.0 (01June2024)
 -------------------
 
 - ENH: Added attributes `p` and `s` for convenience access to pixel-shaped
   and sub-point-shaped numpy arrays
 - ENH: Convenience filed accessor function `real_field`, `int_field`, etc.
   that create fields if they don't exist but return them if they do
```

### Comparing `mugrid-0.91.0/LICENSE` & `mugrid-0.91.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/discover_version.py` & `mugrid-0.91.1/discover_version.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/Doxyfile` & `mugrid-0.91.1/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/MainSchema.png` & `mugrid-0.91.1/doc/MainSchema.png`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/Makefile` & `mugrid-0.91.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/logo_flat.png` & `mugrid-0.91.1/doc/logo_flat.png`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/logo_square.png` & `mugrid-0.91.1/doc/logo_square.png`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/CodingConvention.rst` & `mugrid-0.91.1/doc/source/CodingConvention.rst`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/Cplusplus.rst` & `mugrid-0.91.1/doc/source/Cplusplus.rst`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/GettingStarted.rst` & `mugrid-0.91.1/doc/source/GettingStarted.rst`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/Python.rst` & `mugrid-0.91.1/doc/source/Python.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Python Bindings
 ###############
 
 Fields
 ******
 
-The *µ*\Grid library handles field quantities, i.e. scalar, vectors or tensors,
+The µGrid library handles field quantities, i.e. scalar, vectors or tensors,
 that vary in space. It supports only a uniform discretization of space. In the
-language of *µ*\Grid, we call the discrete coordinates **pixels**. Each pixel
-is associated with a physical position in space. *µ*\Grid supports fields in
+language of µGrid, we call the discrete coordinates **pixels**. Each pixel
+is associated with a physical position in space. µGrid supports fields in
 two and three dimensional Cartesian grids. Note that a common name for a pixel
 in three dimensions is a **voxel**, but we refer to it as a pixel throughout
 this documentation.
 
 Each pixel
 can be subdivided into logical elements, for example into a number of
 support points for numerical quadrature. These subdivisions are called
-**sub-points**. Note that while *µ*\Grid understands the physical location of
+**sub-points**. Note that while µGrid understands the physical location of
 each *pixel*, the *sub-points* are logical subdivisions and not associated
 with any position within the pixel. Each *sub-point* carries the field quantity,
 which can be a scalar, vector or any type of tensor. The field quantity is
 called the **component**.
 
 Multidimensional arrays
 ***********************
 
-Each *µ*\Grid field has a representation in a multidimensional array. This
+Each µGrid field has a representation in a multidimensional array. This
 representation is used when accessing a field with Python via `numpy <https://numpy.org/>`_
 or when writing the field to a file. The default representation has the shape
 
 .. code-block:: Python
 
     (components, sub-points, pixels)
 
@@ -58,15 +58,15 @@
 
 Depending on the numerical use case, it can be useful to work with either
 representation.
 
 Field collections
 *****************
 
-In *µ*\Grid, fields are grouped into field collections. A field collection knows
+In µGrid, fields are grouped into field collections. A field collection knows
 about the spatial discretization of the fields, but each field can differ in number of
 sub-points and components.
 
 There are two kinds of field collections:
 
 * A **global** collection that groups fields that have values at all pixels.
 * A **local** collection that groups fields that have values only at a subset of pixels.
@@ -171,15 +171,15 @@
 Note that the default storage order of the field is column-major, which means the
 field components are stored next to each other in memory.
 
 I/O
 ***
 
 Fields can be written to disk in the `NetCDF <https://en.wikipedia.org/wiki/NetCDF>`_ format.
-*µ*\Grid uses `Unidata NetCDF <https://www.unidata.ucar.edu/software/netcdf/>`_ when build
+µGrid uses `Unidata NetCDF <https://www.unidata.ucar.edu/software/netcdf/>`_ when build
 with just serial capabilities and `PnetCDF <https://parallel-netcdf.github.io/>`_ when build
 with MPI enabled.
 
 I/O is handled by the `FileIONetCDF` class. The following example shows how to write all fields
 from a field collection to disk:
 
 .. literalinclude:: ../../examples/io.py
```

### Comparing `mugrid-0.91.0/doc/source/Summary.rst` & `mugrid-0.91.1/doc/source/Summary.rst`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/conf.py` & `mugrid-0.91.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/doc/source/index.rst` & `mugrid-0.91.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/examples/field_collection.py` & `mugrid-0.91.1/examples/field_collection.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/examples/io.py` & `mugrid-0.91.1/examples/io.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/examples/meson.build` & `mugrid-0.91.1/examples/meson.build`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/examples/sub_points.py` & `mugrid-0.91.1/examples/sub_points.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_common_mugrid.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_common_mugrid.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_communicator.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_communicator.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_declarations.hh` & `mugrid-0.91.1/language_bindings/python/bind_py_declarations.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_field.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_field.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_field_collection.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_field_collection.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_file_io.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_file_io.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_module.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_module.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_options_dictionary.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_options_dictionary.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/bind_py_state_field.cc` & `mugrid-0.91.1/language_bindings/python/bind_py_state_field.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/meson.build` & `mugrid-0.91.1/language_bindings/python/meson.build`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/muGrid/Parallel.py` & `mugrid-0.91.1/language_bindings/python/muGrid/Parallel.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/language_bindings/python/muGrid/__init__.py` & `mugrid-0.91.1/language_bindings/python/muGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/meson.build` & `mugrid-0.91.1/meson.build`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/pyproject.toml` & `mugrid-0.91.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov"
 ]
 
 [project.urls]
-documentation = "https://muspectre.gitlab.io/muspectre/index.html"
+documentation = "https://muspectre.github.io/muGrid/"
 repository = "https://github.com/muSpectre/muGrid"
 changelog = "https://github.com/muSpectre/muGrid/blob/main/CHANGELOG.md"
 
 [[tool.cibuildwheel.overrides]]
 select = "*manylinux*"
 # Build static NetCDF library
 before-all = [
```

### Comparing `mugrid-0.91.0/src/libmugrid/T4_map_proxy.hh` & `mugrid-0.91.1/src/libmugrid/T4_map_proxy.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/ccoord_operations.cc` & `mugrid-0.91.1/src/libmugrid/ccoord_operations.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/ccoord_operations.hh` & `mugrid-0.91.1/src/libmugrid/ccoord_operations.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/communicator.cc` & `mugrid-0.91.1/src/libmugrid/communicator.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/communicator.hh` & `mugrid-0.91.1/src/libmugrid/communicator.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/cpp_compliance.hh` & `mugrid-0.91.1/src/libmugrid/cpp_compliance.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/eigen_tools.hh` & `mugrid-0.91.1/src/libmugrid/eigen_tools.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/exception.cc` & `mugrid-0.91.1/src/libmugrid/exception.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/exception.hh` & `mugrid-0.91.1/src/libmugrid/exception.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field.cc` & `mugrid-0.91.1/src/libmugrid/field.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field.hh` & `mugrid-0.91.1/src/libmugrid/field.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection.cc` & `mugrid-0.91.1/src/libmugrid/field_collection.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection.hh` & `mugrid-0.91.1/src/libmugrid/field_collection.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection_global.cc` & `mugrid-0.91.1/src/libmugrid/field_collection_global.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection_global.hh` & `mugrid-0.91.1/src/libmugrid/field_collection_global.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection_local.cc` & `mugrid-0.91.1/src/libmugrid/field_collection_local.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_collection_local.hh` & `mugrid-0.91.1/src/libmugrid/field_collection_local.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_map.cc` & `mugrid-0.91.1/src/libmugrid/field_map.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_map.hh` & `mugrid-0.91.1/src/libmugrid/field_map.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_map_static.hh` & `mugrid-0.91.1/src/libmugrid/field_map_static.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_typed.cc` & `mugrid-0.91.1/src/libmugrid/field_typed.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/field_typed.hh` & `mugrid-0.91.1/src/libmugrid/field_typed.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/file_io_base.cc` & `mugrid-0.91.1/src/libmugrid/file_io_base.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/file_io_base.hh` & `mugrid-0.91.1/src/libmugrid/file_io_base.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/file_io_netcdf.cc` & `mugrid-0.91.1/src/libmugrid/file_io_netcdf.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/file_io_netcdf.hh` & `mugrid-0.91.1/src/libmugrid/file_io_netcdf.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/gradient_operator_base.hh` & `mugrid-0.91.1/src/libmugrid/gradient_operator_base.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/gradient_operator_default.cc` & `mugrid-0.91.1/src/libmugrid/gradient_operator_default.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/gradient_operator_default.hh` & `mugrid-0.91.1/src/libmugrid/gradient_operator_default.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/grid_common.cc` & `mugrid-0.91.1/src/libmugrid/grid_common.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/grid_common.hh` & `mugrid-0.91.1/src/libmugrid/grid_common.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/iterators.hh` & `mugrid-0.91.1/src/libmugrid/iterators.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/mapped_field.hh` & `mugrid-0.91.1/src/libmugrid/mapped_field.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/mapped_state_field.hh` & `mugrid-0.91.1/src/libmugrid/mapped_state_field.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/meson.build` & `mugrid-0.91.1/src/libmugrid/meson.build`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/numpy_tools.hh` & `mugrid-0.91.1/src/libmugrid/numpy_tools.hh`

 * *Files 3% similar despite different names*

```diff
@@ -65,16 +65,15 @@
 
   namespace internal {
 
     //! convert strides into the storage order description used by muGrid
     template <typename T, int flags = py::array::forcecast>
     inline std::tuple<StorageOrder, DynCcoord_t, Shape_t>
     detect_storage_order(const DynCcoord_t & nb_subdomain_grid_pts,
-                         const Shape_t & components_shape,
-                         Index_t nb_sub_pts,
+                         const Shape_t & components_shape, Index_t nb_sub_pts,
                          py::array_t<T, flags> & array) {
       auto & dim{nb_subdomain_grid_pts.get_dim()};
       if (static_cast<py::ssize_t>(dim + components_shape.size()) !=
           array.ndim()) {
         std::stringstream s;
         s << "Internal error: Array dimension (= " << array.ndim()
           << ") do not match expected number of dimensions (" << dim
@@ -101,36 +100,35 @@
         }
       }
       if (nb_components > 1 and !components_shape.empty() and nb_sub_pts == 1) {
         // Insert a token stride for the single sub-point
         strides.push_back(0);
       }
       for (int i = 0; i < dim; ++i) {
-        pixels_strides.push_back(
-            array.strides(array.ndim() - dim + i));
-        strides.push_back(
-            array.strides(array.ndim() - dim + i) / array.itemsize());
+        pixels_strides.push_back(array.strides(array.ndim() - dim + i));
+        strides.push_back(array.strides(array.ndim() - dim + i) /
+                          array.itemsize());
       }
 
       // Determine the storage order of the whole buffer. We first check the
       // order of pixels vs. sub-points storage. This is our first guess for
       // the storage order of the whole buffer.
       StorageOrder fc_storage_order{StorageOrder::ColMajor};
       if (components_strides.size() > 0) {
         fc_storage_order = StorageOrder::Unknown;
         const auto c{std::minmax_element(components_strides.begin(),
                                          components_strides.end())};
-        const auto p{std::minmax_element(pixels_strides.begin(),
-                                         pixels_strides.end())};
+        const auto p{
+            std::minmax_element(pixels_strides.begin(), pixels_strides.end())};
         if (*c.first > *p.second) {
           // this may be row-major, but we need to check that buffer is
           // contiguous
-          if (*c.first == nb_subdomain_grid_pts[
-                              p.second - pixels_strides.begin()] *
-                              (*p.second)) {
+          if (*c.first ==
+              nb_subdomain_grid_pts[p.second - pixels_strides.begin()] *
+                  (*p.second)) {
             fc_storage_order = StorageOrder::RowMajor;
           }
         } else {
           if (*c.second <= *p.first) {
             // this may be column-major, but we need to check that buffer is
             // contiguous
             if (*p.first ==
@@ -174,16 +172,16 @@
             }
           }
         }
       }
 
       // the pixels generally support arbitrary strides, but we must normalize
       // to the smallest entry
-      Index_t smallest_stride{*std::min_element(pixels_strides.begin(),
-                                                pixels_strides.end())};
+      Index_t smallest_stride{
+          *std::min_element(pixels_strides.begin(), pixels_strides.end())};
       if (smallest_stride > 0) {
         for (auto && s : pixels_strides) {
           s /= smallest_stride;
         }
       }
 
       // If we have more than one sub-pt, the field to be wrapped must match
@@ -259,21 +257,20 @@
      * where the number of components and grid indices can be arbitrary.
      */
     NumpyProxy(DynCcoord_t nb_domain_grid_pts,
                DynCcoord_t nb_subdomain_grid_pts,
                DynCcoord_t subdomain_locations, Index_t nb_dof_per_pixel,
                py::array_t<T, flags> & array,
                const Unit & unit = Unit::unitless())
-        : collection{}, field{}
-    {
+        : collection{}, field{} {
       // Sanity check 1: Are the sizes of array and field equal?
-      Index_t size{std::accumulate(
-                       nb_subdomain_grid_pts.begin(),
-                       nb_subdomain_grid_pts.end(), 1,
-                       std::multiplies<Index_t>())*nb_dof_per_pixel};
+      Index_t size{std::accumulate(nb_subdomain_grid_pts.begin(),
+                                   nb_subdomain_grid_pts.end(), 1,
+                                   std::multiplies<Index_t>()) *
+                   nb_dof_per_pixel};
       if (size != array.size()) {
         std::stringstream s;
         s << "The numpy array has a size of " << array.size() << ", but the "
           << "muGrid field reports a size of " << size << " entries.";
         throw NumpyError(s.str());
       }
 
@@ -324,24 +321,22 @@
       auto & fc_storage_order{std::get<0>(storage_order)};
       auto & pixels_strides{std::get<1>(storage_order)};
       auto & strides{std::get<2>(storage_order)};
 
       FieldCollection::SubPtMap_t map{};
       map["proxy_subpt"] = 1;
       this->collection = std::make_unique<Collection_t>(
-          static_cast<Index_t>(nb_subdomain_grid_pts.get_dim()),
           nb_domain_grid_pts, nb_subdomain_grid_pts, subdomain_locations,
           pixels_strides, map, fc_storage_order);
       // Note: The pointer should be obtained from array.template mutable_data()
       // but this has a guard if the array is not writeable. We need a constant
       // WrappedField to clean up this code.
       this->field = std::make_unique<WrappedField<T>>(
-          "proxy_field", *collection, components_shape,
-          array.size(), static_cast<T *>(array.request().ptr),
-          "proxy_subpt", unit, strides);
+          "proxy_field", *collection, components_shape, array.size(),
+          static_cast<T *>(array.request().ptr), "proxy_subpt", unit, strides);
     }
 
     /**
      * Construct a NumpyProxy given that we know the shape of the leading
      * component indices. The constructor will complain if both the grid
      * dimensions and the component dimensions differ. `get_component_shape`
      * returns exactly the shape passed to this constructor.
@@ -359,32 +354,30 @@
         : collection{}, field{} {
       // Sanity check: Do the array dimensions agree and shapes agree?
       Index_t dim{nb_subdomain_grid_pts.get_dim()};
       bool shape_matches{false};
       Shape_t sub_pt_shape{components_shape};
       if (static_cast<py::ssize_t>(dim + components_shape.size() + 1) ==
           array.ndim()) {
-        shape_matches =
-            std::equal(nb_subdomain_grid_pts.begin(),
-                       nb_subdomain_grid_pts.end(),
-                       array.shape() + array.ndim() - dim) &&
-            nb_sub_pts == array.shape(components_shape.size()) &&
-            std::equal(components_shape.begin(), components_shape.end(),
-                       array.shape());
+        shape_matches = std::equal(nb_subdomain_grid_pts.begin(),
+                                   nb_subdomain_grid_pts.end(),
+                                   array.shape() + array.ndim() - dim) &&
+                        nb_sub_pts == array.shape(components_shape.size()) &&
+                        std::equal(components_shape.begin(),
+                                   components_shape.end(), array.shape());
         sub_pt_shape.push_back(nb_sub_pts);
       } else if (static_cast<py::ssize_t>(dim + components_shape.size()) ==
                  array.ndim()) {
         // For a field with a single quad point, we can omit that dimension.
-        shape_matches =
-            std::equal(nb_subdomain_grid_pts.begin(),
-                       nb_subdomain_grid_pts.end(),
-                       array.shape() + array.ndim() - dim) &&
-            nb_sub_pts == 1 &&
-            std::equal(components_shape.begin(), components_shape.end(),
-                       array.shape());
+        shape_matches = std::equal(nb_subdomain_grid_pts.begin(),
+                                   nb_subdomain_grid_pts.end(),
+                                   array.shape() + array.ndim() - dim) &&
+                        nb_sub_pts == 1 &&
+                        std::equal(components_shape.begin(),
+                                   components_shape.end(), array.shape());
       }
       if (!shape_matches) {
         std::stringstream s;
         s << "The numpy array has shape " << array.request().shape << ", but "
           << "the muGrid field reports a grid of " << nb_subdomain_grid_pts
           << " pixels with " << nb_sub_pts << " quadrature "
           << (nb_sub_pts == 1 ? "point" : "points") << " holding a quantity of "
@@ -397,24 +390,23 @@
       auto & fc_storage_order{std::get<0>(storage_order)};
       auto & pixels_strides{std::get<1>(storage_order)};
       auto & sub_pt_iter_strides{std::get<2>(storage_order)};
 
       FieldCollection::SubPtMap_t map{};
       map["proxy_subpt"] = nb_sub_pts;
       this->collection = std::make_unique<Collection_t>(
-          static_cast<Index_t>(nb_subdomain_grid_pts.get_dim()),
           nb_domain_grid_pts, nb_subdomain_grid_pts, subdomain_locations,
           pixels_strides, map, fc_storage_order);
       // Note: The pointer should be obtained from array.template mutable_data()
       // but this has a guard if the array is not writeable. We need a constant
       // WrappedField to clean up this code.
       this->field = std::make_unique<WrappedField<T>>(
-          "proxy_field", *collection, components_shape,
-          array.size(), static_cast<T *>(array.request().ptr),
-          "proxy_subpt", unit, sub_pt_iter_strides);
+          "proxy_field", *collection, components_shape, array.size(),
+          static_cast<T *>(array.request().ptr), "proxy_subpt", unit,
+          sub_pt_iter_strides);
     }
 
     /**
      * move constructor
      */
     NumpyProxy(NumpyProxy && other) = default;
 
@@ -422,32 +414,30 @@
 
     Collection_t & get_collection() { return *this->collection; }
 
     const Shape_t get_components_shape() const {
       return this->field->get_components_shape();
     }
 
-    Shape_t get_sub_pt_shape() const {
-      return this->field->get_sub_pt_shape();
-    }
+    Shape_t get_sub_pt_shape() const { return this->field->get_sub_pt_shape(); }
 
    protected:
     std::unique_ptr<Collection_t> collection;
     std::unique_ptr<WrappedField<T>> field;
   };
 
   /* Wrap a column-major field into a numpy array, without copying the data */
   template <typename T>
   py::array_t<T, py::array::f_style>
   numpy_wrap(const TypedFieldBase<T> & field,
              IterUnit iter_type = IterUnit::SubPt) {
     Shape_t shape{field.get_shape(iter_type)};
     Shape_t strides{field.get_strides(iter_type, sizeof(T))};
-    return py::array_t<T, py::array::f_style>(
-        shape, strides, field.data(), py::capsule([]() {}));
+    return py::array_t<T, py::array::f_style>(shape, strides, field.data(),
+                                              py::capsule([]() {}));
   }
 
   /* Turn any type that can be enumerated into a tuple */
   template <typename T>
   py::tuple to_tuple(T a) {
     py::tuple t(a.get_dim());
     ssize_t i = 0;
```

### Comparing `mugrid-0.91.0/src/libmugrid/optional_mapped_field.hh` & `mugrid-0.91.1/src/libmugrid/optional_mapped_field.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/options_dictionary.cc` & `mugrid-0.91.1/src/libmugrid/options_dictionary.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/options_dictionary.hh` & `mugrid-0.91.1/src/libmugrid/options_dictionary.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/physics_domain.cc` & `mugrid-0.91.1/src/libmugrid/physics_domain.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/physics_domain.hh` & `mugrid-0.91.1/src/libmugrid/physics_domain.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/raw_memory_operations.cc` & `mugrid-0.91.1/src/libmugrid/raw_memory_operations.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/raw_memory_operations.hh` & `mugrid-0.91.1/src/libmugrid/raw_memory_operations.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/ref_array.hh` & `mugrid-0.91.1/src/libmugrid/ref_array.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/ref_vector.hh` & `mugrid-0.91.1/src/libmugrid/ref_vector.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/state_field.cc` & `mugrid-0.91.1/src/libmugrid/state_field.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/state_field.hh` & `mugrid-0.91.1/src/libmugrid/state_field.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/state_field_map.cc` & `mugrid-0.91.1/src/libmugrid/state_field_map.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/state_field_map.hh` & `mugrid-0.91.1/src/libmugrid/state_field_map.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/state_field_map_static.hh` & `mugrid-0.91.1/src/libmugrid/state_field_map_static.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/tensor_algebra.hh` & `mugrid-0.91.1/src/libmugrid/tensor_algebra.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/units.cc` & `mugrid-0.91.1/src/libmugrid/units.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/units.hh` & `mugrid-0.91.1/src/libmugrid/units.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/src/libmugrid/version.cc.skeleton` & `mugrid-0.91.1/src/libmugrid/version.cc.skeleton`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/subprojects/eigen.wrap` & `mugrid-0.91.1/subprojects/eigen.wrap`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/subprojects/pybind11.wrap` & `mugrid-0.91.1/subprojects/pybind11.wrap`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/field_test_fixtures.cc` & `mugrid-0.91.1/tests/field_test_fixtures.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/field_test_fixtures.hh` & `mugrid-0.91.1/tests/field_test_fixtures.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/header_test_ccoord_operations.cc` & `mugrid-0.91.1/tests/header_test_ccoord_operations.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/header_test_eigen_tools.cc` & `mugrid-0.91.1/tests/header_test_eigen_tools.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/header_test_ref_array.cc` & `mugrid-0.91.1/tests/header_test_ref_array.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/header_test_t4_map.cc` & `mugrid-0.91.1/tests/header_test_t4_map.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/header_test_tensor_algebra.cc` & `mugrid-0.91.1/tests/header_test_tensor_algebra.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/io_mpi_test_file_io.hh` & `mugrid-0.91.1/tests/io_mpi_test_file_io.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/io_mpi_test_file_io_netcdf.cc` & `mugrid-0.91.1/tests/io_mpi_test_file_io_netcdf.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/io_test_file_io.hh` & `mugrid-0.91.1/tests/io_test_file_io.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/io_test_file_io_base.cc` & `mugrid-0.91.1/tests/io_test_file_io_base.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/io_test_file_io_netcdf.cc` & `mugrid-0.91.1/tests/io_test_file_io_netcdf.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/main_test_suite.cc` & `mugrid-0.91.1/tests/main_test_suite.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/meson.build` & `mugrid-0.91.1/tests/meson.build`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/mpi_context.hh` & `mugrid-0.91.1/tests/mpi_context.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/mpi_field_test_fixtures.hh` & `mugrid-0.91.1/tests/mpi_field_test_fixtures.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/mpi_test_communicator.cc` & `mugrid-0.91.1/tests/mpi_test_communicator.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/mpi_test_field_map.cc` & `mugrid-0.91.1/tests/mpi_test_field_map.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_binding_tests.py` & `mugrid-0.91.1/tests/python_binding_tests.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_common_tests.py` & `mugrid-0.91.1/tests/python_common_tests.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_communicator_tests.py` & `mugrid-0.91.1/tests/python_communicator_tests.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_field_tests.py` & `mugrid-0.91.1/tests/python_field_tests.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_file_io_test.py` & `mugrid-0.91.1/tests/python_file_io_test.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_mpi_binding_test.py` & `mugrid-0.91.1/tests/python_mpi_binding_test.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/python_muGrid_license_test.py` & `mugrid-0.91.1/tests/python_muGrid_license_test.py`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_ccoord_operations.cc` & `mugrid-0.91.1/tests/test_ccoord_operations.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_discrete_gradient_operator.cc` & `mugrid-0.91.1/tests/test_discrete_gradient_operator.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_discrete_gradient_operator.hh` & `mugrid-0.91.1/tests/test_discrete_gradient_operator.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_field.cc` & `mugrid-0.91.1/tests/test_field.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_field_collection.cc` & `mugrid-0.91.1/tests/test_field_collection.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_field_map.cc` & `mugrid-0.91.1/tests/test_field_map.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_goodies.cc` & `mugrid-0.91.1/tests/test_goodies.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_goodies.hh` & `mugrid-0.91.1/tests/test_goodies.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_mapped_fields.cc` & `mugrid-0.91.1/tests/test_mapped_fields.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_mapped_state_fields.cc` & `mugrid-0.91.1/tests/test_mapped_state_fields.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_options_dictionary.cc` & `mugrid-0.91.1/tests/test_options_dictionary.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_raw_memory_operations.cc` & `mugrid-0.91.1/tests/test_raw_memory_operations.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_state_field_maps.cc` & `mugrid-0.91.1/tests/test_state_field_maps.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_state_fields.cc` & `mugrid-0.91.1/tests/test_state_fields.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/test_units.cc` & `mugrid-0.91.1/tests/test_units.cc`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/tests/tests.hh` & `mugrid-0.91.1/tests/tests.hh`

 * *Files identical despite different names*

### Comparing `mugrid-0.91.0/PKG-INFO` & `mugrid-0.91.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muGrid
-Version: 0.91.0
+Version: 0.91.1
 Summary: MPI-parallel regular grids
 Author-Email: Ali Falsafi <ali.falsafi@epfl.ch>, Till Junge <till.junge@altermail.ch>, Richard Leute <richard.leute@imtek.uni-freiburg.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Project-URL: Documentation, https://muspectre.gitlab.io/muspectre/index.html
+Project-URL: Documentation, https://muspectre.github.io/muGrid/
 Project-URL: Repository, https://github.com/muSpectre/muGrid
 Project-URL: Changelog, https://github.com/muSpectre/muGrid/blob/main/CHANGELOG.md
 Requires-Python: >=3.8.0
 Requires-Dist: numpy
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: test
@@ -719,67 +719,14 @@
 [MPI](https://www.mpi-forum.org/).
 For I/O, it will try to use
 [Unidata NetCDF](https://www.unidata.ucar.edu/software/netcdf/)
 for serial builds and
 [PnetCDF](https://parallel-netcdf.github.io/) for MPI-parallel builds.
 Monitor output to see which of these options were automatically detected.
 
-## Simple usage example
-
-The following is a simple example for using µGrid through its convenient
-Python interface
-
-    #!/usr/bin/env python3
-
-    import numpy as np
-    import muGrid
-
-    # setting the geometry
-    nb_grid_pts = [51, 51]
-    center = np.array([r//2 for r in nb_grid_pts])
-    incl = nb_grid_pts[0]//5
-
-    lengths = [7., 5.]
-    formulation = µ.Formulation.small_strain
-
-    # creating the periodic cell
-    rve = µ.SystemFactory(nb_grid_pts,
-                          lengths,
-                          formulation)
-    hard = µ.material.MaterialLinearElastic1_2d.make(
-        rve, "hard", 10e9, .33)
-    soft = µ.material.MaterialLinearElastic1_2d.make(
-        rve, "soft",  70e9, .33)
-
-
-    # assign a material to each pixel
-    for i, pixel in enumerate(rve):
-        if np.linalg.norm(center - np.array(pixel),2)<incl:
-            hard.add_pixel(pixel)
-        else:
-            soft.add_pixel(pixel)
-
-    tol = 1e-5
-    cg_tol = 1e-8
-
-    # set macroscopic strain
-    Del0 = np.array([[.0, .0],
-                     [0,  .03]])
-    if formulation == µ.Formulation.small_strain:
-        Del0 = .5*(Del0 + Del0.T)
-    maxiter = 401
-    verbose = 2
-
-    solver = µ.solvers.SolverCG(rve, cg_tol, maxiter, verbose=False)
-    r = µ.solvers.newton_cg(rve, Del0, solver, tol, verbose)
-    print("nb of {} iterations: {}".format(solver.name(), r.nb_fev))
-
-You can find more examples using both the Python and the C++ interface in the
-[`examples`](./examples) and [`tests`](./tests) folder.
-
 ## Funding
 
 This development has received funding from the
 [Swiss National Science Foundation](https://www.snf.ch/en)
 within an Ambizione Project and by the
 [European Research Council](https://erc.europa.eu) within
 [Starting Grant 757343](https://cordis.europa.eu/project/id/757343).
```

