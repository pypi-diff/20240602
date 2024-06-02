# Comparing `tmp/naludaq-0.26.5.tar.gz` & `tmp/naludaq-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naludaq-0.26.5.tar", last modified: Wed May  8 20:37:04 2024, max compression
+gzip compressed data, was "naludaq-0.27.0.tar", last modified: Sun Jun  2 05:15:26 2024, max compression
```

## Comparing `naludaq-0.26.5.tar` & `naludaq-0.27.0.tar`

### file list

```diff
@@ -1,266 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.307410 naludaq-0.26.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-08 20:36:53.000000 naludaq-0.26.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-05-08 20:37:04.307410 naludaq-0.26.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-05-08 20:36:53.000000 naludaq-0.26.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 20:36:53.000000 naludaq-0.26.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:37:04.307410 naludaq-0.26.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-08 20:36:53.000000 naludaq-0.26.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.255409 naludaq-0.26.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.259410 naludaq-0.26.5/src/naludaq/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.263409 naludaq-0.26.5/src/naludaq/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.263409 naludaq-0.26.5/src/naludaq/backend/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/acquisitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/managers/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.263409 naludaq-0.26.5/src/naludaq/backend/models/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/backend/models/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.267409 naludaq-0.26.5/src/naludaq/board/
--rw-r--r--   0 runner    (1001) docker     (127)    31381 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24036 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/board_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.267409 naludaq-0.26.5/src/naludaq/board/connections/
--rw-r--r--   0 runner    (1001) docker     (127)    20239 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/_FTDI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/_MockUART.py
--rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/_UART.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/_USB.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/base_ethernet.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/tcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/connections/udp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.271410 naludaq-0.26.5/src/naludaq/board/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/init_aodsv2_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/init_hdsocv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/init_udc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/init_upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/initializers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/board/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.271410 naludaq-0.26.5/src/naludaq/communication/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/_fpga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/analog_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/chip_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/control_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/digital_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/i2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/communication/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.271410 naludaq-0.26.5/src/naludaq/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/analog_debug_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.275410 naludaq-0.26.5/src/naludaq/controllers/biasing_mode/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/biasing_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/biasing_mode/udc16.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.275410 naludaq-0.26.5/src/naludaq/controllers/board/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/asocv3s.py
--rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/oleas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/udc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/board/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.275410 naludaq-0.26.5/src/naludaq/controllers/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/connection/connection_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/connection/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/connection/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.279410 naludaq-0.26.5/src/naludaq/controllers/external_dac/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/ad5671.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/ad5675.py
--rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/dac7578.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/i2c_dac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/external_dac/upac32.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.279410 naludaq-0.26.5/src/naludaq/controllers/gainstages/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/gainstages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/gainstages/aodsv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/gainstages/oddsock_aods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.279410 naludaq-0.26.5/src/naludaq/controllers/peripherals/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/peripherals_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/peripherals/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/project_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.283410 naludaq-0.26.5/src/naludaq/controllers/readout/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/aardvarcv3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/asocv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/readout/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/si5341_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.283410 naludaq-0.26.5/src/naludaq/controllers/tia/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/tia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/tia/hdsoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.283410 naludaq-0.26.5/src/naludaq/controllers/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/aodsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/upac.py
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/controllers/trigger/upac96.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.283410 naludaq-0.26.5/src/naludaq/daq/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/debugdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/lightdaq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.287410 naludaq-0.26.5/src/naludaq/daq/workers/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/answer_parser_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/csv_storage_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.287410 naludaq-0.26.5/src/naludaq/daq/workers/packager/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/packager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/worker_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/worker_serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/daq/workers/worker_usb_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.287410 naludaq-0.26.5/src/naludaq/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/devices/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/devices/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/devices/ltc2990.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.291410 naludaq-0.26.5/src/naludaq/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/fancyiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/register_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/semiton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/helpers/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.291410 naludaq-0.26.5/src/naludaq/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/io/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/io/io_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.291410 naludaq-0.26.5/src/naludaq/models/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/models/acq_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/models/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/naludaq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.295410 naludaq-0.26.5/src/naludaq/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/aardvarcv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/answer_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/aodsoc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/asocv3_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/asocv3s_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/hdsoc_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.295410 naludaq-0.26.5/src/naludaq/parsers/headers/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/asoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/asocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/siread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/trbhm.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/headers/upac32.py
--rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/trbhm_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/udc_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/upac96_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/parsers/upac_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.295410 naludaq-0.26.5/src/naludaq/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/adc2mv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/adc2mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/adc2mv/adc_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/adc2mv/adc_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/adc2mv/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/adc2mv/pre_adc2mv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/autoaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/autotrigger/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/autotrigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/autotrigger/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/board_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/dac_sweep/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/dac_sweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/data_collector/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/data_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/data_collector/_daq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/data_collector/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/data_collector/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/ft60x.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/ftdi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/lookup_table/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/lookup_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/lookup_table/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/lookup_table/lookup_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.299410 naludaq-0.26.5/src/naludaq/tools/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/bayesian_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/optimizers/gainstagetuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/pedestals/
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24746 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/hdsoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/udc16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/generators/upac96.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/pedestals_correcter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/pedestals_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/threshold_scan/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/threshold_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/threshold_scan/threshold_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/timing_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/timing_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/timing_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/timing_cal/correcter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/src/naludaq/tools/waiter/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/waiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 20:36:53.000000 naludaq-0.26.5/src/naludaq/tools/waiter/eventwaiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.307410 naludaq-0.26.5/src/naludaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-05-08 20:37:04.000000 naludaq-0.26.5/src/naludaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-05-08 20:37:04.000000 naludaq-0.26.5/src/naludaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:37:04.000000 naludaq-0.26.5/src/naludaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 20:37:04.000000 naludaq-0.26.5/src/naludaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 20:37:04.000000 naludaq-0.26.5/src/naludaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:37:04.303410 naludaq-0.26.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 20:36:53.000000 naludaq-0.26.5/tests/test_naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.304169 naludaq-0.27.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-06-02 05:15:17.000000 naludaq-0.27.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-06-02 05:15:26.304169 naludaq-0.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-06-02 05:15:17.000000 naludaq-0.27.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-06-02 05:15:17.000000 naludaq-0.27.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 05:15:26.304169 naludaq-0.27.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-02 05:15:17.000000 naludaq-0.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.244168 naludaq-0.27.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.252168 naludaq-0.27.0/src/naludaq/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.256168 naludaq-0.27.0/src/naludaq/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.256168 naludaq-0.27.0/src/naludaq/backend/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/acquisitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/managers/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.256168 naludaq-0.27.0/src/naludaq/backend/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39569 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/backend/models/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.256168 naludaq-0.27.0/src/naludaq/board/
+-rw-r--r--   0 runner    (1001) docker     (127)    31381 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24123 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/board_inits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.260168 naludaq-0.27.0/src/naludaq/board/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)    20239 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/_FTDI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/_MockUART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15207 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/_UART.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/_USB.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/base_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9855 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/connections/udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.260168 naludaq-0.27.0/src/naludaq/board/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/init_aodsv2_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/init_hdsocv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/init_udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/init_upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/initializers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/board/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.264168 naludaq-0.27.0/src/naludaq/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10200 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/_fpga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/analog_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/chip_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/control_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/digital_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/communication/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.264168 naludaq-0.27.0/src/naludaq/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/analog_debug_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.264168 naludaq-0.27.0/src/naludaq/controllers/biasing_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/biasing_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/biasing_mode/udc16.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.268168 naludaq-0.27.0/src/naludaq/controllers/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/asocv3s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15507 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/oleas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/udc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/board/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.268168 naludaq-0.27.0/src/naludaq/controllers/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22223 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/connection/connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/connection/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/connection/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.272168 naludaq-0.27.0/src/naludaq/controllers/external_dac/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/ad5671.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/ad5675.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11496 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/dac7578.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/i2c_dac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/external_dac/upac32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.272168 naludaq-0.27.0/src/naludaq/controllers/gainstages/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/gainstages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/gainstages/aodsv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/gainstages/oddsock_aods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.272168 naludaq-0.27.0/src/naludaq/controllers/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/peripherals_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/peripherals/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/project_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.272168 naludaq-0.27.0/src/naludaq/controllers/readout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/aardvarcv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/asocv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/readout/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/si5341_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.276168 naludaq-0.27.0/src/naludaq/controllers/tia/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/tia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/tia/hdsoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.276168 naludaq-0.27.0/src/naludaq/controllers/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/aodsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/upac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/controllers/trigger/upac96.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.276168 naludaq-0.27.0/src/naludaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/debugdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8003 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/hiperdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/lightdaq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.280168 naludaq-0.27.0/src/naludaq/daq/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/answer_parser_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/csv_storage_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.280168 naludaq-0.27.0/src/naludaq/daq/workers/packager/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/packager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager_hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/worker_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/worker_serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/daq/workers/worker_usb_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.280168 naludaq-0.27.0/src/naludaq/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/devices/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/devices/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/devices/ltc2990.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.284168 naludaq-0.27.0/src/naludaq/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/fancyiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/register_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/semiton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/helpers/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.284168 naludaq-0.27.0/src/naludaq/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22338 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/io/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35939 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/io/io_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.284168 naludaq-0.27.0/src/naludaq/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/models/acq_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/models/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18812 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/naludaq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.288169 naludaq-0.27.0/src/naludaq/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/aardvarcv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/answer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/aodsoc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/asocv3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/asocv3s_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/hdsoc_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.288169 naludaq-0.27.0/src/naludaq/parsers/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/asoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/asocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/siread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/trbhm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/headers/upac32.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/hiper_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11956 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/trbhm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/udc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/upac96_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/parsers/upac_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.292168 naludaq-0.27.0/src/naludaq/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.292168 naludaq-0.27.0/src/naludaq/tools/adc2mv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/adc2mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/adc2mv/adc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/adc2mv/adc_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/adc2mv/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/adc2mv/pre_adc2mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/autoaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.292168 naludaq-0.27.0/src/naludaq/tools/autotrigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/autotrigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/autotrigger/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/board_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.292168 naludaq-0.27.0/src/naludaq/tools/dac_sweep/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/dac_sweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.292168 naludaq-0.27.0/src/naludaq/tools/data_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/data_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/data_collector/_daq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16865 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/data_collector/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/data_collector/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/ft60x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/ftdi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.296168 naludaq-0.27.0/src/naludaq/tools/lookup_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/lookup_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/lookup_table/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/lookup_table/lookup_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.296168 naludaq-0.27.0/src/naludaq/tools/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/bayesian_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.296168 naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/optimizers/gainstagetuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.296168 naludaq-0.27.0/src/naludaq/tools/pedestals/
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25213 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/hdsoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/hiper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/udc16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/generators/upac96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/pedestals_correcter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/pedestals_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/src/naludaq/tools/threshold_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/threshold_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/threshold_scan/threshold_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/src/naludaq/tools/timing_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/timing_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/timing_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/timing_cal/correcter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/src/naludaq/tools/waiter/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/waiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-06-02 05:15:17.000000 naludaq-0.27.0/src/naludaq/tools/waiter/eventwaiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/src/naludaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-06-02 05:15:26.000000 naludaq-0.27.0/src/naludaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-06-02 05:15:26.000000 naludaq-0.27.0/src/naludaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 05:15:26.000000 naludaq-0.27.0/src/naludaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-02 05:15:26.000000 naludaq-0.27.0/src/naludaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-06-02 05:15:26.000000 naludaq-0.27.0/src/naludaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 05:15:26.300168 naludaq-0.27.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-02 05:15:17.000000 naludaq-0.27.0/tests/test_naludaq.py
```

### Comparing `naludaq-0.26.5/LICENSE.txt` & `naludaq-0.27.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/PKG-INFO` & `naludaq-0.27.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.5
+Version: 0.27.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.5/README.md` & `naludaq-0.27.0/README.md`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/pyproject.toml` & `naludaq-0.27.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/setup.py` & `naludaq-0.27.0/setup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/__init__.py` & `naludaq-0.27.0/src/naludaq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/client.py` & `naludaq-0.27.0/src/naludaq/backend/client.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/context.py` & `naludaq-0.27.0/src/naludaq/backend/context.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/exceptions.py` & `naludaq-0.27.0/src/naludaq/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/managers/acquisitions.py` & `naludaq-0.27.0/src/naludaq/backend/managers/acquisitions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/managers/config.py` & `naludaq-0.27.0/src/naludaq/backend/managers/config.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/managers/connection.py` & `naludaq-0.27.0/src/naludaq/backend/managers/connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/managers/io.py` & `naludaq-0.27.0/src/naludaq/backend/managers/io.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/models/acquisition.py` & `naludaq-0.27.0/src/naludaq/backend/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/backend/models/device.py` & `naludaq-0.27.0/src/naludaq/backend/models/device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/__init__.py` & `naludaq-0.27.0/src/naludaq/board/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/board_inits.py` & `naludaq-0.27.0/src/naludaq/board/board_inits.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import time
 
 from naludaq.backend.managers.connection import ConnectionManager
 from naludaq.board.initializers import Initializers
 from naludaq.board.initializers.aardvarcv3 import InitAardvarcv3
 from naludaq.board.initializers.aodsoc import InitAodsoc
 from naludaq.board.initializers.asocv3s import InitASoCv3S
+from naludaq.board.initializers.hiper import InitHiper
 from naludaq.board.initializers.init_aodsv2_eval import InitAodsv2Eval
 from naludaq.board.initializers.init_hdsocv1 import InitHDSoCv1
 from naludaq.board.initializers.init_udc import InitUDC16
 from naludaq.board.initializers.init_upac96 import InitUPAC96
 from naludaq.board.initializers.trbhm import InitTrbhm
 from naludaq.communication import (
     AnalogRegisters,
@@ -54,14 +55,15 @@
             "asocv2": self.init_ASoCv2,
             "asocv3": self.init_ASoCv3,
             "asocv3s": InitASoCv3S,
             "asoc-ml605": self.init_ASoC_ML605,
             "hdsocv1": InitHDSoCv1,
             "hdsocv1_evalr1": InitHDSoCv1,
             "hdsocv1_evalr2": InitHDSoCv1,
+            "hiper": InitHiper,
             "aodsoc_asoc": InitAodsoc,
             "aodsoc_aods": InitAodsoc,
             "siread": self.init_SiREAD,
             "trbhm": InitTrbhm,
             "udc16": InitUDC16,
             "upac96": InitUPAC96,
             "upaci": self.init_upac32,
```

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/_FTDI.py` & `naludaq-0.27.0/src/naludaq/board/connections/_FTDI.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/_MockUART.py` & `naludaq-0.27.0/src/naludaq/board/connections/_MockUART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/_UART.py` & `naludaq-0.27.0/src/naludaq/board/connections/_UART.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/_USB.py` & `naludaq-0.27.0/src/naludaq/board/connections/_USB.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/base_connection.py` & `naludaq-0.27.0/src/naludaq/board/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/connection_factory.py` & `naludaq-0.27.0/src/naludaq/board/connections/connection_factory.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/tcp.py` & `naludaq-0.27.0/src/naludaq/board/connections/tcp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/connections/udp.py` & `naludaq-0.27.0/src/naludaq/board/connections/udp.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/__init__.py` & `naludaq-0.27.0/src/naludaq/board/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/aardvarcv3.py` & `naludaq-0.27.0/src/naludaq/board/initializers/aardvarcv3.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class InitAardvarcv3(Initializers):
     def __init__(self, board):
         """Initializer for the aardvarcv3.
 
         Args:
             board (Board): the board to initialize.
         """
