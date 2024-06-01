# Comparing `tmp/mpflash-0.8.0.tar.gz` & `tmp/mpflash-0.8.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpflash-0.8.0.tar", max compression
+gzip compressed data, was "mpflash-0.8.1b1.tar", max compression
```

## Comparing `mpflash-0.8.0.tar` & `mpflash-0.8.1b1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.8.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.8.0/mpflash/__init__.py
--rw-r--r--   0        0        0     3435 2024-05-22 21:29:21.517582 mpflash-0.8.0/mpflash/add_firmware.py
--rw-r--r--   0        0        0     8496 2024-05-27 21:07:02.040121 mpflash-0.8.0/mpflash/ask_input.py
--rw-r--r--   0        0        0     3645 2024-05-27 21:03:47.978786 mpflash-0.8.0/mpflash/cli_download.py
--rw-r--r--   0        0        0     7074 2024-05-27 21:24:52.546385 mpflash-0.8.0/mpflash/cli_flash.py
--rw-r--r--   0        0        0     1974 2024-05-27 21:03:47.983988 mpflash-0.8.0/mpflash/cli_group.py
--rw-r--r--   0        0        0     1997 2024-05-27 21:03:47.983988 mpflash-0.8.0/mpflash/cli_list.py
--rw-r--r--   0        0        0     1030 2024-06-01 12:56:07.150733 mpflash-0.8.0/mpflash/cli_main.py
--rw-r--r--   0        0        0     5594 2024-06-01 11:40:47.253016 mpflash-0.8.0/mpflash/common.py
--rw-r--r--   0        0        0      495 2024-05-27 21:03:47.991712 mpflash-0.8.0/mpflash/config.py
--rw-r--r--   0        0        0     3029 2024-05-27 21:03:47.992049 mpflash-0.8.0/mpflash/connected.py
--rw-r--r--   0        0        0    11421 2024-06-01 11:29:24.977288 mpflash-0.8.0/mpflash/download.py
--rw-r--r--   0        0        0     3804 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/downloaded.py
--rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.8.0/mpflash/errors.py
--rw-r--r--   0        0        0     2468 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash.py
--rw-r--r--   0        0        0     2311 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_esp.py
--rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32.py
--rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32_cube.py
--rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.8.0/mpflash/flash_stm32_dfu.py
--rw-r--r--   0        0        0     2508 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_uf2.py
--rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.8.0/mpflash/flash_uf2_boardid.py
--rw-r--r--   0        0        0     4055 2024-05-27 21:03:47.993017 mpflash-0.8.0/mpflash/flash_uf2_linux.py
--rw-r--r--   0        0        0     2696 2024-05-27 21:03:48.002459 mpflash-0.8.0/mpflash/flash_uf2_macos.py
--rw-r--r--   0        0        0     1093 2024-05-03 13:05:36.160916 mpflash-0.8.0/mpflash/flash_uf2_windows.py
--rw-r--r--   0        0        0     2963 2024-05-27 21:03:48.002459 mpflash-0.8.0/mpflash/list.py
--rw-r--r--   0        0        0     1098 2024-05-09 18:26:02.794085 mpflash-0.8.0/mpflash/logger.py
--rw-r--r--   0        0        0     3576 2024-06-01 12:35:35.666067 mpflash-0.8.0/mpflash/mpboard_id/__init__.py
--rw-r--r--   0        0        0     9684 2024-06-01 13:17:03.471049 mpflash-0.8.0/mpflash/mpboard_id/add_boards.py
--rw-r--r--   0        0        0     1151 2024-06-01 12:35:24.218389 mpflash-0.8.0/mpflash/mpboard_id/board.py
--rw-r--r--   0        0        0     2489 2024-06-01 12:32:47.930044 mpflash-0.8.0/mpflash/mpboard_id/board_id.py
--rw-r--r--   0        0        0    19759 2024-06-01 13:17:49.539026 mpflash-0.8.0/mpflash/mpboard_id/board_info.zip
--rw-r--r--   0        0        0     1462 2024-06-01 12:41:26.069251 mpflash-0.8.0/mpflash/mpboard_id/store.py
--rw-r--r--   0        0        0     7683 2024-05-10 21:00:04.227607 mpflash-0.8.0/mpflash/mpremoteboard/__init__.py
--rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.8.0/mpflash/mpremoteboard/mpy_fw_info.py
--rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.8.0/mpflash/mpremoteboard/runner.py
--rw-r--r--   0        0        0      298 2024-05-27 21:03:48.006614 mpflash-0.8.0/mpflash/uf2disk.py
--rw-r--r--   0        0        0     9545 2024-05-27 21:03:57.348737 mpflash-0.8.0/mpflash/vendor/basicgit.py
--rw-r--r--   0        0        0     5755 2024-05-27 21:03:48.006614 mpflash-0.8.0/mpflash/vendor/dfu.py
--rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.8.0/mpflash/vendor/pydfu.py
--rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.8.0/mpflash/vendor/readme.md
--rw-r--r--   0        0        0     3783 2024-05-27 21:06:13.964512 mpflash-0.8.0/mpflash/vendor/versions.py
--rw-r--r--   0        0        0     5962 2024-06-01 12:14:29.624478 mpflash-0.8.0/mpflash/worklist.py
--rw-r--r--   0        0        0     1651 2024-06-01 13:22:52.017074 mpflash-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    13680 2024-05-27 21:03:47.974599 mpflash-0.8.0/README.md
--rw-r--r--   0        0        0    15224 1970-01-01 00:00:00.000000 mpflash-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-05 22:17:23.926920 mpflash-0.8.1b1/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 22:17:23.927891 mpflash-0.8.1b1/mpflash/__init__.py
+-rw-r--r--   0        0        0     3435 2024-06-01 13:47:27.343277 mpflash-0.8.1b1/mpflash/add_firmware.py
+-rw-r--r--   0        0        0     8496 2024-06-01 13:47:27.343277 mpflash-0.8.1b1/mpflash/ask_input.py
+-rw-r--r--   0        0        0     3645 2024-06-01 13:59:42.079358 mpflash-0.8.1b1/mpflash/cli_download.py
+-rw-r--r--   0        0        0     7074 2024-06-01 13:47:27.351444 mpflash-0.8.1b1/mpflash/cli_flash.py
+-rw-r--r--   0        0        0     1974 2024-06-01 13:47:27.353895 mpflash-0.8.1b1/mpflash/cli_group.py
+-rw-r--r--   0        0        0     1997 2024-06-01 13:47:27.355744 mpflash-0.8.1b1/mpflash/cli_list.py
+-rw-r--r--   0        0        0     1030 2024-06-01 13:47:27.355744 mpflash-0.8.1b1/mpflash/cli_main.py
+-rw-r--r--   0        0        0     5594 2024-06-01 13:47:27.355744 mpflash-0.8.1b1/mpflash/common.py
+-rw-r--r--   0        0        0      495 2024-05-27 21:03:47.991712 mpflash-0.8.1b1/mpflash/config.py
+-rw-r--r--   0        0        0     3029 2024-06-01 13:47:27.355744 mpflash-0.8.1b1/mpflash/connected.py
+-rw-r--r--   0        0        0    11612 2024-06-01 14:08:45.151281 mpflash-0.8.1b1/mpflash/download.py
+-rw-r--r--   0        0        0     3804 2024-06-01 13:47:27.366119 mpflash-0.8.1b1/mpflash/downloaded.py
+-rw-r--r--   0        0        0       96 2024-04-29 18:55:09.413103 mpflash-0.8.1b1/mpflash/errors.py
+-rw-r--r--   0        0        0     2468 2024-06-01 13:47:27.366423 mpflash-0.8.1b1/mpflash/flash.py
+-rw-r--r--   0        0        0     2311 2024-06-01 13:47:27.366423 mpflash-0.8.1b1/mpflash/flash_esp.py
+-rw-r--r--   0        0        0      823 2024-04-29 18:55:09.416103 mpflash-0.8.1b1/mpflash/flash_stm32.py
+-rw-r--r--   0        0        0     3970 2024-04-29 18:55:09.416103 mpflash-0.8.1b1/mpflash/flash_stm32_cube.py
+-rw-r--r--   0        0        0     2972 2024-04-29 18:55:09.416103 mpflash-0.8.1b1/mpflash/flash_stm32_dfu.py
+-rw-r--r--   0        0        0     2463 2024-06-01 19:58:29.953979 mpflash-0.8.1b1/mpflash/flash_uf2.py
+-rw-r--r--   0        0        0      414 2024-04-05 19:52:32.892053 mpflash-0.8.1b1/mpflash/flash_uf2_boardid.py
+-rw-r--r--   0        0        0     4055 2024-06-01 13:47:27.366423 mpflash-0.8.1b1/mpflash/flash_uf2_linux.py
+-rw-r--r--   0        0        0     1078 2024-06-01 19:56:12.326406 mpflash-0.8.1b1/mpflash/flash_uf2_macos.py
+-rw-r--r--   0        0        0     1025 2024-06-01 19:57:10.161120 mpflash-0.8.1b1/mpflash/flash_uf2_windows.py
+-rw-r--r--   0        0        0     2963 2024-06-01 13:47:27.366423 mpflash-0.8.1b1/mpflash/list.py
+-rw-r--r--   0        0        0     1098 2024-05-09 18:26:02.794085 mpflash-0.8.1b1/mpflash/logger.py
+-rw-r--r--   0        0        0     3576 2024-06-01 13:47:27.380133 mpflash-0.8.1b1/mpflash/mpboard_id/__init__.py
+-rw-r--r--   0        0        0     9684 2024-06-01 13:47:27.380133 mpflash-0.8.1b1/mpflash/mpboard_id/add_boards.py
+-rw-r--r--   0        0        0     1151 2024-06-01 13:47:27.380133 mpflash-0.8.1b1/mpflash/mpboard_id/board.py
+-rw-r--r--   0        0        0     2489 2024-06-01 13:47:27.380133 mpflash-0.8.1b1/mpflash/mpboard_id/board_id.py
+-rw-r--r--   0        0        0    19759 2024-06-01 13:47:27.388873 mpflash-0.8.1b1/mpflash/mpboard_id/board_info.zip
+-rw-r--r--   0        0        0     1462 2024-06-01 13:47:27.391764 mpflash-0.8.1b1/mpflash/mpboard_id/store.py
+-rw-r--r--   0        0        0     7683 2024-05-10 21:00:04.227607 mpflash-0.8.1b1/mpflash/mpremoteboard/__init__.py
+-rw-r--r--   0        0        0     4554 2024-03-12 12:49:58.751813 mpflash-0.8.1b1/mpflash/mpremoteboard/mpy_fw_info.py
+-rw-r--r--   0        0        0     4786 2024-04-29 20:58:49.567039 mpflash-0.8.1b1/mpflash/mpremoteboard/runner.py
+-rw-r--r--   0        0        0      298 2024-05-27 21:03:48.006614 mpflash-0.8.1b1/mpflash/uf2disk.py
+-rw-r--r--   0        0        0     9545 2024-06-01 13:47:27.393545 mpflash-0.8.1b1/mpflash/vendor/basicgit.py
+-rw-r--r--   0        0        0     5755 2024-06-01 13:47:27.393545 mpflash-0.8.1b1/mpflash/vendor/dfu.py
+-rw-r--r--   0        0        0    20542 2024-04-29 18:55:09.423435 mpflash-0.8.1b1/mpflash/vendor/pydfu.py
+-rw-r--r--   0        0        0       86 2024-04-29 18:55:09.424458 mpflash-0.8.1b1/mpflash/vendor/readme.md
+-rw-r--r--   0        0        0     3783 2024-06-01 13:47:27.393545 mpflash-0.8.1b1/mpflash/vendor/versions.py
+-rw-r--r--   0        0        0     5962 2024-06-01 13:47:27.393545 mpflash-0.8.1b1/mpflash/worklist.py
+-rw-r--r--   0        0        0     1653 2024-06-01 20:03:18.809633 mpflash-0.8.1b1/pyproject.toml
+-rw-r--r--   0        0        0    13680 2024-05-27 21:03:47.974599 mpflash-0.8.1b1/README.md
+-rw-r--r--   0        0        0    15226 1970-01-01 00:00:00.000000 mpflash-0.8.1b1/PKG-INFO
```

### Comparing `mpflash-0.8.0/LICENSE` & `mpflash-0.8.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/add_firmware.py` & `mpflash-0.8.1b1/mpflash/add_firmware.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/ask_input.py` & `mpflash-0.8.1b1/mpflash/ask_input.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/cli_download.py` & `mpflash-0.8.1b1/mpflash/cli_download.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/cli_flash.py` & `mpflash-0.8.1b1/mpflash/cli_flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/cli_group.py` & `mpflash-0.8.1b1/mpflash/cli_group.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/cli_list.py` & `mpflash-0.8.1b1/mpflash/cli_list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/cli_main.py` & `mpflash-0.8.1b1/mpflash/cli_main.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/common.py` & `mpflash-0.8.1b1/mpflash/common.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/connected.py` & `mpflash-0.8.1b1/mpflash/connected.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/download.py` & `mpflash-0.8.1b1/mpflash/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,9 +286,14 @@
         raise MPFlashError("No boards found")
     # versions = [clean_version(v, drop_v=True) for v in versions]  # remove leading v from version
     try:
         destination.mkdir(exist_ok=True, parents=True)
     except (PermissionError, FileNotFoundError) as e:
         log.critical(f"Could not create folder {destination}")
         raise MPFlashError(f"Could not create folder {destination}") from e
