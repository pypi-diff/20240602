# Comparing `tmp/libretro_py-0.1.2.tar.gz` & `tmp/libretro_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_py-0.1.2.tar", last modified: Fri May 31 22:35:44 2024, max compression
+gzip compressed data, was "libretro_py-0.1.3.tar", last modified: Sun Jun  2 16:29:14 2024, max compression
```

## Comparing `libretro_py-0.1.2.tar` & `libretro_py-0.1.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.541933 libretro_py-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-31 22:34:46.000000 libretro_py-0.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 22:34:46.000000 libretro_py-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 22:34:46.000000 libretro_py-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-31 22:35:44.541933 libretro_py-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-31 22:34:46.000000 libretro_py-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-31 22:34:46.000000 libretro_py-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 22:35:44.541933 libretro_py-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 22:34:46.000000 libretro_py-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.513933 libretro_py-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.517933 libretro_py-0.1.2/src/libretro/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/av.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/api/input/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/analog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/joypad.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/lightgun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/input/pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/midi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/netpacket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/perf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/rumble.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/savestate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/vfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/api/video/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/video/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/video/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/video/negotiate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/api/video/render.py
--rw-r--r--   0 runner    (1001) docker     (127)    29812 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/drivers/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/audio/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/audio/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/audio/wave.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.525933 libretro_py-0.1.2/src/libretro/drivers/camera/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/camera/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/camera/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/content/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/content/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/content/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/disk/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/disk/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/environment/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/environment/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/environment/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/environment/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/input/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/input/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    21421 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/input/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/led/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/led/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/led/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/location/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/location/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/location/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/log/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/log/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/log/unformatted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.529933 libretro_py-0.1.2/src/libretro/drivers/message/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/message/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/message/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/microphone/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/microphone/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/midi/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/midi/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/midi/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/netpacket/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/netpacket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/netpacket/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/netpacket/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/options/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/options/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/options/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/path/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/path/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/path/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/perf/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/perf/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/perf/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/power/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/power/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/rumble/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/rumble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/rumble/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/rumble/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.533933 libretro_py-0.1.2/src/libretro/drivers/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/sensor/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/sensor/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/timing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/timing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/timing/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/timing/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/user/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/user/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/user/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/vfs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/vfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/vfs/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/vfs/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/vfs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/video/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/multi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/video/opengl/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/opengl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25214 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/opengl/moderngl.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/opengl/moderngl_frag.glsl
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/opengl/moderngl_vertex.glsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro/drivers/video/software/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/software/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/drivers/video/software/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/h.py
--rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-05-31 22:34:46.000000 libretro_py-0.1.2/src/libretro/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:35:44.537933 libretro_py-0.1.2/src/libretro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-31 22:35:44.000000 libretro_py-0.1.2/src/libretro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-31 22:35:44.000000 libretro_py-0.1.2/src/libretro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:35:44.000000 libretro_py-0.1.2/src/libretro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 22:35:44.000000 libretro_py-0.1.2/src/libretro.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 22:35:44.000000 libretro_py-0.1.2/src/libretro.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.246910 libretro_py-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-06-02 16:28:17.000000 libretro_py-0.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-02 16:28:17.000000 libretro_py-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 16:28:17.000000 libretro_py-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-06-02 16:29:14.246910 libretro_py-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-06-02 16:28:17.000000 libretro_py-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-02 16:28:17.000000 libretro_py-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 16:29:14.246910 libretro_py-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-06-02 16:28:17.000000 libretro_py-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.218911 libretro_py-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.226911 libretro_py-0.1.3/src/libretro/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.230911 libretro_py-0.1.3/src/libretro/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/av.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.230911 libretro_py-0.1.3/src/libretro/api/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/analog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/joypad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/lightgun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/input/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/midi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/netpacket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/rumble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/savestate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/api/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/video/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/video/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/video/negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/api/video/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29812 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/audio/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/audio/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/audio/wave.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/camera/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/camera/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/content/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/content/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/content/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/disk/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/environment/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/environment/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/environment/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/environment/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/input/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21421 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/input/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.234911 libretro_py-0.1.3/src/libretro/drivers/led/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/led/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/led/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/location/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/location/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/location/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/log/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/log/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/log/unformatted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/message/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/message/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/message/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/microphone/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/microphone/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/midi/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/midi/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/netpacket/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/netpacket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/netpacket/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/netpacket/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/options/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/options/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/options/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.238911 libretro_py-0.1.3/src/libretro/drivers/path/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/path/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/path/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/perf/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/perf/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/power/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/power/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/rumble/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/rumble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/rumble/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/rumble/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/sensor/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/sensor/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/timing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/timing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/timing/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/timing/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/user/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/user/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/vfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/vfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/vfs/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9069 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/vfs/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/vfs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.242910 libretro_py-0.1.3/src/libretro/drivers/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.246910 libretro_py-0.1.3/src/libretro/drivers/video/opengl/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/opengl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25298 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/opengl/moderngl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/opengl/moderngl_frag.glsl
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/opengl/moderngl_vertex.glsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.246910 libretro_py-0.1.3/src/libretro/drivers/video/software/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/software/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/drivers/video/software/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/h.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-06-02 16:28:17.000000 libretro_py-0.1.3/src/libretro/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 16:29:14.246910 libretro_py-0.1.3/src/libretro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-06-02 16:29:14.000000 libretro_py-0.1.3/src/libretro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-06-02 16:29:14.000000 libretro_py-0.1.3/src/libretro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 16:29:14.000000 libretro_py-0.1.3/src/libretro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-02 16:29:14.000000 libretro_py-0.1.3/src/libretro.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-02 16:29:14.000000 libretro_py-0.1.3/src/libretro.py.egg-info/top_level.txt
```

### Comparing `libretro_py-0.1.2/CHANGELOG.md` & `libretro_py-0.1.3/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 > [!ATTENTION]
 > Until libretro.py reaches version 1.x,
 > breaking changes may be introduced
 > at any time without warning.
 