-        super().__init__(board, ["aardvarcv3", "aardvarcv4", "trbhm"])
+        super().__init__(board, ["aardvarcv3", "aardvarcv4", "trbhm", "hiper"])
         self.power_sequence = [
             "2v5_en",
             "1v2_en",
             "3v3_i2c_en",
             "clk2v5_en",
             "clk1v8_en",
             "clk_i2c_sel",
```

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/aodsoc.py` & `naludaq-0.27.0/src/naludaq/board/initializers/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/asocv3s.py` & `naludaq-0.27.0/src/naludaq/board/initializers/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/init_aodsv2_eval.py` & `naludaq-0.27.0/src/naludaq/board/initializers/init_aodsv2_eval.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/init_hdsocv1.py` & `naludaq-0.27.0/src/naludaq/board/initializers/init_hdsocv1.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/init_udc.py` & `naludaq-0.27.0/src/naludaq/board/initializers/init_udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/init_upac96.py` & `naludaq-0.27.0/src/naludaq/board/initializers/init_upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/initializers/trbhm.py` & `naludaq-0.27.0/src/naludaq/board/initializers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/board/params.py` & `naludaq-0.27.0/src/naludaq/board/params.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/__init__.py` & `naludaq-0.27.0/src/naludaq/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/_chip.py` & `naludaq-0.27.0/src/naludaq/communication/_chip.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/_common.py` & `naludaq-0.27.0/src/naludaq/communication/_common.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/_fpga.py` & `naludaq-0.27.0/src/naludaq/communication/_fpga.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/analog_registers.py` & `naludaq-0.27.0/src/naludaq/communication/analog_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/chip_selection.py` & `naludaq-0.27.0/src/naludaq/communication/chip_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     Args:
         board: the board
 
     Returns:
         list[int]: list of selected chips
     """
     fn = {
+        "hiper": _selected_chips_hiper,
         "aodsoc_asoc": _selected_chips_aodsoc,
         "aodsoc_aods": _selected_chips_aodsoc,
         "trbhm": _selected_chips_aodsoc,
         "upac96": _selected_chips_upac96,
     }.get(board.model, None)
     result = []
     if fn is not None:
@@ -105,26 +106,38 @@
         board (Board): the board
         chips (list[int]): list of chips to enable
 
     Returns:
         str: _description_
     """
     fn = {
+        "hiper": _select_chips_command_hiper,
         "aodsoc_asoc": _select_chips_command_aodsoc,
         "aodsoc_aods": _select_chips_command_aodsoc,
         "trbhm": _select_chips_command_aodsoc,
         "upac96": _select_chips_command_upac96,
     }.get(board.model, None)
 
     command = ""
     if fn is not None:
         command = fn(board, chips)
     return command
 
 
+def _select_chips_command_hiper(board, chips: list[int]) -> str:
+    """Chip select command generator for aodsoc boards"""
+    mask = _build_chip_mask_or_raise(board.params, chips)
+    return _generate_commands(
+        board,
+        {
+            "rxout_en": mask,
+        },
+    )
+
+
 def _select_chips_command_aodsoc(board, chips: list[int]) -> str:
     """Chip select command generator for aodsoc boards"""
     mask = _build_chip_mask_or_raise(board.params, chips)
     return _generate_commands(
         board,
         {
             "ard_tx_en": mask,
@@ -138,14 +151,24 @@
     mask = _build_chip_mask_or_raise(board.params, chips)
     writes = {"udc_rxout_enable": mask}
     if len(chips) != 0:
         writes["udc_select"] = chips[0]
     return _generate_commands(board, writes)
 
 
+def _selected_chips_hiper(board) -> list[int]:
+    """Get selected chips for an aodsoc board"""
+    mask = board.registers["control_registers"]["rxout_en"]["value"]
+    numchips = board.params["num_chips"]
+    maxval = 2**numchips - 1
+    mask = max(0, min(mask, maxval))
+    chiplist = _build_chip_list_or_raise(mask)
+    return chiplist
+
+
 def _selected_chips_aodsoc(board) -> list[int]:
     """Get selected chips for an aodsoc board"""
     mask = board.registers["control_registers"]["ard_rx_en"]["value"]
     return _build_chip_list_or_raise(mask)
 
 
 def _selected_chips_upac96(board) -> list[int]:
```

### Comparing `naludaq-0.26.5/src/naludaq/communication/control_registers.py` & `naludaq-0.27.0/src/naludaq/communication/control_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/digital_registers.py` & `naludaq-0.27.0/src/naludaq/communication/digital_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/i2c.py` & `naludaq-0.27.0/src/naludaq/communication/i2c.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/i2c_registers.py` & `naludaq-0.27.0/src/naludaq/communication/i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/communication/registers.py` & `naludaq-0.27.0/src/naludaq/communication/registers.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/analog_debug_controller.py` & `naludaq-0.27.0/src/naludaq/controllers/analog_debug_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/biasing_mode/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/biasing_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/biasing_mode/udc16.py` & `naludaq-0.27.0/src/naludaq/controllers/biasing_mode/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/board/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 import logging
 
 from .aodsoc import BoardControllerAodsoc
 from .asocv3s import ASoCv3SBoardController
 from .default import BoardController
 from .hdsoc import HDSoCBoardController
+from .hiper import BoardControllerHiper
 from .oleas import BoardControllerOleas
 from .trbhm import TrbhmBoardController
 from .udc import UDCBoardController
 from .upac import UpacBoardController
 from .upac96 import UPAC96BoardController
 
 LOGGER = logging.getLogger(__name__)  # pylint: disable=invalid-name
@@ -32,14 +33,15 @@
         # 'aodsoc_aods': BoardControllerAodsoc,
         "aodsoc_aods": BoardControllerOleas,
         "aodsoc_asoc": BoardControllerAodsoc,
         "hdsocv1": HDSoCBoardController,
         "hdsocv1_evalr1": HDSoCBoardController,
         "hdsocv1_evalr2": HDSoCBoardController,
         "asocv3s": ASoCv3SBoardController,
+        "hiper": BoardControllerHiper,
         "trbhm": TrbhmBoardController,
         "udc16": UDCBoardController,
         "upac32": UpacBoardController,
         "upaci": UpacBoardController,
         "upac96": UPAC96BoardController,
         "zdigitizer": UpacBoardController,
     }.get(board.model, BoardController)(board)