+    try:
+        result = download_firmwares(destination, ports, boards, versions, force=force, clean=clean)
+    except requests.exceptions.RequestException as e:
+        log.exception(e)
+        raise MPFlashError("Could not connect to micropython.org") from e
 
-    return download_firmwares(destination, ports, boards, versions, force=force, clean=clean)
+    return result
```

### Comparing `mpflash-0.8.0/mpflash/downloaded.py` & `mpflash-0.8.1b1/mpflash/downloaded.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash.py` & `mpflash-0.8.1b1/mpflash/flash.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_esp.py` & `mpflash-0.8.1b1/mpflash/flash_esp.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_stm32.py` & `mpflash-0.8.1b1/mpflash/flash_stm32.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_stm32_cube.py` & `mpflash-0.8.1b1/mpflash/flash_stm32_cube.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_stm32_dfu.py` & `mpflash-0.8.1b1/mpflash/flash_stm32_dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_uf2.py` & `mpflash-0.8.1b1/mpflash/flash_uf2.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from loguru import logger as log
 from rich.progress import track
 
 from mpflash.mpremoteboard import MPRemoteBoard
 
 from .common import PORT_FWTYPES
-from .config import config
+from .flash_uf2_boardid import get_board_id
 from .flash_uf2_linux import dismount_uf2_linux, wait_for_UF2_linux
 from .flash_uf2_macos import wait_for_UF2_macos
 from .flash_uf2_windows import wait_for_UF2_windows
 
 
 def flash_uf2(mcu: MPRemoteBoard, fw_file: Path, erase: bool) -> Optional[MPRemoteBoard]:
     """
@@ -41,28 +41,26 @@
 
     if sys.platform == "linux":
         destination = wait_for_UF2_linux()
     elif sys.platform == "win32":
         destination = wait_for_UF2_windows()
     elif sys.platform == "darwin":
         log.warning(f"OS {sys.platform} not tested/supported")
-        # TODO: test which of the options is best
-        if "macos_uf2" in config.tests:
-            destination = wait_for_UF2_macos()
-        else:
-            destination = wait_for_UF2_linux()
+        destination = wait_for_UF2_macos()
     else:
         log.warning(f"OS {sys.platform} not tested/supported")
         return None
 
     if not destination or not destination.exists() or not (destination / "INFO_UF2.TXT").exists():
         log.error("Board is not in bootloader mode")
         return None
 
     log.info("Board is in bootloader mode")
+    board_id = get_board_id(destination)  # type: ignore
+    log.info(f"Board ID: {board_id}")
     log.info(f"Copying {fw_file} to {destination}.")
     shutil.copy(fw_file, destination)
     log.success("Done copying, resetting the board and wait for it to restart")
     if sys.platform in ["linux"]:
         dismount_uf2_linux()
     for _ in track(range(5 + 2), description="Waiting for the board to restart", transient=True, refresh_per_second=2):
         time.sleep(1)  # 5 secs to short on linux
```

### Comparing `mpflash-0.8.0/mpflash/flash_uf2_linux.py` & `mpflash-0.8.1b1/mpflash/flash_uf2_linux.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/flash_uf2_windows.py` & `mpflash-0.8.1b1/mpflash/flash_uf2_windows.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # sourcery skip: snake-case-functions
 """Flash a MCU with a UF2 bootloader on Windows"""
 
 from __future__ import annotations
 
 import time
 from pathlib import Path
+from typing import Optional
 
 import psutil
 from rich.progress import track
 
-from .flash_uf2_boardid import get_board_id
 
 
-def wait_for_UF2_windows(s_max: int = 10):
+
+def wait_for_UF2_windows(s_max: int = 10) -> Optional[Path]:
     """Wait for the MCU to mount as a drive"""
     if s_max < 1:
         s_max = 10
-    destination = ""
+    destination = None
     for _ in track(range(s_max), description="Waiting for mcu to mount as a drive", transient=True,refresh_per_second=2):
         # log.info(f"Waiting for mcu to mount as a drive : {n} seconds left")
         drives = [drive.device for drive in psutil.disk_partitions()]
         for drive in drives:
             try:
                 if Path(drive, "INFO_UF2.TXT").exists():
-                    board_id = get_board_id(Path(drive))  # type: ignore
                     destination = Path(drive)
                     break
             except OSError:
                 pass
         if destination:
             break
         time.sleep(1)
```

### Comparing `mpflash-0.8.0/mpflash/list.py` & `mpflash-0.8.1b1/mpflash/list.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/logger.py` & `mpflash-0.8.1b1/mpflash/logger.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/__init__.py` & `mpflash-0.8.1b1/mpflash/mpboard_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/add_boards.py` & `mpflash-0.8.1b1/mpflash/mpboard_id/add_boards.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/board.py` & `mpflash-0.8.1b1/mpflash/mpboard_id/board.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/board_id.py` & `mpflash-0.8.1b1/mpflash/mpboard_id/board_id.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/board_info.zip` & `mpflash-0.8.1b1/mpflash/mpboard_id/board_info.zip`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpboard_id/store.py` & `mpflash-0.8.1b1/mpflash/mpboard_id/store.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpremoteboard/__init__.py` & `mpflash-0.8.1b1/mpflash/mpremoteboard/__init__.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpremoteboard/mpy_fw_info.py` & `mpflash-0.8.1b1/mpflash/mpremoteboard/mpy_fw_info.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/mpremoteboard/runner.py` & `mpflash-0.8.1b1/mpflash/mpremoteboard/runner.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/vendor/basicgit.py` & `mpflash-0.8.1b1/mpflash/vendor/basicgit.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/vendor/dfu.py` & `mpflash-0.8.1b1/mpflash/vendor/dfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/vendor/pydfu.py` & `mpflash-0.8.1b1/mpflash/vendor/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/vendor/versions.py` & `mpflash-0.8.1b1/mpflash/vendor/versions.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/mpflash/worklist.py` & `mpflash-0.8.1b1/mpflash/worklist.py`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/pyproject.toml` & `mpflash-0.8.1b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpflash"
-version = "0.8.0"
+version = "0.8.1b1"
 description = "Flash and download tool for MicroPython firmwares"
 authors = ["Jos Verlinde <jos_verlinde@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["MicroPython", "firmware", "flash", "download", "UF2", "esptool"]
 homepage = "https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md"
 repository = "https://github.com/Josverl/micropython-stubber"
```

### Comparing `mpflash-0.8.0/README.md` & `mpflash-0.8.1b1/README.md`

 * *Files identical despite different names*

### Comparing `mpflash-0.8.0/PKG-INFO` & `mpflash-0.8.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpflash
-Version: 0.8.0
+Version: 0.8.1b1
 Summary: Flash and download tool for MicroPython firmwares
 Home-page: https://github.com/Josverl/micropython-stubber/blob/main/src/mpflash/README.md
 License: MIT
 Keywords: MicroPython,firmware,flash,download,UF2,esptool
 Author: Jos Verlinde
 Author-email: jos_verlinde@hotmail.com
 Requires-Python: >=3.8.1,<4.0
```