+## [0.1.3] - 2024-06-02
+
+### Fixed
+
+- Fixed a bug where logging invalid UTF-8 characters in `UnformattedLogDriver` would raise an exception.
+- Fixed a bug where fetching an unset option from a `DictOptionDriver` wouldn't register the default value for next time.
+- Fixed a bug where `ModernGlVideoDriver` would try to use OpenGL debugging features even if they weren't available.
+
 ## [0.1.2] - 2024-05-31
 
 ### Fixed
 
 - Fixed the GLSL shaders used by `ModernGlVideoDriver` not being included in distributions.
 
 ## [0.1.1] - 2024-05-31
```

### Comparing `libretro_py-0.1.2/LICENSE` & `libretro_py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/PKG-INFO` & `libretro_py-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretro.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A libretro frontend for Python intended for testing cores.
 Author-email: Jesse Talavera <jesse@jesse.tg>
 Maintainer-email: Jesse Talavera <jesse@jesse.tg>
 License: MIT License
 Project-URL: Homepage, https://github.com/JesseTG/libretro.py
 Project-URL: Issues, https://github.com/JesseTG/libretro.py/issues
 Project-URL: Repository, https://github.com/JesseTG/libretro.py
```

### Comparing `libretro_py-0.1.2/README.md` & `libretro_py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/pyproject.toml` & `libretro_py-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/setup.py` & `libretro_py-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/_utils.py` & `libretro_py-0.1.3/src/libretro/_utils.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/__init__.py` & `libretro_py-0.1.3/src/libretro/api/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/_utils.py` & `libretro_py-0.1.3/src/libretro/api/_utils.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/audio.py` & `libretro_py-0.1.3/src/libretro/api/audio.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/av.py` & `libretro_py-0.1.3/src/libretro/api/av.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/camera.py` & `libretro_py-0.1.3/src/libretro/api/camera.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/content.py` & `libretro_py-0.1.3/src/libretro/api/content.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/disk.py` & `libretro_py-0.1.3/src/libretro/api/disk.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/environment.py` & `libretro_py-0.1.3/src/libretro/api/environment.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/analog.py` & `libretro_py-0.1.3/src/libretro/api/input/analog.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/device.py` & `libretro_py-0.1.3/src/libretro/api/input/device.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/joypad.py` & `libretro_py-0.1.3/src/libretro/api/input/joypad.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/keyboard.py` & `libretro_py-0.1.3/src/libretro/api/input/keyboard.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/lightgun.py` & `libretro_py-0.1.3/src/libretro/api/input/lightgun.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/mouse.py` & `libretro_py-0.1.3/src/libretro/api/input/mouse.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/input/pointer.py` & `libretro_py-0.1.3/src/libretro/api/input/pointer.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/location.py` & `libretro_py-0.1.3/src/libretro/api/location.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/log.py` & `libretro_py-0.1.3/src/libretro/api/log.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/memory.py` & `libretro_py-0.1.3/src/libretro/api/memory.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/message.py` & `libretro_py-0.1.3/src/libretro/api/message.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/microphone.py` & `libretro_py-0.1.3/src/libretro/api/microphone.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/midi.py` & `libretro_py-0.1.3/src/libretro/api/midi.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/netpacket.py` & `libretro_py-0.1.3/src/libretro/api/netpacket.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/options.py` & `libretro_py-0.1.3/src/libretro/api/options.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/perf.py` & `libretro_py-0.1.3/src/libretro/api/perf.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/power.py` & `libretro_py-0.1.3/src/libretro/api/power.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/proc.py` & `libretro_py-0.1.3/src/libretro/api/proc.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/rumble.py` & `libretro_py-0.1.3/src/libretro/api/rumble.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/savestate.py` & `libretro_py-0.1.3/src/libretro/api/savestate.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/sensor.py` & `libretro_py-0.1.3/src/libretro/api/sensor.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/timing.py` & `libretro_py-0.1.3/src/libretro/api/timing.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/user.py` & `libretro_py-0.1.3/src/libretro/api/user.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/vfs.py` & `libretro_py-0.1.3/src/libretro/api/vfs.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/video/context.py` & `libretro_py-0.1.3/src/libretro/api/video/context.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/video/frame.py` & `libretro_py-0.1.3/src/libretro/api/video/frame.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/video/negotiate.py` & `libretro_py-0.1.3/src/libretro/api/video/negotiate.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/api/video/render.py` & `libretro_py-0.1.3/src/libretro/api/video/render.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/builder.py` & `libretro_py-0.1.3/src/libretro/builder.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/core.py` & `libretro_py-0.1.3/src/libretro/core.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/__init__.py` & `libretro_py-0.1.3/src/libretro/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/audio/array.py` & `libretro_py-0.1.3/src/libretro/drivers/audio/array.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/audio/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/audio/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/audio/wave.py` & `libretro_py-0.1.3/src/libretro/drivers/audio/wave.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/camera/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/camera/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/camera/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/camera/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/content/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/content/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/content/standard.py` & `libretro_py-0.1.3/src/libretro/drivers/content/standard.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/disk/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/disk/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/environment/composite.py` & `libretro_py-0.1.3/src/libretro/drivers/environment/composite.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/environment/default.py` & `libretro_py-0.1.3/src/libretro/drivers/environment/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/environment/dict.py` & `libretro_py-0.1.3/src/libretro/drivers/environment/dict.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/environment/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/environment/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/input/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/input/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/input/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/input/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/led/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/led/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/location/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/location/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/location/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/location/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/log/unformatted.py` & `libretro_py-0.1.3/src/libretro/drivers/log/unformatted.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,11 +24,11 @@
             self._logger.addFilter(_log_record)
 
     @property
     def records(self) -> Sequence[LogRecord]:
         return self._records
 
     def log(self, level: LogLevel, fmt: bytes, *args) -> None:
-        self._logger.log(level.logging_level, fmt.decode().rstrip())
+        self._logger.log(level.logging_level, fmt.decode(errors="replace").rstrip())
 
 
 __all__ = ["UnformattedLogDriver"]
```

### Comparing `libretro_py-0.1.2/src/libretro/drivers/message/logger.py` & `libretro_py-0.1.3/src/libretro/drivers/message/logger.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/microphone/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/microphone/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/microphone/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/microphone/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/midi/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/midi/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/midi/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/midi/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/netpacket/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/netpacket/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/netpacket/socket.py` & `libretro_py-0.1.3/src/libretro/drivers/netpacket/socket.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/options/dict.py` & `libretro_py-0.1.3/src/libretro/drivers/options/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,21 @@
 
         key = as_bytes(item)
 
         if key not in self._options_us:
             # For invalid keys, return None
             return None
 
-        if key not in self._variables:
-            # For unset options, return the default value
-            return string_at(self._options_us[key].default_value)
-
-        value = self._variables[key]
+        if key in self._variables:
+            # If we have a value for this option key...
+            value = self._variables[key]
+        else:
+            # Otherwise get the default value and save it to the dict
+            value = string_at(self._options_us[key].default_value)
+            self._variables[key] = value
 
         if value not in (string_at(v.value) for v in self._options_us[key].values if v.value):
             # For invalid values, return None
             return string_at(self._options_us[key].default_value)
 
         return self._variables[key]
```

### Comparing `libretro_py-0.1.2/src/libretro/drivers/options/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/options/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/path/default.py` & `libretro_py-0.1.3/src/libretro/drivers/path/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/path/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/path/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/perf/default.py` & `libretro_py-0.1.3/src/libretro/drivers/perf/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/perf/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/perf/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/power/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/power/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/rumble/default.py` & `libretro_py-0.1.3/src/libretro/drivers/rumble/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/rumble/interface.py` & `libretro_py-0.1.3/src/libretro/drivers/rumble/interface.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/sensor/generator.py` & `libretro_py-0.1.3/src/libretro/drivers/sensor/generator.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/sensor/interface.py` & `libretro_py-0.1.3/src/libretro/drivers/sensor/interface.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/timing/default.py` & `libretro_py-0.1.3/src/libretro/drivers/timing/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/timing/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/timing/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/user/default.py` & `libretro_py-0.1.3/src/libretro/drivers/user/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/vfs/default.py` & `libretro_py-0.1.3/src/libretro/drivers/vfs/default.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/vfs/history.py` & `libretro_py-0.1.3/src/libretro/drivers/vfs/history.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/vfs/interface.py` & `libretro_py-0.1.3/src/libretro/drivers/vfs/interface.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/video/driver.py` & `libretro_py-0.1.3/src/libretro/drivers/video/driver.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/video/multi.py` & `libretro_py-0.1.3/src/libretro/drivers/video/multi.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/video/opengl/moderngl.py` & `libretro_py-0.1.3/src/libretro/drivers/video/opengl/moderngl.py`

 * *Files 2% similar despite different names*

```diff
@@ -422,15 +422,15 @@
         self._shader_program["mvp"].write(mvp)
         self._vbo = self._context.buffer(_VERTEXES)
         self._vao = self._context.vertex_array(
             self._shader_program, self._vbo, "vertexCoord", "texCoord"
         )
         # TODO: Make the particular names configurable
 