```

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/aodsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/board/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/asocv3s.py` & `naludaq-0.27.0/src/naludaq/controllers/board/asocv3s.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/default.py` & `naludaq-0.27.0/src/naludaq/controllers/board/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/board/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/oleas.py` & `naludaq-0.27.0/src/naludaq/controllers/board/oleas.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/trbhm.py` & `naludaq-0.27.0/src/naludaq/controllers/board/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/udc.py` & `naludaq-0.27.0/src/naludaq/controllers/board/udc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/upac.py` & `naludaq-0.27.0/src/naludaq/controllers/board/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/board/upac96.py` & `naludaq-0.27.0/src/naludaq/controllers/board/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/connection/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/connection/connection_controller.py` & `naludaq-0.27.0/src/naludaq/controllers/connection/connection_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/connection/upac.py` & `naludaq-0.27.0/src/naludaq/controllers/connection/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/connection/upac96.py` & `naludaq-0.27.0/src/naludaq/controllers/connection/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from .aardvarcv3 import DacControllerAardvarcv3
 from .ad5671 import DACControllerAD5671
 from .ad5675 import DACControllerAD5675
 from .base import BaseDACController as _DACController
 from .dac7578 import DACControllerDAC7578
 from .hdsoc import DACControllerHDSoC
+from .hiper import DACControllerHiper
 from .trbhm import DACControllerTRBHM
 from .upac32 import DacControllerUpac32
 
 
 def get_dac_controller(board) -> _DACController:
     """Gets the DAC controller appropriate for a given board.
 
@@ -50,14 +51,15 @@
         "aodsv1": DACControllerAD5671,
         "aodsv2_eval": DACControllerAD5671,
         "asocv3": DACControllerAD5671,
         "asocv3s": DACControllerAD5671,
         "hdsocv1": DACControllerHDSoC,
         "hdsocv1_evalr1": DACControllerHDSoC,
         "hdsocv1_evalr2": DACControllerHDSoC,
+        "hiper": DACControllerHiper,
         "trbhm": DACControllerTRBHM,
         "udc16": DACControllerDAC7578,
         "upac32": DacControllerUpac32,
         "upac96": DACControllerDAC7578,
         "aodsoc_aods": DACControllerDAC7578,
         "aodsoc_asoc": DACControllerDAC7578,
     }.get(board.model, None)
```

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/aardvarcv3.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/ad5671.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/ad5671.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/ad5675.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/ad5675.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/base.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/dac7578.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/dac7578.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/i2c_dac.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/i2c_dac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/trbhm.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/external_dac/upac32.py` & `naludaq-0.27.0/src/naludaq/controllers/external_dac/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/gainstages/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/gainstages/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/gainstages/aodsv2.py` & `naludaq-0.27.0/src/naludaq/controllers/gainstages/aodsv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/gainstages/oddsock_aods.py` & `naludaq-0.27.0/src/naludaq/controllers/gainstages/oddsock_aods.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/aardvarcv3.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/aodsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/peripherals_controller.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/peripherals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/upac.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/peripherals/upac96.py` & `naludaq-0.27.0/src/naludaq/controllers/peripherals/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/project_controller.py` & `naludaq-0.27.0/src/naludaq/controllers/project_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .aardvarcv3 import Aardvarcv3ReadoutController
 from .asocv3 import Asocv3ReadoutController
 from .default import ReadoutController
 from .hdsoc import HDSoCReadoutController
+from .hiper import HiperReadoutController
 from .trbhm import TrbhmReadoutController
 
 
 def get_readout_controller(board):
     """Gets the readout controller which is appropriate for the given board.
 
     hdsocv1 -> HDSoCReadoutController
@@ -20,13 +21,14 @@
     """
     return {
         "hdsocv1": HDSoCReadoutController,
         "hdsocv1_evalr1": HDSoCReadoutController,
         "hdsocv1_evalr2": HDSoCReadoutController,
         "aardvarcv3": Aardvarcv3ReadoutController,
         "aardvarcv4": Aardvarcv3ReadoutController,
+        "hiper": HiperReadoutController,
         "asocv3": Asocv3ReadoutController,
         "asocv3s": Asocv3ReadoutController,
         "trbhm": TrbhmReadoutController,
         "aodsoc_aods": TrbhmReadoutController,
         "aodsoc_asoc": TrbhmReadoutController,
     }.get(board.model, ReadoutController)(board)
```

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/aardvarcv3.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/aardvarcv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/asocv3.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/asocv3.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/default.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/readout/trbhm.py` & `naludaq-0.27.0/src/naludaq/controllers/readout/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/si5341_controller.py` & `naludaq-0.27.0/src/naludaq/controllers/si5341_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/tia/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/tia/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/tia/base.py` & `naludaq-0.27.0/src/naludaq/controllers/tia/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/tia/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/tia/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/__init__.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/aodsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/aodsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/default.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/hdsoc.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/trbhm.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/upac.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/upac.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/controllers/trigger/upac96.py` & `naludaq-0.27.0/src/naludaq/controllers/trigger/upac96.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/__init__.py` & `naludaq-0.27.0/src/naludaq/daq/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from naludaq.board.connections.base_serial import BaseSerialConnection
 from naludaq.daq.debugdaq import DebugDaq
 from naludaq.daq.debugdaq import DebugDaq as BenDaq
+from naludaq.daq.hiperdaq import HiperDaq
 from naludaq.daq.lightdaq import LightDaq
 
 
 def get_daq(board, *args, parsed: bool = False, debug: bool = False, **kwargs):
     """Return an instantiated Daq object based on model and preferences.
 
     Args:
@@ -15,8 +16,11 @@
     Returns:
         Instantiated daq object
     """
     daq = LightDaq
     if debug or parsed:
         daq = DebugDaq
 
+    elif board.params["model"] in ["hiper"]:
+        daq = HiperDaq
+
     return daq(board, *args, **kwargs)
```

### Comparing `naludaq-0.26.5/src/naludaq/daq/debugdaq.py` & `naludaq-0.27.0/src/naludaq/daq/debugdaq.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from naludaq.daq.workers.packager import DebugPackager, get_packager
 from naludaq.daq.workers.worker_parser import ParserWorkerLight
 from naludaq.parsers import get_parser
 
 LOGGER = getLogger(__name__)
 
 HDSOC_PACKAGER = ["hdsocv1", "hdsocv1_evalr1", "hdsocv1_evalr2"]