-        if self._has_debug:
+        if self._has_debug and GL.glObjectLabel:
             GL.glObjectLabel(
                 GL.GL_PROGRAM, self._shader_program.glo, -1, b"libretro.py Shader Program"
             )
             GL.glObjectLabel(GL.GL_BUFFER, self._vbo.glo, -1, b"libretro.py Screen VBO")
             GL.glObjectLabel(GL.GL_VERTEX_ARRAY, self._vao.glo, -1, b"libretro.py Screen VAO")
 
         # TODO: Honor debug_context; enable debugging features if requested
@@ -620,15 +620,15 @@
         # Similar to glGenTextures, glBindTexture, and glTexImage2D
         self._color = self._context.texture(size, 4)
         self._depth = self._context.depth_renderbuffer(size)
 
         # Similar to glGenFramebuffers, glBindFramebuffer, and glFramebufferTexture2D
         self._fbo = self._context.framebuffer(self._color, self._depth)
 
-        if self._has_debug:
+        if self._has_debug and GL.glObjectLabel:
             GL.glObjectLabel(
                 GL.GL_TEXTURE, self._color.glo, -1, b"libretro.py Main FBO Color Attachment"
             )
             GL.glObjectLabel(
                 GL.GL_RENDERBUFFER, self._depth.glo, -1, b"libretro.py Main FBO Depth Attachment"
             )
             GL.glObjectLabel(GL.GL_FRAMEBUFFER, self._fbo.glo, -1, b"libretro.py Main FBO")
@@ -663,15 +663,15 @@
 
         # Similar to glGenFramebuffers, glBindFramebuffer, and glFramebufferTexture2D
         self._hw_render_fbo = self._context.framebuffer(
             self._hw_render_color, self._hw_render_depth
         )
         self._hw_render_fbo.clear()
 
-        if self._has_debug:
+        if self._has_debug and GL.glObjectLabel:
             GL.glObjectLabel(
                 GL.GL_FRAMEBUFFER,
                 self._hw_render_fbo.glo,
                 -1,
                 b"libretro.py Hardware Rendering FBO",
             )
             GL.glObjectLabel(
@@ -709,14 +709,14 @@
                 case PixelFormat.RGB1555:
                     GL_RGB5 = 0x8050
                     self._cpu_color = self._context.texture(
                         (width, height), 3, data, internal_format=GL_RGB5
                     )
                     # moderngl can't natively express GL_RGB5
 
-            if self._has_debug:
+            if self._has_debug and GL.glObjectLabel:
                 GL.glObjectLabel(
                     GL.GL_TEXTURE, self._cpu_color.glo, -1, b"libretro.py CPU-Rendered Frame"
                 )
 
 
 __all__ = ["ModernGlVideoDriver"]
```

### Comparing `libretro_py-0.1.2/src/libretro/drivers/video/software/array.py` & `libretro_py-0.1.3/src/libretro/drivers/video/software/array.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/drivers/video/software/base.py` & `libretro_py-0.1.3/src/libretro/drivers/video/software/base.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro/session.py` & `libretro_py-0.1.3/src/libretro/session.py`

 * *Files identical despite different names*

### Comparing `libretro_py-0.1.2/src/libretro.py.egg-info/PKG-INFO` & `libretro_py-0.1.3/src/libretro.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretro.py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A libretro frontend for Python intended for testing cores.
 Author-email: Jesse Talavera <jesse@jesse.tg>
 Maintainer-email: Jesse Talavera <jesse@jesse.tg>
 License: MIT License
 Project-URL: Homepage, https://github.com/JesseTG/libretro.py
 Project-URL: Issues, https://github.com/JesseTG/libretro.py/issues
 Project-URL: Repository, https://github.com/JesseTG/libretro.py
```

### Comparing `libretro_py-0.1.2/src/libretro.py.egg-info/SOURCES.txt` & `libretro_py-0.1.3/src/libretro.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