+HIPER_PACKAGER = ["hiper"]
 
 
 class DebugDaq:
     def __init__(self, board, store_raw_data=False, custom_parser=None):
         """Creates a DAQ used to collect data readouts from the given board.
 
         Args:
@@ -169,14 +170,24 @@
             dp = get_packager(
                 self.board,
                 self.serial_to_packager_buffer,
                 # raw_buffer,
                 self.packager_to_parser_buffer,
                 self.intermittent_answers_buffer,
                 self.board.params["stop_word"],
+                1000,
+            )
+        elif self.board.params["model"] in HIPER_PACKAGER:
+            dp = get_packager(
+                self.board,
+                self.serial_to_packager_buffer,
+                # raw_buffer,
+                self.packager_to_parser_buffer,
+                self.intermittent_answers_buffer,
+                self.board.params["stop_word"],
                 1000,
             )
         else:
             dp = DebugPackager(
                 # self.board,
                 self.serial_to_packager_buffer,
                 raw_buffer,
```

### Comparing `naludaq-0.26.5/src/naludaq/daq/lightdaq.py` & `naludaq-0.27.0/src/naludaq/daq/lightdaq.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/preprocess.py` & `naludaq-0.27.0/src/naludaq/daq/preprocess.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/__init__.py` & `naludaq-0.27.0/src/naludaq/daq/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/answer_parser_worker.py` & `naludaq-0.27.0/src/naludaq/daq/workers/answer_parser_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/csv_storage_worker.py` & `naludaq-0.27.0/src/naludaq/daq/workers/csv_storage_worker.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager.py` & `naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
  raw_data': bytesarray()
 }
 
 """
 
 import logging
 import time
-from collections import deque
+from queue import Queue
 from threading import Thread
+from typing import MutableSequence
 
 logger = logging.getLogger("naludaq.packager")
 
 
 ##############################################################################
 class OldPackagerLight(Thread):
     """Drop in replacement for the Packager but without the zmq stuff.
@@ -171,17 +172,17 @@
     """Drop in replacement for the Packager but without the zmq stuff.
 
     Significantly slower, beware.
     """
 
     def __init__(
         self,
-        input_buffer: deque,
-        output_buffer: deque,
-        output_answers: deque,
+        input_buffer: MutableSequence,
+        output_buffer: MutableSequence,
+        output_answers: Queue,
         stop_word: bytes,
         frequency: int,
     ):
         """Prepares a thread (not open) which polls the input buffer and pops all data in it
         into a internal buffer. Depending on frequency, it will slice the internal
         buffer once it reaches a stop word, and store the sliced data into an
         output_buffer for parsing. If there are answers within the data, it will separate it
@@ -381,23 +382,23 @@
             while self.running:
                 frametime = time.perf_counter()
 
                 for _ in range(len(self.input_buffer)):
                     try:
                         internal_buffer.extend(self.input_buffer.pop())
                     except:
-                        logger.error("can't pop!")
+                        logger.error("can't pop from input buffer.")
 
                 if internal_buffer:
                     rest = self._route_serial_data(internal_buffer)
                     internal_buffer = bytearray(rest)
 
                 if self._reset_pkg_num:
                     self._pkg_num = 0
                     self._reset_pkg_num = False
 
                 try:
                     time.sleep(frametime + self._interval - time.perf_counter())
-                except ValueError:
-                    pass
+                finally:
+                    continue
         except KeyboardInterrupt:
-            pass
+            self.running = False
```

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager_debug.py` & `naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager_debug.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py` & `naludaq-0.27.0/src/naludaq/daq/workers/packager/worker_packager_hdsoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/postprocessing.py` & `naludaq-0.27.0/src/naludaq/daq/workers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/worker_parser.py` & `naludaq-0.27.0/src/naludaq/daq/workers/worker_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/worker_serial_reader.py` & `naludaq-0.27.0/src/naludaq/daq/workers/worker_serial_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/daq/workers/worker_usb_reader.py` & `naludaq-0.27.0/src/naludaq/daq/workers/worker_usb_reader.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/devices/eeprom.py` & `naludaq-0.27.0/src/naludaq/devices/eeprom.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/devices/i2c_device.py` & `naludaq-0.27.0/src/naludaq/devices/i2c_device.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/devices/ltc2990.py` & `naludaq-0.27.0/src/naludaq/devices/ltc2990.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/decorators.py` & `naludaq-0.27.0/src/naludaq/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/exceptions.py` & `naludaq-0.27.0/src/naludaq/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/fancyiter.py` & `naludaq-0.27.0/src/naludaq/helpers/fancyiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/helper_functions.py` & `naludaq-0.27.0/src/naludaq/helpers/helper_functions.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/operations.py` & `naludaq-0.27.0/src/naludaq/helpers/operations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/register_cache.py` & `naludaq-0.27.0/src/naludaq/helpers/register_cache.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/semiton.py` & `naludaq-0.27.0/src/naludaq/helpers/semiton.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/helpers/validations.py` & `naludaq-0.27.0/src/naludaq/helpers/validations.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/io/__init__.py` & `naludaq-0.27.0/src/naludaq/io/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/io/csv_writer.py` & `naludaq-0.27.0/src/naludaq/io/csv_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/io/hdf5.py` & `naludaq-0.27.0/src/naludaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/io/io_manager.py` & `naludaq-0.27.0/src/naludaq/io/io_manager.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/models/acq_converters.py` & `naludaq-0.27.0/src/naludaq/models/acq_converters.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/models/acquisition.py` & `naludaq-0.27.0/src/naludaq/models/acquisition.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/naludaq.py` & `naludaq-0.27.0/src/naludaq/naludaq.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from naludaq.backend import AcquisitionManager, RemoteAcquisition
 from naludaq.backend.exceptions import BackendError
 from naludaq.board import init_hardware, startup_board
 from naludaq.controllers import get_board_controller, get_readout_controller
 from naludaq.controllers.trigger import get_trigger_controller
 from naludaq.daq import LightDaq as DataAcquisitionController
+from naludaq.daq.hiperdaq import HiperDaq as hDAQ
 from naludaq.daq.preprocess import Preprocess
 from naludaq.helpers import event_transfer_time
 from naludaq.io import io_manager
 from naludaq.tools.pedestals import get_pedestals_controller
 from naludaq.tools.waiter import EventWaiter
 
 LOGGER = getLogger(__name__)
@@ -503,7 +504,72 @@
 
     def _current_output_buffer_len(self) -> int:
         """Get the current number of events in the output buffer"""
         if self.board.using_new_backend:
             return len(AcquisitionManager(self.board).current_acquisition or [])
         else:
             return len(self.daq.output_buffer)
+
+
+class HiperDaq(NaluDaq):
+    """Special HACK adapter for the upac board.
+
+    Need to be cleaned up with a proper factory.
+    """
+
+    def __init__(self, board, working_dir, *args, start_workers=True, **kwargs):
+        super().__init__(board, working_dir, start_workers=True)
+        if not self.board.using_new_backend:
+            self.daq = hDAQ(self.board, working_dir, start_workers)
+            self.daq.preprocess = Preprocess(board)
+        self.chips: list = [0]
+        self.read_amount = 0
+        self.readout_settings = {
+            "trig": "ext",
+            "lb": "forced",
+            "acq": "raw",
+            "dig_head": False,
+            "ped": "zero",
+            "readoutEn": True,
+            "singleEv": False,
+        }
+
+    def select_readout_chips(self, chips_to_read):
+        self.chips = chips_to_read
+
+    def reset_board(self):
+        """Reset the board.
+
+        Sends a digital reset command to the board and resets the fpga.
+        It will not wipe any settings made by the user.
+        """
+        get_board_controller(self.board).reset_board()
+
+    def capture_event(self):
+        """Send a trigger pulse to the board"""
+        get_board_controller(self.board).toggle_trigger()
+
+    def start_acquisition(self):
+        """Start acquiring data from the board and store it.
+
+        Make sure to swap the output storage before starting.
+
+        Args:
+            readouts(int): Maximum amount of readouts, 0 = infinite
+        """
+        self.is_capturing = True
+        bc = get_board_controller(self.board)
+        self.daq.pkg_num = 0
+        self.daq.start_capture()
+        bc.start_readout(**self.readout_settings)
+
+    def stop_acquisition(self):
+        """Stop acquiring data."""
+        if self.board.connection is not None:
+            try:
+                get_board_controller(self.board).stop_readout()  # Nuke the board
+            except Exception as error_msg:
+                LOGGER.warning("stop_acquisition can't stop due to: %s", error_msg)
+        self.daq.stop_capture()
+        self.daq.pkg_num = 0
+        self.is_capturing = False
+        self.daq.get_buffer_levels()
```

### Comparing `naludaq-0.26.5/src/naludaq/parsers/__init__.py` & `naludaq-0.27.0/src/naludaq/parsers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from . import answer_parser
 from .aardvarcv3_parser import Aardvarcv3Parser
 from .aodsoc_parser import OddsockParser
 from .asocv3_parser import ASoCv3Parser
 from .asocv3s_parser import ASoCv3SParser
 from .hdsoc_parser import HDSoCParser
 from .headers import get_header_parser
+from .hiper_parser import HiperParser
 from .parser import Parser
 from .trbhm_parser import TRBHMParser
 from .udc_parser import UDCParser
 from .upac96_parser import Upac96Parser
 from .upac_parser import UPACParser
 
 PARSERS = {
@@ -17,14 +18,15 @@
     "aodsoc_aods": OddsockParser,
     "aodsoc_asoc": OddsockParser,
     "asocv3": ASoCv3Parser,
     "asocv3s": ASoCv3SParser,
     "hdsocv1": HDSoCParser,
     "hdsocv1_evalr1": HDSoCParser,
     "hdsocv1_evalr2": HDSoCParser,
+    "hiper": HiperParser,
     "trbhm": TRBHMParser,
     "udc16": UDCParser,
     "upac32": UPACParser,
     "upac96": Upac96Parser,
     "upaci": UPACParser,
     "zdigitizer": UPACParser,
 }
```

### Comparing `naludaq-0.26.5/src/naludaq/parsers/aardvarcv3_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/aardvarcv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/answer_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/answer_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/aodsoc_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/aodsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/asocv3_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/asocv3_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/asocv3s_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/asocv3s_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/hdsoc_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/hdsoc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/__init__.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/asoc.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/asoc.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/asocv2.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/asocv2.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/base.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/base.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/siread.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/siread.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/trbhm.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/trbhm.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/headers/upac32.py` & `naludaq-0.27.0/src/naludaq/parsers/headers/upac32.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/parser.py` & `naludaq-0.27.0/src/naludaq/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/trbhm_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/trbhm_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/udc_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/udc_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/upac96_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/upac96_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/parsers/upac_parser.py` & `naludaq-0.27.0/src/naludaq/parsers/upac_parser.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/adc2mv/adc_converter.py` & `naludaq-0.27.0/src/naludaq/tools/adc2mv/adc_converter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/adc2mv/adc_linear_regression.py` & `naludaq-0.27.0/src/naludaq/tools/adc2mv/adc_linear_regression.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/adc2mv/generate.py` & `naludaq-0.27.0/src/naludaq/tools/adc2mv/generate.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/adc2mv/pre_adc2mv.py` & `naludaq-0.27.0/src/naludaq/tools/adc2mv/pre_adc2mv.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/autoaction.py` & `naludaq-0.27.0/src/naludaq/tools/autoaction.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/autotrigger/default.py` & `naludaq-0.27.0/src/naludaq/tools/autotrigger/default.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/board_backup.py` & `naludaq-0.27.0/src/naludaq/tools/board_backup.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/dac_sweep/dac_sweep_controller.py` & `naludaq-0.27.0/src/naludaq/tools/dac_sweep/dac_sweep_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/data_collector/_daq_interface.py` & `naludaq-0.27.0/src/naludaq/tools/data_collector/_daq_interface.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/data_collector/default.py` & `naludaq-0.27.0/src/naludaq/tools/data_collector/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             interface.stop_capture()
 
     # ================================================================================
     # Readout
     # ================================================================================
     def _start_readout(self):
         """Start a readout"""
-        logger.info("Starting readout")
+        logger.info("Starting readout using: %s", self._readout_settings)
         get_board_controller(self._board).start_readout(**self._readout_settings)
 
     def _stop_readout(self):
         """Stop the readout"""
         logger.info("Stopping readout")
         get_board_controller(self._board).stop_readout()
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/data_collector/udc16.py` & `naludaq-0.27.0/src/naludaq/tools/data_collector/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/features.py` & `naludaq-0.27.0/src/naludaq/tools/features.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/ft60x.py` & `naludaq-0.27.0/src/naludaq/tools/ft60x.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/ftdi.py` & `naludaq-0.27.0/src/naludaq/tools/ftdi.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/lookup_table/lookup_table.py` & `naludaq-0.27.0/src/naludaq/tools/lookup_table/lookup_table.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/lookup_table/lookup_table_generator.py` & `naludaq-0.27.0/src/naludaq/tools/lookup_table/lookup_table_generator.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/metadata.py` & `naludaq-0.27.0/src/naludaq/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/optimizers/bayesian_optimizer.py` & `naludaq-0.27.0/src/naludaq/tools/optimizers/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/__init__.py` & `naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py` & `naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/channel_writer.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/optimizers/conversion_ramp/udc16.py` & `naludaq-0.27.0/src/naludaq/tools/optimizers/conversion_ramp/udc16.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/optimizers/gainstagetuner.py` & `naludaq-0.27.0/src/naludaq/tools/optimizers/gainstagetuner.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/__init__.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/generators/__init__.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/generators/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .default import PedestalsGenerator
 from .hdsoc import PedestalsGeneratorHdsoc
+from .hiper import PedestalsGeneratorHiper
 from .udc16 import PedestalsGeneratorUdc16
 from .upac96 import PedestalsGeneratorUpac96
 
 
 def get_pedestals_generator(
     board,
     num_captures: int = 10,
@@ -32,9 +33,10 @@
     if board.model in ["upac32", "upaci", "zdigitizer"]:
         raise NotImplementedError("Board is currently unsupported")
 
     classy = {
         "hdsocv1_evalr2": PedestalsGeneratorHdsoc,
         "udc16": PedestalsGeneratorUdc16,
         "upac96": PedestalsGeneratorUpac96,
+        "hiper": PedestalsGeneratorHiper,
     }.get(board.model, PedestalsGenerator)
     return classy(board, num_captures, num_warmup_events, channels)
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/generators/default.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/generators/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,17 @@
 
         self._progress = []
         self._cancel = False
 
         self.num_captures = num_captures
         self.num_warmup_events = num_warmup_events
         self.block_size = self.board.params["pedestals_blocks"]
+        self._dc = get_data_collector(board)
         self.channels = channels or range(self.board.channels)
 
-        self._dc = get_data_collector(board)
         self._dc.channels = self.channels
         self._dc.forced = True
         self._dc.timeout_overhead = timeout_overhead or self.board.params.get(
             "timeout_overhead", 10.0
         )
         self._current_block = 0
         self._current_start_window = 0
@@ -148,20 +148,20 @@
         self._progress = value
 
     @property
     def channels(self) -> list[int]:
         """Get/set the channels that will be read out. Any channels not enabled will result
         in NANs for that channel.
         """
-        return self._channels
+        return self._dc.channels
 
     @channels.setter
     def channels(self, channels: Iterable[int]):
         validations.validate_channel_sequence_or_raise(self.board.params, channels)
-        self._channels = list(channels)
+        self._dc.channels = list(channels)
 
     @property
     def num_captures(self) -> int:
         """Get/set the number of events per block."""
         return self._num_captures
 
     @num_captures.setter
@@ -315,15 +315,15 @@
             PedestalsDataCaptureError: if pedestals failed to generate.
             OperationCanceledError: if pedestals generation was cancelled.
         """
         LOGGER.debug(
             "Capturing pedestals for %s. Block size=%s, channels=%s",
             self.board.model,
             self.block_size,
-            self._channels,
+            self.channels,
         )
         self._current_block = 0
         blocks = []
         total_windows = self.board.params["windows"]
         for start_window in range(0, total_windows, self.block_size):
             self._raise_if_canceled()
             self._set_read_window(start_window)
@@ -427,15 +427,15 @@
         Args:
             event (dict): event to validate
             expected_block (list): a list of expected window numbers
 
         Returns:
             True if validated, False if the events windows doesn't match expected.
         """
-        test_channel = self._channels[0]
+        test_channel = self.channels[0]
         try:
             if np.all(event["window_labels"][test_channel] == expected_window_labels):
                 return True
         except Exception as error_msg:
             LOGGER.error(f"Event validation failed due to: {error_msg}")
             return False
         LOGGER.warning(
@@ -505,28 +505,38 @@
             blocks (list[list[dict]]): blocks to store
         """
         block_size = self.block_size
         raw_data = self.board.pedestals["rawdata"]
         for block_idx, block in enumerate(blocks):
             for capture_number, event in enumerate(block):
                 for chan in range(self.board.params["channels"]):
-                    if chan not in self._channels:
+                    if chan not in self.channels:
                         continue
                     for window_num in range(block_size):
                         window = window_num + block_idx * block_size
                         # Avoid rolling over and overwrite block 0
                         if block_idx != 0 and (window < block_size):
                             continue
                         # avoid window number rolling over
                         if window >= self.board.params["windows"]:
                             continue
                         for sample in range(self.board.params["samples"]):
                             index = sample + window_num * self.board.params["samples"]
-                            data = event["data"][chan][index]
-                            raw_data[chan, window, sample][capture_number] = data
+                            try:
+                                data = event["data"][chan][index]
+
+                                raw_data[chan, window, sample][capture_number] = data
+                            except Exception as e:
+                                LOGGER.debug(
+                                    "Event doesn't contain data, block: %s, capnum: %s, chan %s, idx: %s",
+                                    block_idx,
+                                    capture_number,
+                                    chan,
+                                    index,
+                                )
 
     def _store_averaged_data(self):
         """Generate processed pedestals data from the raw data."""
         raw_data = self.board.pedestals["rawdata"]
         self.board.pedestals["data"] = np.nanmean(raw_data, axis=3)
 
     # ================================================================================
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/generators/hdsoc.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/generators/hdsoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         return block_size
 
     def _validate_event(self, event: dict, expected_window_labels: list[int]) -> bool:
         """Reimplemented to check all channels.
 
         Windows can be missing from individual channels on HDSoC.
         """
-        for channel in self._channels:
+        for channel in self.channels:
             labels = event["window_labels"][channel]
             try:
                 is_bad = np.any(labels != expected_window_labels)
             except Exception as error_msg:
                 LOGGER.error(f"Event validation failed due to: {error_msg}")
                 return False
             if is_bad:
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/generators/udc16.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/generators/udc16.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         Raises:
             PedestalsDataCaptureError: if pedestals failed to generate.
             OperationCanceledError: if pedestals generation was cancelled.
         """
         LOGGER.debug(
             "Capturing pedestals for %s. channels=%s",
             self.board.model,
-            self._channels,
+            self.channels,
         )
         get_actual_count = lambda events: np.min(
             self._get_window_counts(events)[self.channels]
         )
         pipeline = (
             self._create_data_pipeline()
             .accumulated()
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/generators/upac96.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/generators/upac96.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,26 +57,26 @@
         """Check if the event has a data field, which means it's parsed"""
         self._last_event_channels = []
         if "data" not in event:
             LOGGER.warning("Got an invalid event")
             return False
         chans_with_data = [i for i, x in enumerate(event.get("data", [])) if len(x) > 0]
         self._last_event_channels = chans_with_data
-        is_superset = set(chans_with_data).issuperset(self._channels)
+        is_superset = set(chans_with_data).issuperset(self.channels)
         if not is_superset:
             LOGGER.warning(
                 "Got a parseable event, but the channels are incorrect: %s",
                 chans_with_data,
             )
         return is_superset
 
     def _exc_str(self, e: Exception) -> str:
         """Override since UPAC96 can fail on a per-chip basis"""
         missing_channels = find_missing_channels(
-            self._channels, self._last_event_channels
+            self.channels, self._last_event_channels
         )
         # IterationError means we're getting valid data but it's getting filtered
         # out by the constraints in `validate_event()`. Got a custom message for that.
         if not isinstance(e, IterationError) or len(missing_channels) == 0:
             return super()._exc_str(e)
 
         channels_per_chip = self.board.params.get("channels_per_chip", 16)
```

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/pedestals_correcter.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/pedestals_correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/pedestals_processor.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/pedestals_processor.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/pedestals/upac32_pedestals_controller.py` & `naludaq-0.27.0/src/naludaq/tools/pedestals/upac32_pedestals_controller.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/threshold_scan/__init__.py` & `naludaq-0.27.0/src/naludaq/tools/threshold_scan/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py` & `naludaq-0.27.0/src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/threshold_scan/threshold_scan.py` & `naludaq-0.27.0/src/naludaq/tools/threshold_scan/threshold_scan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py` & `naludaq-0.27.0/src/naludaq/tools/threshold_scan/upac96_thresholdscan.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/timing_cal/__init__.py` & `naludaq-0.27.0/src/naludaq/tools/timing_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/timing_cal/calibration.py` & `naludaq-0.27.0/src/naludaq/tools/timing_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/timing_cal/correcter.py` & `naludaq-0.27.0/src/naludaq/tools/timing_cal/correcter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq/tools/waiter/eventwaiter.py` & `naludaq-0.27.0/src/naludaq/tools/waiter/eventwaiter.py`

 * *Files identical despite different names*

### Comparing `naludaq-0.26.5/src/naludaq.egg-info/PKG-INFO` & `naludaq-0.27.0/src/naludaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naludaq
-Version: 0.26.5
+Version: 0.27.0
 Summary: Backend package for Nalu Scientific hardware
 Home-page: 
 Author: Thomas Yang, Emily Lum, Terry Pham
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naludaq-0.26.5/src/naludaq.egg-info/SOURCES.txt` & `naludaq-0.27.0/src/naludaq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/naludaq/board/connections/connection_factory.py
 src/naludaq/board/connections/tcp.py
 src/naludaq/board/connections/udp.py
 src/naludaq/board/initializers/__init__.py
 src/naludaq/board/initializers/aardvarcv3.py
 src/naludaq/board/initializers/aodsoc.py
 src/naludaq/board/initializers/asocv3s.py
+src/naludaq/board/initializers/hiper.py
 src/naludaq/board/initializers/init_aodsv2_eval.py
 src/naludaq/board/initializers/init_hdsocv1.py
 src/naludaq/board/initializers/init_udc.py
 src/naludaq/board/initializers/init_upac96.py
 src/naludaq/board/initializers/trbhm.py
 src/naludaq/communication/__init__.py
 src/naludaq/communication/_chip.py
@@ -65,14 +66,15 @@
 src/naludaq/controllers/biasing_mode/__init__.py
 src/naludaq/controllers/biasing_mode/udc16.py
 src/naludaq/controllers/board/__init__.py
 src/naludaq/controllers/board/aodsoc.py
 src/naludaq/controllers/board/asocv3s.py
 src/naludaq/controllers/board/default.py
 src/naludaq/controllers/board/hdsoc.py
+src/naludaq/controllers/board/hiper.py
 src/naludaq/controllers/board/oleas.py
 src/naludaq/controllers/board/trbhm.py
 src/naludaq/controllers/board/udc.py
 src/naludaq/controllers/board/upac.py
 src/naludaq/controllers/board/upac96.py
 src/naludaq/controllers/connection/__init__.py
 src/naludaq/controllers/connection/connection_controller.py
@@ -81,14 +83,15 @@
 src/naludaq/controllers/external_dac/__init__.py
 src/naludaq/controllers/external_dac/aardvarcv3.py
 src/naludaq/controllers/external_dac/ad5671.py
 src/naludaq/controllers/external_dac/ad5675.py
 src/naludaq/controllers/external_dac/base.py
 src/naludaq/controllers/external_dac/dac7578.py
 src/naludaq/controllers/external_dac/hdsoc.py
+src/naludaq/controllers/external_dac/hiper.py
 src/naludaq/controllers/external_dac/i2c_dac.py
 src/naludaq/controllers/external_dac/trbhm.py
 src/naludaq/controllers/external_dac/upac32.py
 src/naludaq/controllers/gainstages/__init__.py
 src/naludaq/controllers/gainstages/aodsv2.py
 src/naludaq/controllers/gainstages/oddsock_aods.py
 src/naludaq/controllers/peripherals/__init__.py
@@ -99,41 +102,44 @@
 src/naludaq/controllers/peripherals/upac.py
 src/naludaq/controllers/peripherals/upac96.py
 src/naludaq/controllers/readout/__init__.py
 src/naludaq/controllers/readout/aardvarcv3.py
 src/naludaq/controllers/readout/asocv3.py
 src/naludaq/controllers/readout/default.py
 src/naludaq/controllers/readout/hdsoc.py
+src/naludaq/controllers/readout/hiper.py
 src/naludaq/controllers/readout/trbhm.py
 src/naludaq/controllers/tia/__init__.py
 src/naludaq/controllers/tia/base.py
 src/naludaq/controllers/tia/hdsoc.py
 src/naludaq/controllers/trigger/__init__.py
 src/naludaq/controllers/trigger/aodsoc.py
 src/naludaq/controllers/trigger/default.py
 src/naludaq/controllers/trigger/hdsoc.py
 src/naludaq/controllers/trigger/siread.py
 src/naludaq/controllers/trigger/trbhm.py
 src/naludaq/controllers/trigger/upac.py
 src/naludaq/controllers/trigger/upac96.py
 src/naludaq/daq/__init__.py
 src/naludaq/daq/debugdaq.py
+src/naludaq/daq/hiperdaq.py
 src/naludaq/daq/lightdaq.py
 src/naludaq/daq/preprocess.py
 src/naludaq/daq/workers/__init__.py
 src/naludaq/daq/workers/answer_parser_worker.py
 src/naludaq/daq/workers/csv_storage_worker.py
 src/naludaq/daq/workers/postprocessing.py
 src/naludaq/daq/workers/worker_parser.py
 src/naludaq/daq/workers/worker_serial_reader.py
 src/naludaq/daq/workers/worker_usb_reader.py
 src/naludaq/daq/workers/packager/__init__.py
 src/naludaq/daq/workers/packager/worker_packager.py
 src/naludaq/daq/workers/packager/worker_packager_debug.py
 src/naludaq/daq/workers/packager/worker_packager_hdsoc.py
+src/naludaq/daq/workers/packager/worker_packager_hiper.py
 src/naludaq/devices/__init__.py
 src/naludaq/devices/device.py
 src/naludaq/devices/eeprom.py
 src/naludaq/devices/i2c_device.py
 src/naludaq/devices/ltc2990.py
 src/naludaq/helpers/__init__.py
 src/naludaq/helpers/decorators.py
@@ -154,14 +160,15 @@
 src/naludaq/parsers/__init__.py
 src/naludaq/parsers/aardvarcv3_parser.py
 src/naludaq/parsers/answer_parser.py
 src/naludaq/parsers/aodsoc_parser.py
 src/naludaq/parsers/asocv3_parser.py
 src/naludaq/parsers/asocv3s_parser.py
 src/naludaq/parsers/hdsoc_parser.py
+src/naludaq/parsers/hiper_parser.py
 src/naludaq/parsers/parser.py
 src/naludaq/parsers/trbhm_parser.py
 src/naludaq/parsers/udc_parser.py
 src/naludaq/parsers/upac96_parser.py
 src/naludaq/parsers/upac_parser.py
 src/naludaq/parsers/headers/__init__.py
 src/naludaq/parsers/headers/asoc.py
@@ -202,14 +209,15 @@
 src/naludaq/tools/pedestals/__init__.py
 src/naludaq/tools/pedestals/pedestals_correcter.py
 src/naludaq/tools/pedestals/pedestals_processor.py
 src/naludaq/tools/pedestals/upac32_pedestals_controller.py
 src/naludaq/tools/pedestals/generators/__init__.py
 src/naludaq/tools/pedestals/generators/default.py
 src/naludaq/tools/pedestals/generators/hdsoc.py
+src/naludaq/tools/pedestals/generators/hiper.py
 src/naludaq/tools/pedestals/generators/udc16.py
 src/naludaq/tools/pedestals/generators/upac96.py
 src/naludaq/tools/threshold_scan/__init__.py
 src/naludaq/tools/threshold_scan/hdsoc_thresholdscan.py
 src/naludaq/tools/threshold_scan/threshold_scan.py
 src/naludaq/tools/threshold_scan/upac96_thresholdscan.py
 src/naludaq/tools/timing_cal/__init__.py
```

