# Comparing `tmp/tkintertools-3.0.0b1.tar.gz` & `tmp/tkintertools-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-3.0.0b1.tar", last modified: Fri May 17 15:40:55 2024, max compression
+gzip compressed data, was "tkintertools-3.0.0b2.tar", last modified: Sun Jun  2 18:30:18 2024, max compression
```

## Comparing `tkintertools-3.0.0b1.tar` & `tkintertools-3.0.0b2.tar`

### file list

```diff
@@ -1,107 +1,116 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.587236 tkintertools-3.0.0b1/
--rw-rw-rw-   0        0        0     1086 2024-05-05 00:16:47.000000 tkintertools-3.0.0b1/LICENSE.txt
--rw-rw-rw-   0        0        0       35 2024-05-17 15:40:16.000000 tkintertools-3.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     8551 2024-05-17 15:40:55.585733 tkintertools-3.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     6093 2024-05-17 15:04:39.000000 tkintertools-3.0.0b1/README.md
--rw-rw-rw-   0        0        0     1633 2024-05-17 15:40:29.000000 tkintertools-3.0.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 15:40:55.587236 tkintertools-3.0.0b1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.481788 tkintertools-3.0.0b1/tkintertools/
--rw-rw-rw-   0        0        0     2091 2024-05-16 02:19:58.000000 tkintertools-3.0.0b1/tkintertools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.491806 tkintertools-3.0.0b1/tkintertools/animation/
--rw-rw-rw-   0        0        0       86 2024-05-12 12:01:21.000000 tkintertools-3.0.0b1/tkintertools/animation/__init__.py
--rw-rw-rw-   0        0        0     9290 2024-05-17 11:46:35.000000 tkintertools-3.0.0b1/tkintertools/animation/animations.py
--rw-rw-rw-   0        0        0     2838 2024-05-14 13:36:12.000000 tkintertools-3.0.0b1/tkintertools/animation/controllers.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.495807 tkintertools-3.0.0b1/tkintertools/color/
--rw-rw-rw-   0        0        0       72 2024-05-12 12:31:18.000000 tkintertools-3.0.0b1/tkintertools/color/__init__.py
--rw-rw-rw-   0        0        0    25979 2024-05-14 13:41:15.000000 tkintertools-3.0.0b1/tkintertools/color/colormap.py
--rw-rw-rw-   0        0        0     3475 2024-05-16 09:27:41.000000 tkintertools-3.0.0b1/tkintertools/color/rgb.py
--rw-rw-rw-   0        0        0      466 2024-05-17 14:58:42.000000 tkintertools-3.0.0b1/tkintertools/constants.py
--rw-rw-rw-   0        0        0    39879 2024-05-17 12:42:32.000000 tkintertools-3.0.0b1/tkintertools/core.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.503823 tkintertools-3.0.0b1/tkintertools/standard/
--rw-rw-rw-   0        0        0       53 2024-05-15 10:30:54.000000 tkintertools-3.0.0b1/tkintertools/standard/__init__.py
--rw-rw-rw-   0        0        0     3842 2024-05-15 10:30:36.000000 tkintertools-3.0.0b1/tkintertools/standard/dialogs.py
--rw-rw-rw-   0        0        0     8679 2024-05-17 11:51:34.000000 tkintertools-3.0.0b1/tkintertools/standard/features.py
--rw-rw-rw-   0        0        0       27 2024-05-15 02:38:31.000000 tkintertools-3.0.0b1/tkintertools/standard/images.py
--rw-rw-rw-   0        0        0     9544 2024-05-17 13:03:44.000000 tkintertools-3.0.0b1/tkintertools/standard/shapes.py
--rw-rw-rw-   0        0        0     6496 2024-05-16 13:59:22.000000 tkintertools-3.0.0b1/tkintertools/standard/texts.py
--rw-rw-rw-   0        0        0    12748 2024-05-17 12:43:13.000000 tkintertools-3.0.0b1/tkintertools/standard/widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.507327 tkintertools-3.0.0b1/tkintertools/style/
--rw-rw-rw-   0        0        0       72 2024-05-14 13:43:42.000000 tkintertools-3.0.0b1/tkintertools/style/__init__.py
--rw-rw-rw-   0        0        0     2823 2024-05-17 00:33:42.000000 tkintertools-3.0.0b1/tkintertools/style/parser.py
--rw-rw-rw-   0        0        0     3189 2024-05-17 00:34:04.000000 tkintertools-3.0.0b1/tkintertools/style/theme.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.465592 tkintertools-3.0.0b1/tkintertools/theme/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.514842 tkintertools-3.0.0b1/tkintertools/theme/Button/
--rw-rw-rw-   0        0        0      158 2024-05-14 03:31:24.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Information.dark.json
--rw-rw-rw-   0        0        0      158 2024-05-14 03:31:35.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Information.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:26:27.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Rectangle.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:31:53.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/Rectangle.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:21:08.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/RoundedRectangle.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:32:22.000000 tkintertools-3.0.0b1/tkintertools/theme/Button/RoundedRectangle.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.522379 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/
--rw-rw-rw-   0        0        0      158 2024-05-14 03:33:07.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Information.dark.json
--rw-rw-rw-   0        0        0      158 2024-05-14 03:33:17.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Information.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:33:26.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Rectangle.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:33:42.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/Rectangle.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:34:03.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/RoundedRectangle.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:34:34.000000 tkintertools-3.0.0b1/tkintertools/theme/CheckButton/RoundedRectangle.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.532932 tkintertools-3.0.0b1/tkintertools/theme/Entry/
--rw-rw-rw-   0        0        0      251 2024-05-14 03:36:45.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/Rectangle.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:36:56.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/Rectangle.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:37:17.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.in.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:37:41.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.in.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 08:40:52.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.out.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-15 11:36:08.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/RoundedRectangle.out.light.json
--rw-rw-rw-   0        0        0      158 2024-05-14 03:38:44.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/SingleLineText.dark.json
--rw-rw-rw-   0        0        0      158 2024-05-14 03:38:55.000000 tkintertools-3.0.0b1/tkintertools/theme/Entry/SingleLineText.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.535931 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/
--rw-rw-rw-   0        0        0      155 2024-05-14 03:47:15.000000 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/Information.dark.json
--rw-rw-rw-   0        0        0      155 2024-05-14 03:47:23.000000 tkintertools-3.0.0b1/tkintertools/theme/HighlightButton/Information.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.537971 tkintertools-3.0.0b1/tkintertools/theme/Information/
--rw-rw-rw-   0        0        0       55 2024-05-14 03:39:22.000000 tkintertools-3.0.0b1/tkintertools/theme/Information/Information.dark.json
--rw-rw-rw-   0        0        0       55 2024-05-14 03:39:26.000000 tkintertools-3.0.0b1/tkintertools/theme/Information/Information.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.545976 tkintertools-3.0.0b1/tkintertools/theme/Label/
--rw-rw-rw-   0        0        0      106 2024-05-14 03:39:38.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Information.dark.json
--rw-rw-rw-   0        0        0      106 2024-05-14 03:39:46.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Information.light.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:39:54.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Rectangle.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:00.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/Rectangle.light.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:15.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/RoundedRectangle.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Label/RoundedRectangle.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.556897 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:59.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.in.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:41:06.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.in.light.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:44.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.out.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:40:51.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/Rectangle.out.light.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:41:49.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.in.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:42:04.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.in.light.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:41:21.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.out.dark.json
--rw-rw-rw-   0        0        0      168 2024-05-14 03:41:35.000000 tkintertools-3.0.0b1/tkintertools/theme/ProgressBar/SemicircularRectangle.out.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.568070 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:37.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.in.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:47.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.in.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:18.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.out.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:27.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Oval.out.light.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:37.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.in.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-14 03:42:47.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.in.light.json
--rw-rw-rw-   0        0        0      251 2024-05-15 09:23:07.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.out.dark.json
--rw-rw-rw-   0        0        0      251 2024-05-15 09:23:20.000000 tkintertools-3.0.0b1/tkintertools/theme/RadioButton/Rectangle.out.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.578179 tkintertools-3.0.0b1/tkintertools/theme/Switch/
--rw-rw-rw-   0        0        0      520 2024-05-14 03:51:34.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.dark.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:51:45.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.light.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:51:56.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.dark.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:52:05.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.light.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:52:17.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.dark.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:52:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.light.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:53:29.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.dark.json
--rw-rw-rw-   0        0        0      520 2024-05-14 03:54:12.000000 tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.580733 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/
--rw-rw-rw-   0        0        0      159 2024-05-14 03:46:16.000000 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/Information.dark.json
--rw-rw-rw-   0        0        0      154 2024-05-14 03:46:25.000000 tkintertools-3.0.0b1/tkintertools/theme/UnderlineButton/Information.light.json
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.582733 tkintertools-3.0.0b1/tkintertools/three/
--rw-rw-rw-   0        0        0       47 2024-05-14 13:48:22.000000 tkintertools-3.0.0b1/tkintertools/three/__init__.py
--rw-rw-rw-   0        0        0    27170 2024-05-16 06:52:58.000000 tkintertools-3.0.0b1/tkintertools/three/engine.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:40:55.584732 tkintertools-3.0.0b1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0     8551 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3850 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 15:40:55.000000 tkintertools-3.0.0b1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.804802 tkintertools-3.0.0b2/
+-rw-rw-rw-   0        0        0     1088 2024-05-26 00:45:58.000000 tkintertools-3.0.0b2/LICENSE.txt
+-rw-rw-rw-   0        0        0       35 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9996 2024-06-02 18:30:18.803754 tkintertools-3.0.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     7465 2024-06-02 18:26:03.000000 tkintertools-3.0.0b2/README.md
+-rw-rw-rw-   0        0        0     1686 2024-06-02 17:55:05.000000 tkintertools-3.0.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-02 18:30:18.805313 tkintertools-3.0.0b2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.680426 tkintertools-3.0.0b2/tkintertools/
+-rw-rw-rw-   0        0        0     2098 2024-06-02 18:18:20.000000 tkintertools-3.0.0b2/tkintertools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.691602 tkintertools-3.0.0b2/tkintertools/animation/
+-rw-rw-rw-   0        0        0       86 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/animation/__init__.py
+-rw-rw-rw-   0        0        0     9445 2024-06-02 18:17:16.000000 tkintertools-3.0.0b2/tkintertools/animation/animations.py
+-rw-rw-rw-   0        0        0     2929 2024-06-02 18:17:17.000000 tkintertools-3.0.0b2/tkintertools/animation/controllers.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.697594 tkintertools-3.0.0b2/tkintertools/color/
+-rw-rw-rw-   0        0        0       47 2024-06-02 06:50:21.000000 tkintertools-3.0.0b2/tkintertools/color/__init__.py
+-rw-rw-rw-   0        0        0    26035 2024-06-02 18:17:22.000000 tkintertools-3.0.0b2/tkintertools/color/colormap.py
+-rw-rw-rw-   0        0        0     2807 2024-06-02 18:17:23.000000 tkintertools-3.0.0b2/tkintertools/color/hsl.py
+-rw-rw-rw-   0        0        0     3696 2024-06-02 18:17:25.000000 tkintertools-3.0.0b2/tkintertools/color/rgb.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.703077 tkintertools-3.0.0b2/tkintertools/core/
+-rw-rw-rw-   0        0        0       71 2024-06-02 18:15:36.000000 tkintertools-3.0.0b2/tkintertools/core/__init__.py
+-rw-rw-rw-   0        0        0      745 2024-06-02 18:17:30.000000 tkintertools-3.0.0b2/tkintertools/core/constants.py
+-rw-rw-rw-   0        0        0    26392 2024-06-02 18:17:31.000000 tkintertools-3.0.0b2/tkintertools/core/containers.py
+-rw-rw-rw-   0        0        0    15153 2024-06-02 18:17:32.000000 tkintertools-3.0.0b2/tkintertools/core/virtual.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.711724 tkintertools-3.0.0b2/tkintertools/standard/
+-rw-rw-rw-   0        0        0       53 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/standard/__init__.py
+-rw-rw-rw-   0        0        0     3873 2024-06-02 18:17:43.000000 tkintertools-3.0.0b2/tkintertools/standard/dialogs.py
+-rw-rw-rw-   0        0        0     8877 2024-06-02 18:17:44.000000 tkintertools-3.0.0b2/tkintertools/standard/features.py
+-rw-rw-rw-   0        0        0      310 2024-06-02 18:17:45.000000 tkintertools-3.0.0b2/tkintertools/standard/images.py
+-rw-rw-rw-   0        0        0     9997 2024-06-02 18:17:46.000000 tkintertools-3.0.0b2/tkintertools/standard/shapes.py
+-rw-rw-rw-   0        0        0     6618 2024-06-02 18:17:50.000000 tkintertools-3.0.0b2/tkintertools/standard/texts.py
+-rw-rw-rw-   0        0        0    14918 2024-06-02 18:17:51.000000 tkintertools-3.0.0b2/tkintertools/standard/widgets.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.715976 tkintertools-3.0.0b2/tkintertools/style/
+-rw-rw-rw-   0        0        0       72 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/style/__init__.py
+-rw-rw-rw-   0        0        0     2770 2024-06-02 18:17:59.000000 tkintertools-3.0.0b2/tkintertools/style/parser.py
+-rw-rw-rw-   0        0        0     4056 2024-06-02 18:18:00.000000 tkintertools-3.0.0b2/tkintertools/style/theme.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.672763 tkintertools-3.0.0b2/tkintertools/theme/
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.723741 tkintertools-3.0.0b2/tkintertools/theme/Button/
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/Information.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/Information.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Button/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.732461 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/Information.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/Information.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/CheckButton/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.743148 tkintertools-3.0.0b2/tkintertools/theme/Entry/
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/Rectangle.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/RoundedRectangle.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/RoundedRectangle.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/RoundedRectangle.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/RoundedRectangle.out.light.json
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/SingleLineText.dark.json
+-rw-rw-rw-   0        0        0      158 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Entry/SingleLineText.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.744877 tkintertools-3.0.0b2/tkintertools/theme/HighlightButton/
+-rw-rw-rw-   0        0        0      155 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/HighlightButton/Information.dark.json
+-rw-rw-rw-   0        0        0      155 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/HighlightButton/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.747500 tkintertools-3.0.0b2/tkintertools/theme/Information/
+-rw-rw-rw-   0        0        0       55 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Information/Information.dark.json
+-rw-rw-rw-   0        0        0       55 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Information/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.755353 tkintertools-3.0.0b2/tkintertools/theme/Label/
+-rw-rw-rw-   0        0        0      106 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/Information.dark.json
+-rw-rw-rw-   0        0        0      106 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/Information.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/Rectangle.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/Rectangle.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/RoundedRectangle.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Label/RoundedRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.767535 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/Rectangle.out.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/SemicircularRectangle.in.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/SemicircularRectangle.in.light.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/SemicircularRectangle.out.dark.json
+-rw-rw-rw-   0        0        0      168 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/ProgressBar/SemicircularRectangle.out.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.778323 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Oval.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Oval.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Oval.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Oval.out.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      251 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/RadioButton/Rectangle.out.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.789252 tkintertools-3.0.0b2/tkintertools/theme/Switch/
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Oval.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Oval.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.in.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.in.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.out.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.out.light.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/SemicircularRectangle.dark.json
+-rw-rw-rw-   0        0        0      520 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/Switch/SemicircularRectangle.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.792382 tkintertools-3.0.0b2/tkintertools/theme/UnderlineButton/
+-rw-rw-rw-   0        0        0      159 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/UnderlineButton/Information.dark.json
+-rw-rw-rw-   0        0        0      154 2024-05-23 12:19:00.000000 tkintertools-3.0.0b2/tkintertools/theme/UnderlineButton/Information.light.json
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.796582 tkintertools-3.0.0b2/tkintertools/three/
+-rw-rw-rw-   0        0        0       74 2024-06-02 18:18:04.000000 tkintertools-3.0.0b2/tkintertools/three/__init__.py
+-rw-rw-rw-   0        0        0    28197 2024-06-02 18:18:06.000000 tkintertools-3.0.0b2/tkintertools/three/engine.py
+-rw-rw-rw-   0        0        0     4711 2024-06-02 18:18:07.000000 tkintertools-3.0.0b2/tkintertools/three/geometries.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.800702 tkintertools-3.0.0b2/tkintertools/toolbox/
+-rw-rw-rw-   0        0        0       77 2024-06-02 18:18:12.000000 tkintertools-3.0.0b2/tkintertools/toolbox/__init__.py
+-rw-rw-rw-   0        0        0     1367 2024-06-02 18:18:13.000000 tkintertools-3.0.0b2/tkintertools/toolbox/enhanced.py
+-rw-rw-rw-   0        0        0     2532 2024-06-02 18:18:14.000000 tkintertools-3.0.0b2/tkintertools/toolbox/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-02 18:30:18.802731 tkintertools-3.0.0b2/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0     9996 2024-06-02 18:30:18.000000 tkintertools-3.0.0b2/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4080 2024-06-02 18:30:18.000000 tkintertools-3.0.0b2/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 18:30:18.000000 tkintertools-3.0.0b2/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-06-02 18:30:18.000000 tkintertools-3.0.0b2/tkintertools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 18:30:18.000000 tkintertools-3.0.0b2/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-3.0.0b1/LICENSE.txt` & `tkintertools-3.0.0b2/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 小康2022
+Copyright (c) 2024 Xiaokang2022
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tkintertools-3.0.0b1/PKG-INFO` & `tkintertools-3.0.0b2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: tkintertools is a UI framework based on the Canvas class of tkinter
 Author-email: Xiaokang2022 <2951256653@qq.com>
 Maintainer-email: Xiaokang2022 <2951256653@qq.com>
 License: MIT License
         
-        Copyright (c) 2024 小康2022
+        Copyright (c) 2024 Xiaokang2022
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -36,35 +36,41 @@
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: darkdetect
 Requires-Dist: darkdetect[macos-listener]
 
+> [!IMPORTANT]  
+> Due to the growing nature of the project, the original name `tkintertools` is no longer in line with its original intended, so the project is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put them in the discussion forum.  
+> 由于本项目的不断壮大，原名称 `tkintertools` 已不符合其本意，故本项目准备在进入 `3.0.0.rc1` 版本时更名为 “tkinter advanced canvas UI framework”（`tacUI`）。如有其它想法或建议，可在讨论区中提出。
+
 <h1 align="center">tkintertools</h1>
 
 <p align="center"><img alt="logo" src="https://xiaokang2022.github.io/tkintertools/logo.png" title="Logo" /></p>
 
 <p align="center">
 <code>tkintertools</code> 是一个基于 <code>tkinter</code> 的 <code>Canvas</code> 类的 UI 框架
 <br/>
 <code>tkintertools</code> is a UI framework based on the <code>Canvas</code> class of <code>tkinter</code>
 </p>
 
 <p align="center">
-<a href="."><img alt="Version" src="https://img.shields.io/pypi/v/tkintertools?label=Version" title="Version" /></a>
-<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/pypi/l/tkintertools?label=License" title="License" /></a>
-<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads" title="Downloads" /></a>
+<a href="https://github.com/Xiaokang2022/tkintertools/releases"><img alt="Version" src="https://img.shields.io/github/v/release/Xiaokang2022/tkintertools?include_prereleases&logo=github&label=Version" title="Latest Version" /></a>
+<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/github/license/Xiaokang2022/tkintertools?logo=github&label=License" title="License" /></a>
+<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi&logoColor=skyblue" title="Downloads" /></a>
 <a href="https://pepy.tech/project/tkintertools"><img alt="Total Downloads" src="https://static.pepy.tech/badge/tkintertools" title="Total Downloads" /></a>
-<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size" title="Code Size"/></a>
+<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size&logo=github" title="Code Size"/></a>
 <br/>
 <a href="https://github.com/Xiaokang2022/tkintertools/watchers"><img alt="Watchers" src="https://img.shields.io/github/watchers/Xiaokang2022/tkintertools?label=Watchers&logo=github&style=flat" title="Watchers" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/forks"><img alt="Forks" src="https://img.shields.io/github/forks/Xiaokang2022/tkintertools?label=Forks&logo=github&style=flat" title="Forks" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/Xiaokang2022/tkintertools?label=Stars&color=gold&logo=github&style=flat" title="Stars" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/issues"><img alt="Issues" src="https://img.shields.io/github/issues/Xiaokang2022/tkintertools?label=Issues&logo=github" title="Issues" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/pulls"><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/Xiaokang2022/tkintertools?label=Pull%20Requests&logo=github" title="Pull Requests" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/Xiaokang2022/tkintertools?label=Discussions&logo=github" title="Discussions" /></a>
@@ -80,59 +86,84 @@
             <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date&theme=dark" />
             <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
             <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
         </picture>
     </a>
 </p>
 
-Install - 模块安装
------------------
+📦 Installation - 安装
+-----------------------
 
-### Stable Version - 稳定版本
+### ✅ Stable Version - 稳定版本
 
 * 🔖 Version - 最新版本 : `2.6.21`
 * 🕓 Release - 发布日期 : 2024-01-01
 * ✨ Feature - 更新内容 : [News-2.6.21](https://xiaokang2022.github.io/tkintertools/news/2.6.21/News/)
 
 ```sh
 pip install tkintertools
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
 
 [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
 
 [![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/#%E4%B8%89%E9%80%9A%E8%BF%87-after-%E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB)
 
 </details>
 
-### Development Version - 开发版本
+### 🔥 Development Version - 开发版本
 
-* 🔖 Version - 最新版本 : `3.0.0.beta1`
-* 🕓 Release - 发布日期 : 2024-05-17
-* ✨ Feature - 更新内容 : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
+* 🔖 Version - 最新版本 : `3.0.0.beta2`
+* 🕓 Release - 发布日期 : 2024-06-03
+* ✨ Feature - 更新内容 : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
 
 ```sh
-
+pip install tkintertools==3.0.0b2
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
+
+* **Windows 11 Dark Theme**
+
+![Light - Win11](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png)
+
+* **Windows 10 Light Theme**
+
+![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-win10.png)
+
+* **Ubuntu 24.04 (GNOME) Dark Theme**
 
-[![Light Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+![Light - Ubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png)
 
-[![Dark Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+* **Kubuntu 24.04 (KDE) Light Theme**
+
+![Light - Kubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png)
+
+* **macOS Dark Theme**
+
+![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-mac.png)
 
 </details>
 
-> [!IMPORTANT]  
+> [!WARNING]  
 > `tkt 2.*` has been discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*` can be difficult.  
 > `tkt 2.*` 已放弃支持，如需获取新的功能，请使用 `tkt 3.*`。同时请注意，`tkt 3.*` 与 `tkt 2.*` 几乎完全不兼容，将项目从 `tkt 2.*` 移植到 `tkt 3.*` 可能会十分困难。
 
-More - 更多
------------
+📦 Dependency packages - 依赖包
+-------------------------------
+
+### 1️⃣ darkdetect
+
+* 🔖 Version - 版本 : `0.8.0`
+* 📑 License - 许可 : BSD 3-Clause
+* 🔗 GitHub - 仓库 : [darkdetect](https://github.com/albertosottile/darkdetect)
+
+👀 More - 更多
+---------------
 
 * 📋 Todo - 待办事项: [TODO.md](TODO.md)
 * 📑 License - 项目许可: [LICENSE.txt](LICENSE.txt)
 * 📘 Changelog - 更新日志: [CHANGELOG.md](CHANGELOG.md)
 * 📕 Security Policy - 安全策略: [SECURITY.md](SECURITY.md)
 * 📗 Contribution Guide - 贡献指南: [CONTRIBUTING.md](CONTRIBUTING.md)
 * 📙 Code of Conduct - 行为准则: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 3.0.0b1 Summary: tkintertools
+Metadata-Version: 2.1 Name: tkintertools Version: 3.0.0b2 Summary: tkintertools
 is a UI framework based on the Canvas class of tkinter Author-email:
 Xiaokang2022 <2951256653@qq.com> Maintainer-email: Xiaokang2022
-<2951256653@qq.com> License: MIT License Copyright (c) 2024 å°åº·2022
+<2951256653@qq.com> License: MIT License Copyright (c) 2024 Xiaokang2022
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
@@ -22,55 +22,72 @@
 platform,themed Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: MacOS Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Widget Sets Classifier:
-Typing :: Typed Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.txt Requires-Dist: darkdetect[macos-listener]
+Typing :: Typed Classifier: Development Status :: 4 - Beta Requires-Python:
+>=3.10 Description-Content-Type: text/markdown License-File: LICENSE.txt
+Requires-Dist: darkdetect Requires-Dist: darkdetect[macos-listener] >
+[!IMPORTANT] > Due to the growing nature of the project, the original name
+`tkintertools` is no longer in line with its original intended, so the project
+is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in
+version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put
+them in the discussion forum. > ç±äºæ¬é¡¹ç®çä¸æ­å£®å¤§ï¼ååç§°
+`tkintertools` å·²ä¸ç¬¦åå¶æ¬æï¼ææ¬é¡¹ç®åå¤å¨è¿å¥ `3.0.0.rc1`
+çæ¬æ¶æ´åä¸º âtkinter advanced canvas UI
+frameworkâï¼`tacUI`ï¼ãå¦æå¶å®æ³æ³æå»ºè®®ï¼å¯å¨è®¨è®ºåºä¸­æåºã
                           ************ ttkkiinntteerrttoooollss ************
                                     [logo]
        tkintertools æ¯ä¸ä¸ªåºäº tkinter ç Canvas ç±»ç UI æ¡æ¶
       tkintertools is a UI framework based on the Canvas class of tkinter
              _[_V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_T_o_t_a_l_ _D_o_w_n_l_o_a_d_s_]_[_S_i_z_e_]
          _[_W_a_t_c_h_e_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_P_u_l_l_ _R_e_q_u_e_s_t_s_]_[_D_i_s_c_u_s_s_i_o_n_s_]
                                   _[_I_n_s_i_g_h_t_s_]
                              _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
-Install - æ¨¡åå®è£ ----------------- ### Stable Version - ç¨³å®çæ¬ *
-ð Version - ææ°çæ¬ : `2.6.21` * ð Release - åå¸æ¥æ : 2024-01-
-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://xiaokang2022.github.io/
-tkintertools/news/2.6.21/News/) ```sh pip install tkintertools ``` Preview -
-é¢è§ [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/
-images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-
-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
-[![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/
-7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
+ð¦ Installation - å®è£ ----------------------- ### â Stable Version -
+ç¨³å®çæ¬ * ð Version - ææ°çæ¬ : `2.6.21` * ð Release -
+åå¸æ¥æ : 2024-01-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://
+xiaokang2022.github.io/tkintertools/news/2.6.21/News/) ```sh pip install
+tkintertools ``` ðï¸ Preview - é¢è§ [![Preview UI](https://
+xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://
+xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-
+%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6) [!
+[Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-
+3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
 #%E4%B8%89%E9%80%9A%E8%BF%87-after-
 %E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB) ###
-Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
-`3.0.0.beta1` * ð Release - åå¸æ¥æ : 2024-05-17 * â¨ Feature -
-æ´æ°åå®¹ : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/
-3.0.0/News/) ```sh ``` Preview - é¢è§ [![Light Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) [![Dark Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) > [!IMPORTANT] > `tkt 2.*` has been
-discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*`
-is almost completely incompatible with `tkt 2.*`, and porting a project from
-`tkt 2.*` to `tkt 3.*` can be difficult. > `tkt 2.*`
+ð¥ Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
+`3.0.0.beta2` * ð Release - åå¸æ¥æ : 2024-06-03 * â¨ Feature -
+æ´æ°åå®¹ : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/News/) ```sh pip install tkintertools==3.0.0b2 ``` ðï¸ Preview -
+é¢è§ * **Windows 11 Dark Theme** ![Light - Win11](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png) * **Windows 10
+Light Theme** ![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/light-win10.png) * **Ubuntu 24.04 (GNOME) Dark Theme** ![Light - Ubuntu]
+(https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png) *
+**Kubuntu 24.04 (KDE) Light Theme** ![Light - Kubuntu](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png) * **macOS
+Dark Theme** ![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/dark-mac.png) > [!WARNING] > `tkt 2.*` has been discontinued, for new
+features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely
+incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*`
+can be difficult. > `tkt 2.*`
 å·²æ¾å¼æ¯æï¼å¦éè·åæ°çåè½ï¼è¯·ä½¿ç¨ `tkt
 3.*`ãåæ¶è¯·æ³¨æï¼`tkt 3.*` ä¸ `tkt 2.*`
 å ä¹å®å¨ä¸å¼å®¹ï¼å°é¡¹ç®ä» `tkt 2.*` ç§»æ¤å° `tkt 3.*`
-å¯è½ä¼ååå°é¾ã More - æ´å¤ ----------- * ð Todo - å¾åäºé¡¹:
-[TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯: [LICENSE.txt](LICENSE.txt) *
-ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md](CHANGELOG.md) * ð Security
-Policy - å®å¨ç­ç¥: [SECURITY.md](SECURITY.md) * ð Contribution Guide -
-è´¡ç®æå: [CONTRIBUTING.md](CONTRIBUTING.md) * ð Code of Conduct -
-è¡ä¸ºåå: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) * ð Tutorials and
-Documents - æç¨åææ¡£: [Tutorials & Documents](https://
-xiaokang2022.github.io/tkintertools/) * ð Repository Mirrors -
-å­å¨åºéåæº: [GitHub](https://github.com/Xiaokang2022/tkintertools) |
-[Gitee](https://gitee.com/xiaokang-2022/tkintertools) | [GitCode](https://
-gitcode.com/Xiaokang2022/tkintertools/overview)
+å¯è½ä¼ååå°é¾ã ð¦ Dependency packages - ä¾èµå -----------------
+-------------- ### 1ï¸â£ darkdetect * ð Version - çæ¬ : `0.8.0` * ð
+License - è®¸å¯ : BSD 3-Clause * ð GitHub - ä»åº : [darkdetect](https://
+github.com/albertosottile/darkdetect) ð More - æ´å¤ --------------- * ð
+Todo - å¾åäºé¡¹: [TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯:
+[LICENSE.txt](LICENSE.txt) * ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md]
+(CHANGELOG.md) * ð Security Policy - å®å¨ç­ç¥: [SECURITY.md]
+(SECURITY.md) * ð Contribution Guide - è´¡ç®æå: [CONTRIBUTING.md]
+(CONTRIBUTING.md) * ð Code of Conduct - è¡ä¸ºåå: [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md) * ð Tutorials and Documents - æç¨åææ¡£:
+[Tutorials & Documents](https://xiaokang2022.github.io/tkintertools/) * ð
+Repository Mirrors - å­å¨åºéåæº: [GitHub](https://github.com/
+Xiaokang2022/tkintertools) | [Gitee](https://gitee.com/xiaokang-2022/
+tkintertools) | [GitCode](https://gitcode.com/Xiaokang2022/tkintertools/
+overview)
```

### Comparing `tkintertools-3.0.0b1/README.md` & `tkintertools-3.0.0b2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+> [!IMPORTANT]  
+> Due to the growing nature of the project, the original name `tkintertools` is no longer in line with its original intended, so the project is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put them in the discussion forum.  
+> 由于本项目的不断壮大，原名称 `tkintertools` 已不符合其本意，故本项目准备在进入 `3.0.0.rc1` 版本时更名为 “tkinter advanced canvas UI framework”（`tacUI`）。如有其它想法或建议，可在讨论区中提出。
+
 <h1 align="center">tkintertools</h1>
 
 <p align="center"><img alt="logo" src="https://xiaokang2022.github.io/tkintertools/logo.png" title="Logo" /></p>
 
 <p align="center">
 <code>tkintertools</code> 是一个基于 <code>tkinter</code> 的 <code>Canvas</code> 类的 UI 框架
 <br/>
 <code>tkintertools</code> is a UI framework based on the <code>Canvas</code> class of <code>tkinter</code>
 </p>
 
 <p align="center">
-<a href="."><img alt="Version" src="https://img.shields.io/pypi/v/tkintertools?label=Version" title="Version" /></a>
-<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/pypi/l/tkintertools?label=License" title="License" /></a>
-<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads" title="Downloads" /></a>
+<a href="https://github.com/Xiaokang2022/tkintertools/releases"><img alt="Version" src="https://img.shields.io/github/v/release/Xiaokang2022/tkintertools?include_prereleases&logo=github&label=Version" title="Latest Version" /></a>
+<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/github/license/Xiaokang2022/tkintertools?logo=github&label=License" title="License" /></a>
+<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi&logoColor=skyblue" title="Downloads" /></a>
 <a href="https://pepy.tech/project/tkintertools"><img alt="Total Downloads" src="https://static.pepy.tech/badge/tkintertools" title="Total Downloads" /></a>
-<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size" title="Code Size"/></a>
+<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size&logo=github" title="Code Size"/></a>
 <br/>
 <a href="https://github.com/Xiaokang2022/tkintertools/watchers"><img alt="Watchers" src="https://img.shields.io/github/watchers/Xiaokang2022/tkintertools?label=Watchers&logo=github&style=flat" title="Watchers" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/forks"><img alt="Forks" src="https://img.shields.io/github/forks/Xiaokang2022/tkintertools?label=Forks&logo=github&style=flat" title="Forks" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/Xiaokang2022/tkintertools?label=Stars&color=gold&logo=github&style=flat" title="Stars" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/issues"><img alt="Issues" src="https://img.shields.io/github/issues/Xiaokang2022/tkintertools?label=Issues&logo=github" title="Issues" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/pulls"><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/Xiaokang2022/tkintertools?label=Pull%20Requests&logo=github" title="Pull Requests" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/Xiaokang2022/tkintertools?label=Discussions&logo=github" title="Discussions" /></a>
@@ -33,59 +37,84 @@
             <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date&theme=dark" />
             <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
             <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
         </picture>
     </a>
 </p>
 
-Install - 模块安装
------------------
+📦 Installation - 安装
+-----------------------
 
-### Stable Version - 稳定版本
+### ✅ Stable Version - 稳定版本
 
 * 🔖 Version - 最新版本 : `2.6.21`
 * 🕓 Release - 发布日期 : 2024-01-01
 * ✨ Feature - 更新内容 : [News-2.6.21](https://xiaokang2022.github.io/tkintertools/news/2.6.21/News/)
 
 ```sh
 pip install tkintertools
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
 
 [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
 
 [![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/#%E4%B8%89%E9%80%9A%E8%BF%87-after-%E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB)
 
 </details>
 
-### Development Version - 开发版本
+### 🔥 Development Version - 开发版本
 
-* 🔖 Version - 最新版本 : `3.0.0.beta1`
-* 🕓 Release - 发布日期 : 2024-05-17
-* ✨ Feature - 更新内容 : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
+* 🔖 Version - 最新版本 : `3.0.0.beta2`
+* 🕓 Release - 发布日期 : 2024-06-03
+* ✨ Feature - 更新内容 : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
 
 ```sh
-
+pip install tkintertools==3.0.0b2
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
+
+* **Windows 11 Dark Theme**
+
+![Light - Win11](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png)
+
+* **Windows 10 Light Theme**
+
+![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-win10.png)
+
+* **Ubuntu 24.04 (GNOME) Dark Theme**
 
-[![Light Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+![Light - Ubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png)
 
-[![Dark Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+* **Kubuntu 24.04 (KDE) Light Theme**
+
+![Light - Kubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png)
+
+* **macOS Dark Theme**
+
+![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-mac.png)
 
 </details>
 
-> [!IMPORTANT]  
+> [!WARNING]  
 > `tkt 2.*` has been discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*` can be difficult.  
 > `tkt 2.*` 已放弃支持，如需获取新的功能，请使用 `tkt 3.*`。同时请注意，`tkt 3.*` 与 `tkt 2.*` 几乎完全不兼容，将项目从 `tkt 2.*` 移植到 `tkt 3.*` 可能会十分困难。
 
-More - 更多
------------
+📦 Dependency packages - 依赖包
+-------------------------------
+
+### 1️⃣ darkdetect
+
+* 🔖 Version - 版本 : `0.8.0`
+* 📑 License - 许可 : BSD 3-Clause
+* 🔗 GitHub - 仓库 : [darkdetect](https://github.com/albertosottile/darkdetect)
+
+👀 More - 更多
+---------------
 
 * 📋 Todo - 待办事项: [TODO.md](TODO.md)
 * 📑 License - 项目许可: [LICENSE.txt](LICENSE.txt)
 * 📘 Changelog - 更新日志: [CHANGELOG.md](CHANGELOG.md)
 * 📕 Security Policy - 安全策略: [SECURITY.md](SECURITY.md)
 * 📗 Contribution Guide - 贡献指南: [CONTRIBUTING.md](CONTRIBUTING.md)
 * 📙 Code of Conduct - 行为准则: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
```

#### html2text {}

```diff
@@ -1,46 +1,62 @@
+> [!IMPORTANT] > Due to the growing nature of the project, the original name
+`tkintertools` is no longer in line with its original intended, so the project
+is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in
+version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put
+them in the discussion forum. > ç±äºæ¬é¡¹ç®çä¸æ­å£®å¤§ï¼ååç§°
+`tkintertools` å·²ä¸ç¬¦åå¶æ¬æï¼ææ¬é¡¹ç®åå¤å¨è¿å¥ `3.0.0.rc1`
+çæ¬æ¶æ´åä¸º âtkinter advanced canvas UI
+frameworkâï¼`tacUI`ï¼ãå¦æå¶å®æ³æ³æå»ºè®®ï¼å¯å¨è®¨è®ºåºä¸­æåºã
                           ************ ttkkiinntteerrttoooollss ************
                                     [logo]
        tkintertools æ¯ä¸ä¸ªåºäº tkinter ç Canvas ç±»ç UI æ¡æ¶
       tkintertools is a UI framework based on the Canvas class of tkinter
              _[_V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_T_o_t_a_l_ _D_o_w_n_l_o_a_d_s_]_[_S_i_z_e_]
          _[_W_a_t_c_h_e_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_P_u_l_l_ _R_e_q_u_e_s_t_s_]_[_D_i_s_c_u_s_s_i_o_n_s_]
                                   _[_I_n_s_i_g_h_t_s_]
                              _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
-Install - æ¨¡åå®è£ ----------------- ### Stable Version - ç¨³å®çæ¬ *
-ð Version - ææ°çæ¬ : `2.6.21` * ð Release - åå¸æ¥æ : 2024-01-
-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://xiaokang2022.github.io/
-tkintertools/news/2.6.21/News/) ```sh pip install tkintertools ``` Preview -
-é¢è§ [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/
-images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-
-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
-[![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/
-7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
+ð¦ Installation - å®è£ ----------------------- ### â Stable Version -
+ç¨³å®çæ¬ * ð Version - ææ°çæ¬ : `2.6.21` * ð Release -
+åå¸æ¥æ : 2024-01-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://
+xiaokang2022.github.io/tkintertools/news/2.6.21/News/) ```sh pip install
+tkintertools ``` ðï¸ Preview - é¢è§ [![Preview UI](https://
+xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://
+xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-
+%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6) [!
+[Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-
+3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
 #%E4%B8%89%E9%80%9A%E8%BF%87-after-
 %E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB) ###
-Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
-`3.0.0.beta1` * ð Release - åå¸æ¥æ : 2024-05-17 * â¨ Feature -
-æ´æ°åå®¹ : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/
-3.0.0/News/) ```sh ``` Preview - é¢è§ [![Light Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) [![Dark Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) > [!IMPORTANT] > `tkt 2.*` has been
-discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*`
-is almost completely incompatible with `tkt 2.*`, and porting a project from
-`tkt 2.*` to `tkt 3.*` can be difficult. > `tkt 2.*`
+ð¥ Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
+`3.0.0.beta2` * ð Release - åå¸æ¥æ : 2024-06-03 * â¨ Feature -
+æ´æ°åå®¹ : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/News/) ```sh pip install tkintertools==3.0.0b2 ``` ðï¸ Preview -
+é¢è§ * **Windows 11 Dark Theme** ![Light - Win11](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png) * **Windows 10
+Light Theme** ![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/light-win10.png) * **Ubuntu 24.04 (GNOME) Dark Theme** ![Light - Ubuntu]
+(https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png) *
+**Kubuntu 24.04 (KDE) Light Theme** ![Light - Kubuntu](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png) * **macOS
+Dark Theme** ![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/dark-mac.png) > [!WARNING] > `tkt 2.*` has been discontinued, for new
+features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely
+incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*`
+can be difficult. > `tkt 2.*`
 å·²æ¾å¼æ¯æï¼å¦éè·åæ°çåè½ï¼è¯·ä½¿ç¨ `tkt
 3.*`ãåæ¶è¯·æ³¨æï¼`tkt 3.*` ä¸ `tkt 2.*`
 å ä¹å®å¨ä¸å¼å®¹ï¼å°é¡¹ç®ä» `tkt 2.*` ç§»æ¤å° `tkt 3.*`
-å¯è½ä¼ååå°é¾ã More - æ´å¤ ----------- * ð Todo - å¾åäºé¡¹:
-[TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯: [LICENSE.txt](LICENSE.txt) *
-ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md](CHANGELOG.md) * ð Security
-Policy - å®å¨ç­ç¥: [SECURITY.md](SECURITY.md) * ð Contribution Guide -
-è´¡ç®æå: [CONTRIBUTING.md](CONTRIBUTING.md) * ð Code of Conduct -
-è¡ä¸ºåå: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) * ð Tutorials and
-Documents - æç¨åææ¡£: [Tutorials & Documents](https://
-xiaokang2022.github.io/tkintertools/) * ð Repository Mirrors -
-å­å¨åºéåæº: [GitHub](https://github.com/Xiaokang2022/tkintertools) |
-[Gitee](https://gitee.com/xiaokang-2022/tkintertools) | [GitCode](https://
-gitcode.com/Xiaokang2022/tkintertools/overview)
+å¯è½ä¼ååå°é¾ã ð¦ Dependency packages - ä¾èµå -----------------
+-------------- ### 1ï¸â£ darkdetect * ð Version - çæ¬ : `0.8.0` * ð
+License - è®¸å¯ : BSD 3-Clause * ð GitHub - ä»åº : [darkdetect](https://
+github.com/albertosottile/darkdetect) ð More - æ´å¤ --------------- * ð
+Todo - å¾åäºé¡¹: [TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯:
+[LICENSE.txt](LICENSE.txt) * ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md]
+(CHANGELOG.md) * ð Security Policy - å®å¨ç­ç¥: [SECURITY.md]
+(SECURITY.md) * ð Contribution Guide - è´¡ç®æå: [CONTRIBUTING.md]
+(CONTRIBUTING.md) * ð Code of Conduct - è¡ä¸ºåå: [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md) * ð Tutorials and Documents - æç¨åææ¡£:
+[Tutorials & Documents](https://xiaokang2022.github.io/tkintertools/) * ð
+Repository Mirrors - å­å¨åºéåæº: [GitHub](https://github.com/
+Xiaokang2022/tkintertools) | [Gitee](https://gitee.com/xiaokang-2022/
+tkintertools) | [GitCode](https://gitcode.com/Xiaokang2022/tkintertools/
+overview)
```

### Comparing `tkintertools-3.0.0b1/pyproject.toml` & `tkintertools-3.0.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
     "tkintertools",
     "gui",
     "ui",
     "3d",
     "cross-platform",
     "themed",
 ]
-dependencies = ["darkdetect[macos-listener]"]
+dependencies = ["darkdetect", "darkdetect[macos-listener]"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Natural Language :: Chinese (Simplified)",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Widget Sets",
     "Typing :: Typed",
+    "Development Status :: 4 - Beta",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/Xiaokang2022/tkintertools"
 Homepage = "https://xiaokang2022.github.io/tkintertools/"
 "Bug Reports" = "https://github.com/Xiaokang2022/tkintertools/issues"
```

### Comparing `tkintertools-3.0.0b1/tkintertools/__init__.py` & `tkintertools-3.0.0b2/tkintertools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 if sys.version_info < (3, 10):
     raise ImportError(
         "tkintertools requires a Python version of 3.10 or greater.")
 
 if platform.system() == "Windows":  # Set Windows DPI awareness
     ctypes.windll.shcore.SetProcessDpiAwareness(1)
 
-from .constants import *
 from .core import *
 from .standard import *
+from .toolbox.enhanced import *
 
-__version__ = "3.0.0.beta1"
+__version__ = "3.0.0.beta2"
 __author__ = "Xiaokang2022 <2951256653@qq.com>"
```

### Comparing `tkintertools-3.0.0b1/tkintertools/animation/animations.py` & `tkintertools-3.0.0b2/tkintertools/animation/animations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 """Standard animations"""
 
 import numbers
 import tkinter
 import typing
 
-from .. import core
 from ..color import rgb
+from ..core import virtual
 from . import controllers
 
+__all__ = [
+    "Animation",
+    "MoveWidget",
+    "MoveComponent",
+    "MoveItem",
+    "Gradient",
+    "ScaleFontSize",
+]
+
 
 class Animation:
     """Base Class for Animation"""
 
     def __init__(
         self,
         ms: int,
@@ -89,15 +98,15 @@
 
 
 class MoveWidget(Animation):
     """Animation of moving a widget"""
 
     def __init__(
         self,
-        widget: "core.Widget",
+        widget: "virtual.Widget",
         ms: int,
         delta: tuple[float, float],
         *,
         controller: typing.Callable[[float], float] = controllers.flat,
         end: typing.Callable[[], typing.Any] | None = None,
         repeat: int = 0,
         fps: int = 30,
@@ -120,15 +129,15 @@
 
 
 class MoveComponent(Animation):
     """Animation of moving a component"""
 
     def __init__(
         self,
-        component: "core.Component",
+        component: "virtual.Component",
         ms: int,
         delta: tuple[float, float],
         *,
         controller: typing.Callable[[float], float] = controllers.flat,
         end: typing.Callable[[], typing.Any] | None = None,
         repeat: int = 0,
         fps: int = 30,
@@ -151,15 +160,15 @@
 
 
 class MoveItem(Animation):
     """Animation of moving a item"""
 
     def __init__(
         self,
-        canvas: "core.Canvas",
+        canvas: "virtual.Canvas",
         item: int,
         ms: int,
         delta: tuple[float, float],
         *,
         controller: typing.Callable[[float], float] = controllers.flat,
         end: typing.Callable[[], typing.Any] | None = None,
         repeat: int = 0,
@@ -184,15 +193,15 @@
 
 
 class Gradient(Animation):
     """Animation for color gradients"""
 
     def __init__(
         self,
-        canvas: "core.Canvas",
+        canvas: "virtual.Canvas",
         item: int,
         option: str,
         ms: int,
         delta: tuple[str, str],
         *,
         controller: typing.Callable[[float], float] = controllers.flat,
         end: typing.Callable[[], typing.Any] | None = None,
@@ -224,15 +233,15 @@
 
 
 class ScaleFontSize(Animation):
     """Animation for scaling the font size"""
 
     def __init__(
         self,
-        text: "core.Text",
+        text: "virtual.Text",
         ms: int,
         delta: float | tuple[float, float],
         *,
         controller: typing.Callable[[float], float] = controllers.flat,
         end: typing.Callable[[], typing.Any] | None = None,
         repeat: int = 0,
         fps: int = 30,
```

### Comparing `tkintertools-3.0.0b1/tkintertools/animation/controllers.py` & `tkintertools-3.0.0b2/tkintertools/animation/controllers.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 * `rebound`: before the end, displacement will bounce off a bit
 """
 
 import functools
 import math
 import typing
 
+__all__ = [
+    "controller_generator",
+    "flat",
+    "smooth",
+    "rebound",
+]
+
 
 def _map_t(
     start: float,
     end: float
 ) -> typing.Callable[[float], float]:
     """
     Map parameters in any range between 0 and 1
```

### Comparing `tkintertools-3.0.0b1/tkintertools/color/colormap.py` & `tkintertools-3.0.0b2/tkintertools/color/colormap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """Color mapping table"""
 
 import tkinter
 
+__all__ = [
+    "COLOR_MAP",
+    "name_to_rgb",
+]
+
 COLOR_MAP: dict[str, tuple[int, int, int]] = {
     'alice blue': (240, 248, 255),
     'aliceblue': (240, 248, 255),
     'antique white': (250, 235, 215),
     'antiquewhite': (250, 235, 215),
     'antiquewhite1': (255, 239, 219),
     'antiquewhite2': (238, 223, 204),
```

### Comparing `tkintertools-3.0.0b1/tkintertools/color/rgb.py` & `tkintertools-3.0.0b2/tkintertools/color/rgb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,64 @@
-"""Support for RGB codes"""
+"""Support for RGB"""
 
 import statistics
 import typing
 
 from ..animation import controllers
 from . import colormap
 
+__all__ = [
+    "contrast",
+    "convert",
+    "blend",
+    "gradient",
+    "str_to_rgb",
+    "rgb_to_str",
+]
+
 RGB = tuple[int, int, int]
+"""
+R: Red, 0 ~ 255
+G: Green, 0 ~ 255
+B: Blue, 0 ~ 255
+"""
+
+MAX = 255, 255, 255
 
 
 def contrast(
     rgb: RGB,
     /,
-    channel: tuple[bool, bool, bool] = (True, True, True),
+    channels: tuple[bool, bool, bool] = (True, True, True),
 ) -> RGB:
     """
     Get a contrasting color of a color
 
     * `rgb`: a tuple, RGB codes
-    * `channel`: three color channels
+    * `channels`: three color channels
     """
-    return tuple(map(lambda x: x[1] * (256-x[0]), zip(rgb, channel)))
+    return tuple(map(lambda x: x[0] * (x[1]-x[2]), zip(channels, MAX, rgb)))
 
 
 def convert(
     first: RGB,
     second: RGB,
     rate: float,
     *,
-    channel: tuple[bool, bool, bool] = (True, True, True),
+    channels: tuple[bool, bool, bool] = (True, True, True),
 ) -> RGB:
     """
     Convert one color to another proportionally
 
     * `first`: first color
     * `second`: second color
     * `rate`: conversion rate
-    * `channel`: three color channels
+    * `channels`: three color channels
     """
-    return tuple(first[i] + round((second[i]-first[i])*rate*v) for i, v in enumerate(channel))
+    return tuple(first[i] + round((second[i]-first[i])*rate*v) for i, v in enumerate(channels))
 
 
 def blend(
     colors: list[RGB],
     *,
     weights: list[tuple] | None = None
 ) -> RGB:
@@ -82,20 +98,20 @@
     rgb_list: list[RGB] = []
     delta = tuple(rate * (j-i) * k for i, j, k in zip(first, second, channels))
     for x in (contoller(i/count) for i in range(count)):
         rgb_list.append(tuple(c + round(x*r) for c, r in zip(first, delta)))
     return rgb_list
 
 
-def _str_to_rgba(__c: str, *, refer: str) -> RGB:
+def _str_to_rgba(__c: str, *, reference: str) -> RGB:
     """Experimental: Convert color strings(RGBA) to RGB codes"""
     hex, a = divmod(int(__c[1:], 16), 256)
     hex, b = divmod(hex, 256)
     r, g = divmod(hex, 256)
-    refer_rgb = str_to_rgb(refer)
+    refer_rgb = str_to_rgb(reference)
     return convert((r, g, b), refer_rgb, 1 - a/255)
 
 
 def str_to_rgb(__c: str, /) -> RGB:
     """Convert color strings to RGB codes"""
     if __c.startswith("#"):  # HEX
         hex, b = divmod(int(__c[1:], 16), 256)
```

### Comparing `tkintertools-3.0.0b1/tkintertools/standard/dialogs.py` & `tkintertools-3.0.0b2/tkintertools/standard/dialogs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """All standard Dialogs"""
 
 import tkinter
 import tkinter.colorchooser as colorchooser
 import typing
 
-__all__ = ["Message", "ColorChooser", "FontChooser"]
+__all__ = [
+    "TkMessage",
+    "TkColorChooser",
+    "TkFontChooser",
+]
 
 
-class Message:
+class TkMessage:
     """Message pop-up"""
 
     def __init__(
         self,
         message: str | None = None,
         detail: str | None = None,
         *,
@@ -53,15 +57,15 @@
         if default is not None:
             args += ["-default", default]
         value = master.call("tk_messageBox", "-parent", master, *args)
         if command is not None:
             command(value)
 
 
-class ColorChooser:
+class TkColorChooser:
     """Color chooser pop-up"""
 
     def __init__(
         self,
         *,
         title: str | None = None,
         color: str | None = None,
@@ -76,15 +80,15 @@
         """
         color: tuple[tuple[int, int, int] | None, str | None] = colorchooser.askcolor(
             parent=master, title=title, initialcolor=color)
         if command is not None and color[0] is not None:
             command(color[1])
 
 
-class FontChooser:
+class TkFontChooser:
     """Font chooser pop-up"""
 
     def __init__(
         self,
         *,
         title: str | None = None,
         font: str | None = None,
```

### Comparing `tkintertools-3.0.0b1/tkintertools/standard/features.py` & `tkintertools-3.0.0b2/tkintertools/standard/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 """All standard Features"""
 
 import tkinter
 import typing
 
-from .. import core
 from ..animation import animations
+from ..core import virtual
 
+__all__ = [
+    "Label",
+    "Button",
+    "Underline",
+    "Highlight",
+    "Switch",
+    "CheckButton",
+    "RadioButton",
+    "ProgressBar",
+    "Entry",
+]
 
-class Label(core.Feature):
+
+class Label(virtual.Feature):
     """"""
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.shapes[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="arrow")
+            self.widget.master._trigger_config.update(cursor="arrow")
             if self.widget.state != "hover":
                 self.widget.update("hover")
         else:
             if self.widget.state != "normal":
                 self.widget.update("normal")
         return flag
 
 
-class Button(core.Feature):
+class Button(virtual.Feature):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         *,
         command: typing.Callable | None = None,
         args: tuple = (),
     ) -> None:
         """"""
-        core.Feature.__init__(self, widget)
+        virtual.Feature.__init__(self, widget)
         self._command: typing.Callable = command
         self._args: tuple = args
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.shapes[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="hand2")
+            self.widget.master._trigger_config.update(cursor="hand2")
             if self.widget.state == "normal":
                 self.widget.update("hover")
         else:
             if self.widget.state != "normal":
                 self.widget.update("normal")
         return flag
 
@@ -66,20 +78,20 @@
             if self.widget.state == "active":
                 self.widget.update("hover")
                 if self._command is not None:
                     self._command(*self._args)
         return flag
 
 
-class UnderLine(Button):
+class Underline(Button):
     """"""
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.texts[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="hand2")
+            self.widget.master._trigger_config.update(cursor="hand2")
             if self.widget.state == "normal":
                 self.widget.update("hover")
                 self.widget.texts[0].font.config(underline=True)
         else:
             if self.widget.state != "normal":
                 self.widget.update("normal")
                 self.widget.texts[0].font.config(underline=False)
@@ -102,15 +114,15 @@
 
 
 class Highlight(Button):
     """"""
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.texts[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="hand2")
+            self.widget.master._trigger_config.update(cursor="hand2")
             if self.widget.state == "normal":
                 self.widget.update("hover")
                 animations.ScaleFontSize(
                     self.widget.texts[0], 150, delta=28).start()
         else:
             if self.widget.state != "normal":
                 self.widget.update("normal")
@@ -138,15 +150,15 @@
 
 
 class Switch(Button):
     """"""
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.shapes[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="hand2")
+            self.widget.master._trigger_config.update(cursor="hand2")
             if self.widget.state.startswith("normal"):
                 self.widget.update(
                     f"hover-{'on' if self.widget.get() else 'off'}")
         else:
             if not self.widget.state.startswith("normal"):
                 self.widget.update(
                     f"normal-{'on' if self.widget.get() else 'off'}")
@@ -199,27 +211,27 @@
 
 
 class Entry(Button):
     """"""
 
     def _move_none(self, event: tkinter.Event) -> bool:
         if flag := self.widget.shapes[0].detect(event.x, event.y):
-            self.widget.master.trigger_config.update(cursor="xterm")
+            self.widget.master._trigger_config.update(cursor="xterm")
             if self.widget.state == "normal":
                 self.widget.update("hover")
         else:
             if self.widget.state == "hover":
                 self.widget.update("normal")
         return flag
 
     def _click_left(self, event: tkinter.Event) -> bool:
         if flag := self.widget.shapes[0].detect(event.x, event.y):
             self.widget.update("active")
             if self.widget.state == "active":  # Maybe widget is disabled
-                self.widget.master.trigger_focus.update(
+                self.widget.master._trigger_focus.update(
                     True, self.widget.texts[0].items[0])
                 self.widget.texts[0].cursor_set(
                     self.widget.texts[0]._text_length())
         else:
             if self.widget.state != "normal":
                 self.widget.update("normal")
         return flag
```

### Comparing `tkintertools-3.0.0b1/tkintertools/standard/shapes.py` & `tkintertools-3.0.0b2/tkintertools/standard/shapes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,125 @@
 """All standard Shapes"""
 
 import math
 import warnings
 
-from .. import core
+from ..core import virtual
 
+__all__ = [
+    "Line",
+    "Rectangle",
+    "Oval",
+    "RegularPolygon",
+    "RoundedRectangle",
+    "SemicircularRectangle",
+    "SharpRectangle",
+    "Parallelogram",
+]
 
-class Line(core.Shape):
+
+class Line(virtual.Shape):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         rel_position: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         width: int = 0,
         points: list[tuple[float, float]] = [],
         animation: bool = True,
         styles: dict[str | int, dict[str | int, dict[str, str]]] | None = None
     ) -> None:
         self.points = points
         self.width = width
-        core.Shape.__init__(self, widget, rel_position, size,
-                            name=name, styles=styles, animation=animation)
+        virtual.Shape.__init__(self, widget, rel_position, size,
+                               name=name, styles=styles, animation=animation)
 
+    # @typing.override
     def display(self) -> None:
         points = [(x+self.x, y+self.y) for x, y in self.points]
         self.items = [self.widget.master.create_line(
             *points, tags=("fill", "fill"), width=self.width)]
 
 
-class Rectangle(core.Shape):
+class Rectangle(virtual.Shape):
     """"""
 
+    # @typing.override
     def display(self) -> None:
         self.items = [self.widget.master.create_rectangle(
             *self.region(), tags=("fill", "fill", "outline", "outline"))]
 
 
-class Oval(core.Shape):
+class Oval(virtual.Shape):
     """"""
 
+    # @typing.override
     def display(self) -> None:
         self.items = [self.widget.master.create_oval(
             *self.region(), tags=("fill", "fill", "outline", "outline"))]
 
 
-class RegularPolygon(core.Shape):
+class RegularPolygon(virtual.Shape):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         rel_position: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         animation: bool = True,
         styles: dict[str, dict[str, str]] | None = None,
         side: int = 3,
         angle: float = 0,
     ) -> None:
         self.side = side
         self.angle = angle
-        core.Shape.__init__(self, widget, rel_position, size,
-                            name=name, styles=styles, animation=animation)
+        virtual.Shape.__init__(self, widget, rel_position, size,
+                               name=name, styles=styles, animation=animation)
 
+    # @typing.override
     def display(self) -> None:
         r = min(self.w, self.h) / 2
         if self.side < 3:
             warnings.warn("Parameters are not suitable")
         points = []
         for i in range(self.side):
             angle = math.tau*i/self.side+self.angle
             points.append(math.cos(angle)*r + self.x + self.w/2)
             points.append(math.sin(angle)*r + self.y + self.h/2)
 
         self.items = [self.widget.master.create_polygon(
             *points, tags=("fill", "fill", "outline", "outline"))]
 
 
-class RoundedRectangle(core.Shape):
+class RoundedRectangle(virtual.Shape):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         rel_position: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         animation: bool = True,
         styles: dict[str, dict[str, str]] | None = None,
         radius: int = 5,
     ) -> None:
         self.radius = radius
-        core.Shape.__init__(self, widget, rel_position, size,
-                            name=name, styles=styles, animation=animation)
+        virtual.Shape.__init__(self, widget, rel_position, size,
+                               name=name, styles=styles, animation=animation)
 
+    # @typing.override
     def display(self) -> None:
         """"""
         x, y, w, h = self.x, self.y, self.w, self.h
         x1, y1, x2, y2 = x, y, x + w, y + h
         r, d = self.radius, self.radius*2
 
         if d > w or d > h:
@@ -143,17 +159,18 @@
             self.widget.master.create_arc(
                 x1, y2-d, x1+d, y2, style="arc", start=180, tags=("outline", "outline")),
             self.widget.master.create_arc(
                 x2-d, y2-d, x2, y2, style="arc", start=-90, tags=("outline", "outline")),
         ]
 
 
-class SemicircularRectangle(core.Shape):
+class SemicircularRectangle(virtual.Shape):
     """"""
 
+    # @typing.override
     def display(self) -> None:
         """"""
         x, y, w, h = self.x, self.y, self.w, self.h
         x1, y1, x2, y2 = x, y, x + w, y + h
         d = h
         r = d/2
 
@@ -176,20 +193,20 @@
             self.widget.master.create_line(
                 x1+r, y1, x2-r+1, y1, tags=("fill", "outline")),
             self.widget.master.create_line(
                 x1+r, y2, x2-r+1, y2, tags=("fill", "outline")),
         ]
 
 
-class SharpRectangle(core.Shape):
+class SharpRectangle(virtual.Shape):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         rel_position: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         animation: bool = True,
         styles: dict[str, dict[str, str]] | None = None,
         theta: float = math.pi/6,
@@ -197,17 +214,18 @@
     ) -> None:
         self.theta = theta
         self.ratio = ratio
         if not 0 <= theta <= math.pi/3:
             warnings.warn("Parameters are not suitable")
         if math.isclose(abs(self.ratio[0] - self.ratio[1]), 1):
             warnings.warn("Parameters are not suitable")
-        core.Shape.__init__(self, widget, rel_position, size,
-                            name=name, styles=styles, animation=animation)
+        virtual.Shape.__init__(self, widget, rel_position, size,
+                               name=name, styles=styles, animation=animation)
 
+    # @typing.override
     def display(self) -> None:
         """"""
         x, y, w, h = self.x, self.y, self.w, self.h
 
         if w < h:
             warnings.warn("Parameters are not suitable")
 
@@ -228,34 +246,35 @@
             x1+dx[0], y2
         ]
 
         self.items = [self.widget.master.create_polygon(
             *points, tags=("fill", "fill", "outline", "outline"))]
 
 
-class Parallelogram(core.Shape):
+class Parallelogram(virtual.Shape):
     """"""
 
     def __init__(
         self,
-        widget: core.Widget,
+        widget: virtual.Widget,
         rel_position: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         animation: bool = True,
         styles: dict[str, dict[str, str]] | None = None,
         theta: float = math.pi/6,
     ) -> None:
         self.theta = theta
         if not abs(theta) <= math.pi/3:
             warnings.warn("Parameters are not suitable")
-        core.Shape.__init__(self, widget, rel_position, size,
-                            name=name, styles=styles, animation=animation)
+        virtual.Shape.__init__(self, widget, rel_position, size,
+                               name=name, styles=styles, animation=animation)
 
+    # @typing.override
     def display(self) -> None:
         """"""
         x, y, w, h = self.x, self.y, self.w, self.h
 
         if (dx := h*math.tan(self.theta)) >= w:
             warnings.warn("Parameters are not suitable")
```

### Comparing `tkintertools-3.0.0b1/tkintertools/standard/texts.py` & `tkintertools-3.0.0b2/tkintertools/standard/texts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """All standard Texts"""
 
 import typing
 
-from .. import core
+from ..core import virtual
 
+__all__ = [
+    "Information",
+    "SingleLineText",
+]
 
-class Information(core.Text):
+
+class Information(virtual.Text):
     """"""
 
+    # @typing.override
     def display(self) -> None:
         self.items.append(self.widget.master.create_text(
             *self.center(), text=self.value, font=self.font, tags=("fill", "fill")))
 
     def get(self) -> str:
         """Get the value of `Text`"""
         return self.value
@@ -39,17 +45,18 @@
 
     def clear(self) -> None:
         """Clear the value of `Text`"""
         self.value = ""
         self.widget.master.itemconfigure(self.items[0], text=self.value)
 
 
-class SingleLineText(core.Text):
+class SingleLineText(virtual.Text):
     """"""
 
+    # @typing.override
     def display(self) -> None:
         self.items.append(self.widget.master.create_text(
             *self.center(), text=self.value, font=self.font, tags=("fill", "fill")))
 
     def _text_get(self) -> str:
         """"""
         return self.widget.master.itemcget(self.items[0], "text")
```

### Comparing `tkintertools-3.0.0b1/tkintertools/standard/widgets.py` & `tkintertools-3.0.0b2/tkintertools/core/virtual.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,375 +1,426 @@
-"""All standard Widgets"""
+"""
+Various virtual classes
 
-import math
-import typing
+The virtual `Widget` consists of 4 parts, which are `Shape`, `Text`, `Image`, and `Feature`
 
-from .. import constants, core
-from ..animation import animations, controllers
-from . import features, images, shapes, texts
+where `Feature` is the function of widgets, and each widget can be bound to up to one,
+but in terms of appearance, there is no limit to the number of `Shape`, `Text`, and `Image`
 
+`Shape`, `Text`, and `Image` are all appearance components that inherit from abstract base class `Components`
+"""
 
-class Information(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (0, 0),
-        *,
-        name: str | None = None,
-        animation: bool = True,
-        text: str = "",
-        family: str | None = None,
-        fontsize: int | None = None,
-        weight: typing.Literal['normal', 'bold'] = "normal",
-        slant: typing.Literal['roman', 'italic'] = "roman",
-        underline: bool = False,
-        overstrike: bool = False,
-    ) -> None:
-        """"""
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        texts.Information(self, text=text, family=family, size=fontsize, weight=weight,
-                          slant=slant, underline=underline, overstrike=overstrike)
+import abc
+import copy
+import math
+import tkinter
+import tkinter.font as font
+import typing
 
+from ..animation import animations
+from ..color import rgb
+from ..style import parser
+from ..toolbox import enhanced
+from . import constants, containers
+
+__all__ = [
+    "Feature",
+    "Component",
+    "Shape",
+    "Text",
+    "Image",
+    "Widget",
+]
+
+
+class Feature(abc.ABC):
+    """The features of a `Widget`"""
+
+    def __init__(self, widget: "Widget") -> None:
+        self.widget: Widget = widget
+        widget.feature = self
+
+    def _move_none(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of moving the mouse"""
+        return False
+
+    def _move_left(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of holding down the left mouse button to move the mouse"""
+        return False
+
+    def _move_center(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of holding down the center mouse button to move the mouse"""
+        return False
+
+    def _move_right(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of holding down the right mouse button to move the mouse"""
+        return False
+
+    def _click_left(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of pressing the left mouse button"""
+        return False
+
+    def _click_center(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of pressing the center mouse button"""
+        return False
+
+    def _click_right(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of pressing the right mouse button"""
+        return False
+
+    def _release_left(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of releasing the left mouse button"""
+        return False
+
+    def _release_center(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of releasing the center mouse button"""
+        return False
+
+    def _release_right(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of releasing the right mouse button"""
+        return False
+
+    def _wheel(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of scrolling the mouse wheel"""
+        return False
+
+    def _input(self, event: tkinter.Event) -> bool:
+        """Internal Method: Event of typing"""
+        return False
 
-class Label(core.Widget):
-    """
-    Label widget
 
-    Used to display information
-    """
+class Component(abc.ABC):
+    """The basic part of a `Widget`"""
 
     def __init__(
         self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (120, 50),
+        widget: "Widget",
+        rel_position: tuple[int, int] = (0, 0),
+        size: tuple[int, int] | None = None,
         *,
         name: str | None = None,
         animation: bool = True,
-        text: str = "",
-        family: str | None = None,
-        fontsize: int | None = None,
-        weight: typing.Literal['normal', 'bold'] = "normal",
-        slant: typing.Literal['roman', 'italic'] = "roman",
-        underline: bool = False,
-        overstrike: bool = False,
+        styles: dict[str, dict[str, str]] | None = None,
     ) -> None:
-        """"""
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self)
-        else:
-            shapes.RoundedRectangle(self)
-        texts.Information(self, text=text, family=family, size=fontsize, weight=weight,
-                          slant=slant, underline=underline, overstrike=overstrike)
-        features.Label(self)
+        self.widget: Widget = widget
+        self.x = rel_position[0] + widget.x
+        self.y = rel_position[1] + widget.y
+        self.w, self.h = size if size else (widget.w, widget.h)
+        self.name: str | None = name
+        self.styles = styles if styles else parser.get(widget, self)
+        self.items: list[int] = []
+        self.visible: bool = True
+        self.animation = animation
+        widget.register(self)
+
+    def move(self, dx: float, dy: float) -> None:
+        """Move the `Component`"""
+        self.x += dx
+        self.y += dy
+        for item in self.items:
+            self.widget.master.move(item, dx, dy)
+
+    def moveto(self, x: float, y: float) -> None:
+        """Move the `Component` to a certain position"""
+        return self.move(x - self.x, y - self.y)
+
+    def destroy(self) -> None:
+        """Destroy the `Component`"""
+        self.widget.master.delete(*self.items)
+
+    def center(self) -> tuple[int, int]:
+        """Return the geometric center of the `Component`"""
+        return self.x + self.w/2, self.y + self.h/2
+
+    def region(self) -> tuple[int, int, int, int]:
+        """Return the decision region of the `Component`"""
+        return self.x, self.y, self.x + self.w, self.y + self.h
+
+    def detect(self, x: int, y: int) -> bool:
+        """Detect whether the specified coordinates are within the `Component`"""
+        x1, y1, x2, y2 = self.region()
+        return x1 <= x <= x2 and y1 <= y <= y2
+
+    def update(self, state: str | None = None, *, no_delay: bool = False) -> None:
+        """
+        Update the style of the `Component` to the corresponding state
+
+        * `state`: the state of the `Component`
+        """
+        if state is None:
+            state = self.widget.state
+        if not self.visible:
+            return
+        if self.styles.get(state) is not None:
+            self.configure(self.styles[state], no_delay=no_delay)
+
+    def _get_disabled_style(self, refer_state: str = "normal") -> dict[str, str]:
+        """"""
+        if self.styles.get("disabled") is None:
+            self.styles["disabled"] = copy.deepcopy(
+                self.styles.get(refer_state, {}))
+            for key, value in self.styles["disabled"].items():
+                self.styles["disabled"][key] = rgb.rgb_to_str(rgb.convert(
+                    rgb.str_to_rgb(value), rgb.str_to_rgb(self.widget.master["bg"]), 0.618))
+        return self.styles["disabled"]
+
+    def configure(self, style: dict[str, str], *, no_delay: bool = False) -> None:
+        """Configure properties of the `Component` and update them immediately"""
+        for item in self.items:
+            tags = self.widget.master.itemcget(item, "tags").split()
+            kwargs = {key: value for key, param in zip(
+                tags[0:-1:2], tags[1:len(tags):2]) if (value := style.get(param)) is not None}
+            if self.widget.animation and self.animation and not no_delay:
+                for key, value in kwargs.items():
+                    start_color: str = self.widget.master.itemcget(item, key)
+                    if start_color.startswith("#") and len(start_color) == 9:
+                        start_color = rgb.rgb_to_str(rgb._str_to_rgba(
+                            start_color, reference=self.widget.master["bg"]))
+                    if value.startswith("#") and len(value) == 9:
+                        value = rgb.rgb_to_str(rgb._str_to_rgba(
+                            value, reference=self.widget.master["bg"]))
+                    if value == "" or start_color == "":  # Null characters cannot be parsed
+                        self.widget.master.itemconfigure(item, **{key: value})
+                    else:
+                        animations.Gradient(
+                            self.widget.master, item, key, 150, (start_color, value)).start()
+            else:
+                for key, value in kwargs.items():
+                    if value.startswith("#") and len(value) == 9:
+                        kwargs[key] = rgb.rgb_to_str(rgb._str_to_rgba(
+                            value, reference=self.widget.master["bg"]))
+                self.widget.master.itemconfigure(item, **kwargs)
+
+    def appear(self, *, no_delay: bool = True) -> None:
+        """"""
+        self.visible = True
+        self.update(self.widget.state, no_delay=no_delay)
+
+    def disappear(self, *, no_delay: bool = True) -> None:
+        """"""
+        self.visible = False
+        temp_style = copy.deepcopy(self.styles.get(self.widget.state))
+        if temp_style is None:
+            return
+        for arg in temp_style:
+            temp_style[arg] = ""
+        self.configure(temp_style, no_delay=no_delay)
+
+    def __getitem__(self, key: str) -> dict[str, str]:
+        """"""
+        return self.styles[key]
+
+    def __setitem__(self, key: str, value: dict[str, str]) -> None:
+        """"""
+        self.styles[key].update(value)
+        self.update(no_delay=True)
+
+    @abc.abstractmethod
+    def zoom(self, ratio: tuple[float, float]) -> None:
+        """Scale the `Component`"""
+
+    @abc.abstractmethod
+    def display(self) -> None:
+        """Display the `Component` on a `Canvas`"""
+
+
+class Shape(Component):
+    """Base Class: The Shape of a `Widget`"""
+
+    # @typing.override
+    def zoom(self, ratio: tuple[float, float]) -> None:
+        """Scale the items"""
+        for item in self.items:
+            self.widget.master.scale(item, 0, 0, *ratio)
 
 
-class Button(core.Widget):
-    """
-    Button Widget
-    """
+class Text(Component):
+    """Base Class: The text of a `Widget`"""
 
     def __init__(
         self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (120, 50),
+        widget: "Widget",
+        rel_position: tuple[int, int] = (0, 0),
         *,
-        name: str | None = None,
+        styles: dict[str, dict[str, str]] | None = None,
         animation: bool = True,
         text: str = "",
         family: str | None = None,
-        fontsize: int | None = None,
-        weight: typing.Literal['normal', 'bold'] = "normal",
-        slant: typing.Literal['roman', 'italic'] = "roman",
+        size: int | None = None,
+        weight: typing.Literal["normal", "bold"] = "normal",
+        slant: typing.Literal["roman", "italic"] = "roman",
         underline: bool = False,
         overstrike: bool = False,
-        command: typing.Callable | None = None,
+        limit: int = math.inf,
     ) -> None:
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self)
-        else:
-            shapes.RoundedRectangle(self)
-        texts.Information(self, text=text, family=family, size=fontsize, weight=weight,
-                          slant=slant, underline=underline, overstrike=overstrike)
-        features.Button(self, command=command)
+        """
+        * `text`: the value of `Text`
+        * `limit`: the limitation of value length
+        """
+        self.value: str = text
+        self.limit: int = limit
+        self.left: int = 0
+        self.right: int = 0
+        self.font: font.Font = font.Font(
+            family=family if family else constants.FONT,
+            size=-abs(size if size else constants.SIZE),
+            weight=weight, slant=slant,
+            underline=underline, overstrike=overstrike)
+        Component.__init__(self, widget, rel_position,
+                           styles=styles, animation=animation)
+
+    def region(self) -> tuple[int, int, int, int]:
+        """Return the decision region of the `Text`"""
+        width_half = self.font.measure(self.value)/2
+        height_half = -self.font.cget("size") / 2
+        x, y = self.center()
+        return x-width_half, y-height_half, x+width_half, y+height_half
+
+    # @typing.override
+    def zoom(self, ratio: tuple[float, float]) -> None:
+        """Scale the text"""
+        for item in self.items:
+            value = self.widget.master._texts[item]
+            value[0] *= math.sqrt(ratio[0]*ratio[1])
+            value[1].config(size=round(value[0]))
+            self.widget.master.itemconfigure(item, font=value[1])
+            self.widget.master.scale(item, 0, 0, *ratio)
 
 
-class Switch(core.Widget):
-    """"""
+class Image(Component):
+    """Base Class: an image of a `Widget`"""
 
     def __init__(
         self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        length: int = 60,
+        widget: "Widget",
+        rel_position: tuple[int, int] = (0, 0),
+        size: tuple[int, int] | None = None,
         *,
+        image: enhanced.PhotoImage | None = None,
         name: str | None = None,
         animation: bool = True,
-        default: bool = False,
-        command: typing.Callable[[bool], typing.Any] | None = None,
+        styles: dict[str, dict[str, str]] | None = None,
     ) -> None:
-        core.Widget.__init__(self, master, position, (length, length / 2),
-                             state=f"normal-{'on' if default else 'off'}",
-                             name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self, name=".out")
-            shapes.Rectangle(self, name=".in", rel_position=(
-                length/12, length/12), size=(length/3, length/3), animation=False)
-        else:
-            shapes.SemicircularRectangle(self)
-            shapes.Oval(self, rel_position=(length/12, length/12),
-                        size=(length/3, length/3), animation=False)
-        features.Switch(self, command=command)
-        if default:
-            self.set(default)
-
-    def get(self) -> bool:
         """"""
-        return self.state.endswith("on")
+        self.image = image
+        Component.__init__(self, widget, rel_position, size,
+                           name=name, animation=animation, styles=styles)
 
-    def set(self, value: bool) -> None:
+    # @typing.override
+    def zoom(self, ratio: tuple[float, float]) -> None:
         """"""
-        self.update(
-            f"{self.state.split('-')[0]}-{'on' if value else 'off'}", no_delay=True)
-        dx = self.shapes[0].w/2 if value else -self.shapes[0].w/2
-        animations.MoveComponent(
-            self.shapes[1], 250, (dx, 0), controller=controllers.smooth, fps=60).start()
-
+        for item in self.items:
+            self.widget.master.scale(item, 0, 0, *ratio)
 
-class Entry(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (250, 50),
-        *,
-        name: str | None = None,
-        animation: bool = True,
-        limit: int = math.inf
-    ) -> None:
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self)
-        else:
-            shapes.RoundedRectangle(self, name=".out")
-            shapes.RoundedRectangle(self, name=".in", size=(self.w, self.h-3))
-        texts.SingleLineText(self, text="", limit=limit)
-        features.Entry(self)
-
-    def get(self) -> str:
-        """"""
-        return self.texts[0].get()
-
-    def set(self, value: str) -> None:
-        """"""
-        self.texts[0].set(value)
-
-    def append(self, value: str) -> None:
-        """"""
-        self.texts[0].append(value)
-
-    def delete(self, count: int) -> None:
-        """"""
-        self.texts[0].pop(count)
-
-    def clear(self) -> None:
-        """"""
-        self.set("")
 
+class Widget:
+    """
+    Base Widget Class
 
-class CheckButton(core.Widget):
-    """"""
+    `Widget` = `Shape` + `Text` + `Image` + `Feature`
+    """
 
     def __init__(
         self,
-        master: core.Canvas,
+        master: "containers.Canvas",
         position: tuple[int, int],
-        length: int = 30,
+        size: tuple[int, int],
         *,
         name: str | None = None,
+        state: str = "normal",
+        through: bool = False,
         animation: bool = True,
-        default: bool = False,
-        command: typing.Callable[[bool], typing.Any] | None = None,
     ) -> None:
-        core.Widget.__init__(self, master, position,
-                             (length, length), name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self)
+        """"""
+        self.master = master
+        self.x, self.y = position
+        self.w, self.h = size
+        self.through = through
+        self.animation = animation
+        self.name = name
+
+        self.texts: list[Text] = []
+        self.shapes: list[Shape] = []
+        self.images: list[Image] = []
+
+        self.feature: Feature = None
+
+        self.state: str = state
+        self._before_disabled: str = ""
+
+        master._widgets.append(self)
+
+    def register(self, component: Component) -> None:
+        """"""
+        if isinstance(component, Shape):
+            self.shapes.append(component)
+        elif isinstance(component, Text):
+            self.texts.append(component)
+        elif isinstance(component, Image):
+            self.images.append(component)
+        component.display()
+        component.update(no_delay=True)
+
+    def zoom(self, ratio: tuple[float, float] | None = None) -> None:
+        """Zoom self"""
+        if ratio is None:
+            ratio = self.master.ratios
+        self.w *= ratio[0]
+        self.h *= ratio[1]
+        self.x *= ratio[0]
+        self.y *= ratio[1]
+        for elem in self.shapes + self.texts + self.images:
+            elem.zoom(ratio)
+
+    def update(self, state: str | None = None, *, no_delay: bool = False) -> None:
+        """Update the widget"""
+        if self._before_disabled:
+            return
+        if state is not None:
+            self.state = state
+        for elem in self.shapes + self.texts:
+            elem.update(state, no_delay=no_delay)
+
+    def move(self, dx: int, dy: int) -> None:
+        """Move the widget"""
+        self.x += dx
+        self.y += dy
+        for elem in self.shapes + self.texts + self.images:
+            elem.move(dx, dy)
+
+    def moveto(self, x: int, y: int) -> None:
+        """Move the Widget to a certain position"""
+        return self.move(x - self.x, y - self.y)
+
+    def disabled(self, flag: bool = True) -> None:
+        """"""
+        if flag:
+            if not self._before_disabled:
+                self._before_disabled = self.state
+            for elem in self.shapes + self.texts:
+                elem._get_disabled_style(self._before_disabled)
+            self._before_disabled, last_state = "", self._before_disabled  # Let theme to change
+            self.update("disabled", no_delay=True)
+            self._before_disabled = last_state
         else:
-            shapes.RoundedRectangle(self)
-        texts.Information(self).set("✔")
-        features.CheckButton(self, command=command)
-        self.set(default)
+            self._before_disabled, last_state = "", self._before_disabled  # Unlock
+            self.update(last_state, no_delay=True)
 
-    def get(self) -> bool:
-        """"""
-        return self.texts[0].visible
+    def destroy(self) -> None:
+        """Destroy the widget"""
+        self.master._widgets.remove(self)
+        for elem in self.shapes + self.texts + self.images:
+            elem.destroy()
 
-    def set(self, value: bool) -> None:
+    def focus_set(self, *args) -> None:
         """"""
-        if value:
-            return self.texts[0].appear()
-        self.texts[0].disappear()
-
-
-class RadioButton(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        length: int = 24,
-        *,
-        name: str | None = None,
-        animation: bool = True,
-        default: bool = False,
-        command: typing.Callable[[int], typing.Any] | None = None,
-    ) -> None:
-        core.Widget.__init__(self, master, position,
-                             (length, length), name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self, name=".out")
-            shapes.Rectangle(self, name=".in", rel_position=(
-                self.w/4, self.h/4), size=(self.w/2, self.h/2)).disappear()
-        else:
-            shapes.Oval(self, name=".out")
-            shapes.Oval(self, name=".in", rel_position=(
-                self.w/4, self.h/4), size=(self.w/2, self.h/2)).disappear()
-        features.RadioButton(self, command=command)
-        if default:
-            self.shapes[1].appear()
+        self.master.focus(*args)
 
-    def get(self) -> bool:
+    def disappear(self) -> None:
         """"""
-        return self.shapes[1].visible
+        for elem in self.shapes + self.texts:
+            elem.disappear()
 
-    def set(self, value: bool) -> None:
+    def appear(self) -> None:
         """"""
-        if value:
-            return self.shapes[1].appear()
-        self.shapes[1].disappear()
-
-
-class ProgressBar(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (400, 20),
-        *,
-        name: str | None = None,
-        animation: bool = True,
-        command: typing.Callable[[], typing.Any] | None = None,
-    ) -> None:
-        self.value: float = 0
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        if constants.SYSTEM == "Windows10":
-            shapes.Rectangle(self, name=".out")
-            shapes.Rectangle(self, name=".in", size=(
-                0, self.h*0.8), rel_position=(self.h*0.1, self.h*0.1))
-        else:
-            shapes.SemicircularRectangle(self, name=".out")
-            shapes.SemicircularRectangle(self, name=".in", size=(
-                self.h*0.7, self.h*0.7), rel_position=(self.h*0.15, self.h*0.15))
-        features.ProgressBar(self)
-        self.shapes[1].disappear()
-        self.command = command
-
-    def get(self) -> float:
-        """"""
-        return self.value
-
-    def set(self, value: float) -> None:
-        """"""
-        self.value = 0 if value < 0 else 1 if value > 1 else value
-        if self.value == 0:
-            return self.shapes[1].disappear()
-        elif not self.shapes[1].visible:
-            self.shapes[1].appear()
-        if isinstance(self.shapes[1], shapes.Rectangle):
-            x, y = self.shapes[1].x, self.shapes[1].y
-            w, h = (self.w - self.h*0.2)*self.value, self.shapes[1].h
-            self.master.coords(self.shapes[1].items[0], x, y, x+w, y+h)
-        else:
-            w, h = self.w - self.h*0.3 - self.shapes[1].h, self.shapes[1].h
-            x, y = self.shapes[1].x + h/2, self.shapes[1].y
-            w *= self.value
-            self.master.coords(self.shapes[1].items[2], x, y, x+w, y+h)
-            self.master.coords(self.shapes[1].items[5], x, y, x+w, y)
-            self.master.coords(self.shapes[1].items[6], x, y+h, x+w, y+h)
-            self.master.coords(
-                self.shapes[1].items[1], x+w-h/2, y, x+w+h/2, y+h)
-            self.master.coords(
-                self.shapes[1].items[4], x+w-h/2, y, x+w+h/2, y+h)
-        if value == 1 and self.command is not None:
-            self.command()
-
-
-class UnderlineButton(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (0, 0),
-        *,
-        text: str = "",
-        family: str | None = None,
-        fontsize: int | None = None,
-        weight: typing.Literal['normal', 'bold'] = "normal",
-        slant: typing.Literal['roman', 'italic'] = "roman",
-        underline: bool = False,
-        overstrike: bool = False,
-        command: typing.Callable | None = None,
-        name: str | None = None,
-        through: bool = False,
-        animation: bool = False,
-    ) -> None:
-        core.Widget.__init__(self, master, position, size,
-                             name=name, through=through, animation=animation)
-        texts.Information(self, text=text, family=family, size=fontsize, weight=weight,
-                          slant=slant, underline=underline, overstrike=overstrike)
-        features.UnderLine(self, command=command)
-
-
-class HighlightButton(core.Widget):
-    """"""
-
-    def __init__(
-        self,
-        master: core.Canvas,
-        position: tuple[int, int],
-        size: tuple[int, int] = (0, 0),
-        *,
-        name: str | None = None,
-        animation: bool = True,
-        text: str = "",
-        family: str | None = None,
-        fontsize: int | None = None,
-        weight: typing.Literal['normal', 'bold'] = "normal",
-        slant: typing.Literal['roman', 'italic'] = "roman",
-        underline: bool = False,
-        overstrike: bool = False,
-        command: typing.Callable | None = None,
-    ) -> None:
-        core.Widget.__init__(self, master, position, size,
-                             name=name, animation=animation)
-        texts.Information(self, text=text, family=family, size=fontsize, weight=weight,
-                          slant=slant, underline=underline, overstrike=overstrike)
-        features.Highlight(self, command=command)
+        for elem in self.shapes + self.texts:
+            elem.appear()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tkintertools-3.0.0b1/tkintertools/style/parser.py` & `tkintertools-3.0.0b2/tkintertools/style/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Parse the style file path and get it"""
 
 import functools
 import inspect
 import json
 import pathlib
 
-from .. import core
+from ..core import virtual
 from . import theme
 
-system_theme_path = pathlib.Path(__file__).parent.parent / "theme"
-default_theme_path = pathlib.Path().cwd() / "theme"
+__all__ = [
+    "get",
+]
 
 
-def _get_name(obj: "str | core.Widget | core.Component") -> str:
+def _get_name(obj: "str | virtual.Widget | virtual.Component") -> str:
     """Get the name of the object"""
     if getattr(obj, "name", None) is not None:
         if obj.name.startswith("."):  # Special rule
             return obj.__class__.__name__ + obj.name
         return obj.name
     elif inspect.isclass(obj):
         return obj.__name__
@@ -54,22 +55,22 @@
     the data is fetched directly from the cache
 
     * `widget`: widget that need to get styles
     * `component`: component that need to get styles
     * `path`: path to the theme folder
     * `dark`: whether it is in dark mode
     """
-    for path in set((system_theme_path, default_theme_path, path)):
+    for path in set((theme.SYSTEM_THEME_PATH, theme.selected_theme_path, path)):
         if file := _get_path(path, widget, component, dark):
             with open(file, "r", encoding="utf-8") as data:
                 return json.load(data)
     return {}
 
 
-def get(widget: "str | core.Widget", component: "str | core.Component", *, path: str | pathlib.Path = system_theme_path) -> "dict[str, dict[str, str]]":
+def get(widget: "str | virtual.Widget", component: "str | virtual.Component", *, path: str | pathlib.Path = theme.selected_theme_path) -> "dict[str, dict[str, str]]":
     """
     Get style data based on parameters
 
     * `widget`: widget that need to get styles
     * `component`: component that need to get styles
     * `path`: path to the theme folder, which is the built-in theme path by default
```

### Comparing `tkintertools-3.0.0b1/tkintertools/style/theme.py` & `tkintertools-3.0.0b2/tkintertools/style/theme.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,65 @@
 """Support for theme"""
 
 import ctypes
+import pathlib
 import platform
 import threading
 import tkinter
 import typing
 
 import darkdetect
 
 from ..color import rgb
 
+__all__ = [
+    "DARK_MODE",
+    "COLOR_MODE",
+    "SYSTEM_THEME_PATH",
+    "selected_theme_path",
+    "set_color_theme",
+    "set_color_mode",
+    "register_event",
+    "remove_event",
+    "custom_window",
+]
+
 DARK_MODE: bool = darkdetect.isDark()
-THEME_MODE: typing.Literal["system", "dark", "light"] = "system"
+COLOR_MODE: typing.Literal["system", "dark", "light"] = "system"
+SYSTEM_THEME_PATH = pathlib.Path(__file__).parent.parent / "theme"
+
+selected_theme_path = SYSTEM_THEME_PATH
 
 _callback_events: dict[typing.Callable[[bool, typing.Any],
                                        typing.Any], tuple[typing.Any, ...]] = {}
 
 
-def use_theme(__theme: typing.Literal["system", "dark", "light"], /) -> None:
+def set_color_theme(theme_path: pathlib.Path | str = SYSTEM_THEME_PATH) -> bool:
+    """
+    Set a special color theme for the entire program
+
+    color theme is a path of theme folder, default value is `system_theme_path`
+    """
+    global selected_theme_path
+    selected_theme_path = pathlib.Path(theme_path)
+    set_color_mode(COLOR_MODE)
+
+
+def set_color_mode(color_mode: typing.Literal["system", "dark", "light"], /) -> None:
     """
-    Set the theme for the entire program
+    Set the color mode for the entire program
 
-    theme can be light, dark, and follow the system, default is follow the system
+    color mode can be light, dark, and follow the system, default is follow the system
     """
-    global DARK_MODE, THEME_MODE
-    THEME_MODE = __theme
-    if __theme == "system":
+    global DARK_MODE, COLOR_MODE
+    COLOR_MODE = color_mode
+    if color_mode == "system":
         DARK_MODE = darkdetect.isDark()
     else:
-        DARK_MODE = __theme == "dark"
+        DARK_MODE = color_mode == "dark"
     _process_event(DARK_MODE)
 
 
 def register_event(
     func: typing.Callable[[bool, typing.Any], typing.Any],
     *args: typing.Any
 ) -> None:
@@ -59,15 +86,15 @@
         except:
             pass
 
 
 def _callback(theme: str) -> None:
     """callback function that is triggered when a system theme is switched.
     Valid only if the theme mode is set to Follow System"""
-    if THEME_MODE != "system":
+    if COLOR_MODE != "system":
         return
     global DARK_MODE
     DARK_MODE = theme == "Dark"
     _process_event(DARK_MODE)
 
 
 def custom_window(
@@ -85,25 +112,27 @@
     * `dark`: dark mode
     * `bordercolor`: window border color
     * `captioncolor`: window caption color
     * `titlecolor`: window title color
 
     WARNING:
 
-    This class is only valid under Windows OS!
+    This function is only works on Windows OS!
     """
     if platform.system() != "Windows":
         return
     tk.update()
     HWND = ctypes.windll.user32.GetParent(tk.winfo_id())
     if dark is None:
         dark = DARK_MODE
     if dark is not None:
-        ctypes.windll.dwmapi.DwmSetWindowAttribute(
-            HWND, 20, ctypes.byref(ctypes.c_int(dark)), 4)
+        if ctypes.windll.dwmapi.DwmSetWindowAttribute(
+                HWND, 20, ctypes.byref(ctypes.c_int(dark)), 4) != 0:
+            ctypes.windll.dwmapi.DwmSetWindowAttribute(
+                HWND, 19, ctypes.byref(ctypes.c_int(dark)), 4)
     for i, value in enumerate((bordercolor, captioncolor, titlecolor)):
         if value is not None:
             ctypes.windll.dwmapi.DwmSetWindowAttribute(
                 HWND, 34 + i, ctypes.byref(ctypes.c_int(rgb._str_to_hex(value, reverse=True))), 4)
 
 
 threading.Thread(target=lambda: darkdetect.listener(
```

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.dark.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Oval.dark.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Oval.light.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Oval.light.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.dark.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.in.dark.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.in.light.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.in.light.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.dark.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.out.dark.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/Rectangle.out.light.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/Rectangle.out.light.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.dark.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/SemicircularRectangle.dark.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/theme/Switch/SemicircularRectangle.light.json` & `tkintertools-3.0.0b2/tkintertools/theme/Switch/SemicircularRectangle.light.json`

 * *Files identical despite different names*

### Comparing `tkintertools-3.0.0b1/tkintertools/three/engine.py` & `tkintertools-3.0.0b2/tkintertools/three/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,169 +1,316 @@
-"""
-core codes of 3D
-
-WARNING:
-
-The contents of this file are ported from tkt 2 and haven't been modified too much,
-there may be some issues!
-"""
+"""Core codes of 3D"""
 
+import abc
 import array
+import dataclasses
 import math
 import platform
 import statistics
 import tkinter
 import typing
 
-from .. import constants, core
+from ..core import constants, containers, virtual
+
+__all__ = [
+    "Canvas",
+    "Space",
+    "translate",
+    "rotate",
+    "scale",
+    "project",
+    "Component",
+    "Point",
+    "Line",
+    "Side",
+    "Text3D",
+    "Geometry",
+]
 
 
-class Canvas3D(core.Canvas):
-    """3D 画布基类"""
+class Canvas(containers.Canvas):
+    """Base class of 3D Canvas"""
 
     def __init__(
         self,
-        master: core.Tk | core.Toplevel | core.NestedToplevel | core.Canvas,
+        master: containers.Tk | containers.Canvas,
         *,
         expand: typing.Literal["", "x", "y", "xy"] = "xy",
         zoom_item: bool = False,
-        keep_ratio: typing.Literal["min", "max", "full"] | None = None,
+        keep_ratio: typing.Literal["min", "max"] | None = None,
         free_anchor: bool = False,
         **kw,
     ) -> None:
-        """"""
-        core.Canvas.__init__(
+        containers.Canvas.__init__(
             self, master, expand=expand, zoom_item=zoom_item,
             keep_ratio=keep_ratio, free_anchor=free_anchor, **kw)
-        self._items_3d: list[Point | Line | Side] = []
-        self._geos: list[Point | Line | Side] = []
+        self._components: list[Component] = []
+        self._geometries: list[Geometry] = []
         self._distance: int = 1000
 
-    def distance(self, value: int | None = None) -> int | None:
-        """"""
-        if value is None:
-            return self._distance
-        self._distance = value
-
-    def items_3d(self) -> tuple["Point | Line | Side", ...]:
-        """返回 `Canvas3D` 类全部的基本 3D 对象"""
-        return tuple(self._items_3d)
-
-    def geos(self) -> tuple["Geometry", ...]:
-        """返回 `Canvas3D` 类全部的几何体对象"""
-        return tuple(self._geos)
+    @property
+    def components(self) -> tuple["Component", ...]:
+        """Return all `Component` of this Canvas"""
+        return tuple(self._components)
+
+    @property
+    def geometries(self) -> tuple["Geometry", ...]:
+        """Return all `Geometry` of this Canvas"""
+        return tuple(self._geometries)
 
     def space_sort(self) -> None:
-        """空间位置排序"""
-        self._items_3d.sort(key=lambda item: item._camera_distance())
-        for item in self._items_3d:
+        """Sort the contextual relationship between the spatial positions of the components"""
+        self._components.sort(key=lambda item: item._camera_distance())
+        for item in self._components:
             self.lower(item.item)
 
 
-class Space(Canvas3D):
-    """三维空间"""
+# class _Widget(virtual.Widget):
+#     """A virtual widget that binds a feature of the 3D canvas to event processing"""
+
+#     def __init__(self, master: containers.Canvas, feature: virtual.Feature) -> None:
+#         """
+#         * `master`: parent canvas
+#         * `feature`: Feature class, not instance
+#         """
+#         virtual.Widget.__init__(self, master, master._position, master._size)
+#         feature(self)
+
+
+# class _SpaceFeature(virtual.Feature):
+#     """Handles events related to 3D canvas rigging"""
+
+#     def __init__(self, widget: virtual.Widget) -> None:
+#         virtual.Feature.__init__(self, widget)
+#         self._cache: tuple[int, int] | None = None
+
+#     def _click_right(self, event: tkinter.Event) -> bool:
+#         self._cache = event.x, event.y
+#         self.widget.master._trigger_config.update(cursor="fleur")
+#         self.widget.master._trigger_config.lock()
+#         return True
+
+#     def _release_right(self, event: tkinter.Event) -> bool:
+#         self._cache = None
+#         self.widget.master._trigger_config.unlock()
+#         return True
+
+#     def _move_right(self, event: tkinter.Event) -> bool:
+#         dx, dy = event.x - self._cache[0], event.y - self._cache[1]
+#         self._cache = event.x, event.y
+
+#         for item in self.widget.master._components + [self.widget.master._origin]:
+#             item.translate(
+#                 0,
+#                 dx*self.widget.master._initial_size[0]/self.widget.master._size[0],
+#                 -dy*self.widget.master._initial_size[1]/self.widget.master._size[1])
+#             item.update()
+#         self.widget.master.space_sort()
+
+
+class Space(Canvas):
+    """A canvas where you can view 3D objects"""
 
     def __init__(
         self,
-        master: core.Tk | core.Toplevel | core.NestedToplevel | core.Canvas,
+        master: containers.Tk | containers.Canvas,
         *,
         expand: typing.Literal["", "x", "y", "xy"] = "xy",
         zoom_item: bool = False,
-        keep_ratio: typing.Literal["min", "max", "full"] | None = None,
+        keep_ratio: typing.Literal["min", "max"] | None = None,
         free_anchor: bool = False,
         **kw,
     ) -> None:
-        """"""
-        Canvas3D.__init__(
+        Canvas.__init__(
             self, master, expand=expand, zoom_item=zoom_item,
             keep_ratio=keep_ratio, free_anchor=free_anchor, **kw)
-        self._bind_event()
 
-    def _zoom_init(self) -> None:
-        Canvas3D._zoom_init(self)
-        self._origin = Point(self, (0, 0, 0), size=1,
-                             width=1, fill="", outline="")
-        self._items_3d.clear()
-
-    def _zoom(self) -> None:
-        """"""
-        Canvas3D._zoom(self)
-        self.update_idletasks()
-        for item in self._items_3d:
-            item.update()
-        self.space_sort()
-
-    def _bind_event(self) -> None:
-        """"""
         self.bind("<B3-Motion>", self._translate, "+")
         self.bind("<Button-3>", lambda event: self._translate(event, True), "+")
         self.bind("<ButtonRelease-3>",
                   lambda event: self._translate(event, False), "+")
-        self.bind("<B1-Motion>", self._rotate, "+")
-        self.bind("<Button-1>", lambda event: self._rotate(event, True), "+")
-        self.bind("<ButtonRelease-1>",
+
+        self.bind("<B2-Motion>", self._rotate, "+")
+        self.bind("<Button-2>", lambda event: self._rotate(event, True), "+")
+        self.bind("<ButtonRelease-2>",
                   lambda event: self._rotate(event, False), "+")
+
         if platform.system() == "Linux":  # 兼容 Linux 系统
             self.bind("<Button-4>", lambda event: self._scale(event, True), "+")
             self.bind("<Button-5>", lambda event: self._scale(event, False), "+")
         else:
             self.bind("<MouseWheel>", self._scale, "+")
 
-    def _translate(self, event: tkinter.Event, flag: bool | None = None, _cache: list[float] = []) -> None:
-        """平移事件"""
-        if flag is True:  # 按下
+    # @typing.override
+    def _initialization(self) -> None:
+        Canvas._initialization(self)
+        # _Widget(self, _SpaceFeature)
+        self._origin = Point(self, (0, 0, 0), fill="", outline="")
+        self._components.clear()
+
+    # @typing.override
+    def _zoom_self(self) -> None:
+        Canvas._zoom_self(self)
+        for item in self._components:
+            item.update()
+        self.space_sort()
+
+    def _translate(
+        self,
+        event: tkinter.Event,
+        press: bool | None = None,
+        _cache: list[float] = []
+    ) -> None:
+        """
+        Triggering of a translation event
+
+        * `event`: Event
+        * `press`: True, False, and None represent press, release, and move events, respectively
+        * `_cache`: cache values that record the coordinates of mouse presses
+        """
+        if press is True:  # Press
             _cache[:] = [event.x, event.y]
             self.configure(cursor="fleur")
+            self._trigger_config.lock()
             return
-        elif flag is False:  # 松开
+
+        elif press is False:  # Release
+            self._trigger_config.unlock()
             self.configure(cursor="arrow")
             return
+
         dx, dy = event.x - _cache[0], event.y - _cache[1]
         _cache[:] = [event.x, event.y]
-        for item in self._items_3d + [self._origin]:
+
+        for item in self._components + [self._origin]:
             item.translate(
                 0, dx*self._initial_size[0]/self._size[0], -dy*self._initial_size[1]/self._size[1])
             item.update()
         self.space_sort()
 
-    def _rotate(self, event, flag=None, _cache=[]):
-        # type: (tkinter.Event, bool | None, list[float]) -> None
-        """旋转事件"""
-        if flag is False:
-            # if self._release(event):  # 兼容原 core.Canvas
-            #     return
+    def _rotate(
+        self,
+        event: tkinter.Event,
+        press: bool | None = None,
+        _cache: list[float] = []
+    ) -> None:
+        """
+        Triggering of a rotation event
+
+        * `event`: Event
+        * `press`: True, False, and None represent press, release, and move events, respectively
+        * `_cache`: cache values that record the coordinates of mouse presses
+        """
+        if press is True:  # Press
+            _cache[:] = [event.x, event.y]
+            self.configure(cursor="fleur")
+            self._trigger_config.lock()
+            return
+
+        elif press is False:  # Release
+            self._trigger_config.unlock()
             self.configure(cursor="arrow")
             return
-        else:
-            if flag is True:
-                _cache[:] = [event.x, event.y]
-            # if self._click(event):
-            #     return
-            if flag is True:
-                self.configure(cursor="fleur")
-                return
+
         dx, dy = event.x - _cache[0], event.y - _cache[1]
         _cache[:] = [event.x, event.y]
-        for item in self._items_3d:
+
+        for item in self._components:
             item.rotate(0, 2*dy/self._size[0]*math.tau, 2*dx/self._size[1]*math.tau,
                         center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
     def _scale(self, event: tkinter.Event, flag: bool | None = None) -> None:
-        """缩放事件"""
+        """Triggering of a scaling event"""
         if flag is not None:
             event.delta = flag
-        k = 1.1 if event.delta > 0 else 0.9
-        for item in self._items_3d:
+        k = 11/10 if event.delta > 0 else 10/11
+
+        for item in self._components:
             item.scale(k, k, k, center=self._origin.coordinates[0])
             item.update()
         self.space_sort()
 
 
+# class Scene(Canvas):
+#     """"""
+
+
+# @dataclasses.dataclass
+# class Quaternion:
+#     """"""
+
+#     w: float = 0
+#     x: float = 0
+#     y: float = 0
+#     z: float = 0
+
+#     def __matmul__(self, other: "Quaternion") -> "Quaternion":
+#         """"""
+#         w = self.w*other.w - self.x*other.x - self.y*other.y - self.z*other.z
+#         x = self.x*other.w + self.w*other.x - self.z*other.y + self.y*other.z
+#         y = self.y*other.w + self.z*other.x + self.w*other.y - self.x*other.z
+#         z = self.z*other.w - self.y*other.x + self.x*other.y + self.w*other.z
+#         return Quaternion(w, x, y, z)
+
+#     def conjugate(self) -> "Quaternion":
+#         """"""
+#         return Quaternion(self.w, -self.x, -self.y, -self.z)
+
+#     @property
+#     def imag(self) -> tuple[float, float, float]:
+#         """"""
+#         return self.x, self.y, self.z
+
+
+# def q_rotate(point: tuple[float, float, float], axis: tuple[float, float, float], theta: float) -> tuple[float, float, float]:
+#     """"""
+#     theta /= 2
+#     p = Quaternion(0, *point)
+#     q = Quaternion(math.cos(theta), *[a*math.sin(theta) for a in axis])
+#     r = q@p@q.conjugate()
+#     return r.imag
+
+
+# def translate(coordinate: list[float], delta: list[float], *, reference: list[float] | None = None) -> None:
+#     """"""
+#     if reference is None:
+#         for i, v in enumerate(delta):
+#             coordinate[i] += v
+#     else:
+#         pass
+
+
+# def rotate(coordinate: list[float], delta: list[float], *, reference: list[float]) -> None:
+#     """"""
+
+
+# def scale(coordinate: list[float], delta: list[float], *, reference: list[float] | None = None) -> None:
+#     """"""
+#     if reference is None:
+#         for i, v in enumerate(delta):
+#             coordinate[i] *= v
+#     else:
+#         for i, v in enumerate(delta):
+#             coordinate[i] += (coordinate[i]-reference[i]) * (v-1)
+
+
+# def reflect() -> None:
+#     """"""
+
+
+# def shear() -> None:
+#     """"""
+
+
+# def project() -> None:
+#     """"""
+
+
 def translate(coordinate: tuple[float, float, float], dx: float = 0, dy: float = 0, dz: float = 0) -> None:
     """将一个三维空间中的点进行平移
 
     * `coordinate`: 点的空间坐标
     * `dx`: x 方向位移长度
     * `dy`: y 方向位移长度
     * `dz`: z 方向位移长度
@@ -192,15 +339,15 @@
     * `dx`: x 方向逆时针旋转弧度，或者绕旋转轴线的旋转弧度
     * `dy`: y 方向逆时针旋转弧度
     * `dz`: z 方向逆时针旋转弧度
     * `center`: 旋转中心的空间坐标
     * `axis`: 旋转轴线的空间坐标
     """
     if axis is not None:  # 参照为线（定轴转动）
-        center = _Object3D(*axis).center()  # 旋转轴中点
+        center = Component(*axis).center()  # 旋转轴中点
         n = list(axis[0])
         for i in range(3):
             n[i] -= axis[1][i]
             coordinate[i] -= center[i]
         n_m = math.hypot(*n)
         for i in range(3):
             n[i] /= n_m
@@ -260,15 +407,57 @@
     relative_dis = distance - coordinate[0]
     if relative_dis <= 1e-16:
         return [math.inf]*2
     k = distance / relative_dis
     return coordinate[1]*k, coordinate[2]*k
 
 
-class _Object3D:
+# class Camera:
+#     """"""
+
+#     def __init__(
+#         self,
+#         position: tuple[float, float, float],
+#         towards: tuple[float, float, float],
+#         *,
+#         zoom: float = 1,
+#         hFOV: float = math.pi/3,
+#     ) -> None:
+#         """"""
+#         self.hFOV = hFOV
+#         self.position = position
+
+#     def project(self, coordinate: tuple[float, float, float]) -> tuple[float, float]:
+#         """"""
+
+#     def zoom(self, value: float) -> None:
+#         """"""
+
+#     def set_pos(self, pos: tuple[float, float, float]) -> None:
+#         """"""
+
+
+# class Light:
+#     """"""
+
+#     def __init__(
+#         self,
+#         color: str,
+#         item: "Component",
+#         *,
+#         strength: float = 1,
+#     ) -> None:
+#         """"""
+
+
+# class Shade:
+#     """"""
+
+
+class Component(abc.ABC):
     """3D 对象基类"""
 
     def __init__(self, *coordinates):
         # type: (tuple[float, float, float]) -> None
         self.coordinates = [array.array("f", lst) for lst in coordinates]
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
@@ -297,15 +486,25 @@
 
         * `dx`: x 方向逆时针旋转弧度，或者绕旋转轴线的旋转弧度
         * `dy`: y 方向逆时针旋转弧度
         * `dz`: z 方向逆时针旋转弧度
         * `center`: 旋转中心，默认为原点
         * `axis`: 旋转轴线，无默认值
         """
-        for coordinate in self.coordinates:
+        for i, coordinate in enumerate(self.coordinates):
+            # if dx != 0:
+            #     coordinate = q_rotate(coordinate, (1, 0, 0), dx)
+            # if dy != 0:
+            #     coordinate = q_rotate(coordinate, (0, 1, 0), dy)
+            # if dz != 0:
+            #     coordinate = q_rotate(coordinate, (0, 0, 1), dz)
+            # coordinate = array.array('f', coordinate)
+            # for j in range(3):
+            #     coordinate[j] += center[j]
+            # self.coordinates[i] = coordinate
             rotate(coordinate, dx, dy, dz, center=center, axis=axis)
 
     def scale(self, kx=1, ky=1, kz=1, *, center=None):
         # type: (float, float, float, ..., tuple[float, float, float] | None) -> None
         """缩放对象本身
 
         * `kx`: x 方向缩放比例
@@ -319,33 +518,36 @@
             scale(coordinate, kx, ky, kz, center=center)
 
     def center(self):  # type: () -> tuple[float, float, float]
         """几何中心"""
         return tuple(statistics.mean(xyz) for xyz in zip(*self.coordinates))
 
     def _project(self, distance, canvas=None):
-        # type: (float, Canvas3D | Space | None) -> list[tuple[float, float]]
+        # type: (float, Canvas | Space | None) -> list[tuple[float, float]]
         """投影对象自身
 
         * `distance`: 对象与观察者的距离
         * `canvas`: 投影到的画布
         """
         lst = [project(point, distance) for point in self.coordinates]
         if canvas is not None:
             lst = [(pos[0] + canvas._initial_size[0]/2, canvas._initial_size[1]/2 - pos[1])
                    for pos in lst]
         return lst
 
+    @abc.abstractmethod
+    def update(self) -> None: ...
+
 
-class Point(_Object3D):
+class Point(Component):
     """点"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas3D | Space
+        canvas,  # type: Canvas | Space
         coords,  # type: tuple[float, float, float]
         *,
         size=1,  # type: float
         width=1,  # type: float
         fill="#000000",  # type: str
         outline="#000000",  # type: str
         markuptext="",  # type: str
@@ -364,16 +566,16 @@
         * `outline`: 点轮廓的颜色
         * `markuptext`: 标记文本
         * `markupdelta`: 标记文本显示位置的偏移量
         * `markupfont`: 标记文本字体
         * `markupfill`: 标记文本颜色
         * `markupjustify`: 标记文本多行对齐方式
         """
-        _Object3D.__init__(self, list(coords))
-        canvas._items_3d.append(self)
+        Component.__init__(self, list(coords))
+        canvas._components.append(self)
         self.canvas = canvas
         self.size = size
         self.width = width
         self.fill = fill
         self.item = canvas.create_oval(-1, -1, -1, -1,
                                        fill=fill, outline=outline, width=width)
         self.text = None
@@ -382,111 +584,111 @@
                                            font=markupfont, fill=markupfill, justify=markupjustify)
             self.delta = markupdelta
         self.update()
 
     def update(self):  # type: () -> None
         """更新对象的显示"""
         x, y = self._project(self.canvas._distance, self.canvas)[0]
-        self.canvas.coords(self.item, (x-self.size) * self.canvas._ratio[0], (y-self.size) *
-                           self.canvas._ratio[1], (x+self.size) * self.canvas._ratio[0], (y+self.size) * self.canvas._ratio[1])
+        self.canvas.coords(self.item, (x-self.size) * self.canvas.ratios[0], (y-self.size) *
+                           self.canvas.ratios[1], (x+self.size) * self.canvas.ratios[0], (y+self.size) * self.canvas.ratios[1])
         if self.text is not None:
             self.canvas.coords(
-                self.text, (x+self.delta[0]) * self.canvas._ratio[0], (y-self.delta[1]) * self.canvas._ratio[1])
+                self.text, (x+self.delta[0]) * self.canvas.ratios[0], (y-self.delta[1]) * self.canvas.ratios[1])
 
     def _camera_distance(self):  # type: () -> float
         """与相机距离"""
         sign = math.copysign(1, self.canvas._distance - self.coordinates[0][0])
         return sign * math.dist([self.canvas._distance, 0, 0], self.coordinates[0])
 
 
-class Line(_Object3D):
+class Line(Component):
     """线"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas3D | Space
+        canvas,  # type: Canvas | Space
         point_start,  # type: tuple[float, float, float]
         point_end,  # type: tuple[float, float, float]
         *,
         width=1,  # type: float
         fill="#000000",  # type: str
     ):  # type: (...) -> None
         """
         * `canvas`: 父画布
         * `point_start`: 起点坐标
         * `point_end`: 终点坐标
         * `width`: 线的宽度
         * `fill`: 线的颜色
         """
-        _Object3D.__init__(self, list(point_start), list(point_end))
-        canvas._items_3d.append(self)
+        Component.__init__(self, list(point_start), list(point_end))
+        canvas._components.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.item = canvas.create_line(-1, -1, -1, -1, width=width, fill=fill)
         self.update()
 
     def update(self):  # type: () -> None
         """更新对象的显示"""
-        self.canvas.coords(self.item, *[coord * self.canvas._ratio[i]
+        self.canvas.coords(self.item, *[coord * self.canvas.ratios[i]
                            for point in self._project(self.canvas._distance, self.canvas) for i, coord in enumerate(point)])
 
     def _camera_distance(self):  # type: () -> float
         """与相机距离"""
         center = self.center()
         sign = math.copysign(1, self.canvas._distance - center[0])
         return sign * math.dist([self.canvas._distance, 0, 0], center)
 
 
-class Side(_Object3D):
+class Side(Component):
     """面"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas3D | Space
+        canvas,  # type: Canvas | Space
         *points,  # type: tuple[float, float, float]
         width=1,  # type: float
         fill="",  # type: str
         outline="#000000",  # type: str
     ):  # type: (...) -> None
         """
         * `canvas`: 父画布
         * `points`: 各点的空间坐标
         * `width`: 面轮廓的宽度
         * `fill`: 面内部的填充颜色
         * `outline`: 面轮廓的颜色
         """
-        _Object3D.__init__(self, *[list(point) for point in points])
-        canvas._items_3d.append(self)
+        Component.__init__(self, *[list(point) for point in points])
+        canvas._components.append(self)
         self.canvas = canvas
         self.width = width
         self.fill = fill
         self.outline = outline
         self.item = canvas.create_polygon(-1, -1, -1, -1,
                                           width=width, fill=fill, outline=outline)
         self.update()
 
     def update(self):  # type: () -> None
         """更新对象的显示"""
         self.canvas.coords(
-            self.item, *[coord * self.canvas._ratio[i] for point in self._project(self.canvas._distance, self.canvas) for i, coord in enumerate(point)])
+            self.item, *[coord * self.canvas.ratios[i] for point in self._project(self.canvas._distance, self.canvas) for i, coord in enumerate(point)])
 
     def _camera_distance(self):  # type: () -> float
         """与相机距离"""
         center = self.center()
         sign = math.copysign(1, self.canvas._distance - center[0])
         return sign * math.dist([self.canvas._distance, 0, 0], center)
 
 
-class Text3D(_Object3D):
+class Text3D(Component):
     """三维文本"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas3D | Space
+        canvas,  # type: Canvas | Space
         coords,  # type: tuple[float, float, float]
         text="",  # type: str
         *,
         # type: tuple[str, int, str]
         font=(constants.FONT, constants.SIZE),
         justify="center",  # type: typing.Literal["center", "left", "right"]
         fill="#000000",  # type: str
@@ -496,53 +698,53 @@
         * `coords`: 点的空间坐标
         * `text`: 显示的文本
         * `size`: 点的大小
         * `font`: 点轮廓的宽度
         * `justify`: 多行文本对齐方式
         * `fill`: 点内部的填充颜色
         """
-        _Object3D.__init__(self, list(coords))
-        canvas._items_3d.append(self)
+        Component.__init__(self, list(coords))
+        canvas._components.append(self)
         self.canvas = canvas
         self.font = font
         self.fill = fill
         self.text = text
         self.item = canvas.create_text(-1, -1,
                                        text=text, fill=fill, justify=justify)
         self.update()
 
     def update(self):  # type: () -> None
         """更新对象的显示"""
         x, y = self._project(self.canvas._distance, self.canvas)[0]
         self.canvas.coords(
-            self.item, x*self.canvas._ratio[0], y*self.canvas._ratio[1])
+            self.item, x*self.canvas.ratios[0], y*self.canvas.ratios[1])
         font = list(self.font)
         font[1] = round(font[1] * self.canvas._distance *
-                        math.sqrt(self.canvas._ratio[0]*self.canvas._ratio[1]) / self._camera_distance())
+                        math.sqrt(self.canvas.ratios[0]*self.canvas.ratios[1]) / self._camera_distance())
         self.canvas.itemconfigure(self.item, font=font)
 
     def _camera_distance(self):  # type: () -> float
         """与相机距离"""
         sign = math.copysign(1, self.canvas._distance - self.coordinates[0][0])
         return sign * math.dist([self.canvas._distance, 0, 0], self.coordinates[0])
 
 
 class Geometry:
     """几何体"""
 
     def __init__(
         self,
-        canvas,  # type: Canvas3D | Space
+        canvas,  # type: Canvas | Space
         *sides,  # type: Side
     ):  # type: (...) -> None
         """
         * `canvas`: 父画布
         * `sides`: 组成几何体的面
         """
-        canvas._geos.append(self)
+        canvas._geometries.append(self)
         self.canvas = canvas
         self.sides = list(sides)
 
     def translate(self, dx=0, dy=0, dz=0):  # type: (float, float, float) -> None
         """平移几何体中的所有 3D 对象
 
         * `dx`: x 方向位移长度
@@ -601,116 +803,7 @@
     def append(self, *sides):  # type: (Side) -> None
         """给几何体添加更多新的面
 
         * `sides`: `Side` 类
         """
         for side in sides:
             self.sides.append(side)
-
-
-class Cuboid(Geometry):
-    """长方体"""
-
-    def __init__(
-        self,
-        canvas,  # type: Canvas3D | Space
-        x,  # type: float
-        y,  # type: float
-        z,  # type: float
-        length,  # type: float
-        width,  # type: float
-        height,  # type: float
-        *,
-        boardwidth=1,  # type: int
-        color_fill_up="",  # type: str
-        color_fill_down="",  # type: str
-        color_fill_left="",  # type: str
-        color_fill_right="",  # type: str
-        color_fill_front="",  # type: str
-        color_fill_back="",  # type: str
-        color_outline_up="#000000",  # type: str
-        color_outline_down="#000000",  # type: str
-        color_outline_left="#000000",  # type: str
-        color_outline_right="#000000",  # type: str
-        color_outline_front="#000000",  # type: str
-        color_outline_back="#000000",  # type: str
-    ):  # type: (...) -> None
-        """
-        * `canvas`: 父画布
-        * `x`: 左上角 x 坐标
-        * `y`: 左上角 y 坐标
-        * `z`: 左上角 z 坐标
-        * `length`: 长度
-        * `width`: 宽度
-        * `height`: 高度
-        * `boardwidth`: 边框线条宽度
-        * `color_fill_up`: 上表面内部颜色
-        * `color_fill_down`: 下表面内部颜色
-        * `color_fill_left`: 左侧面内部颜色
-        * `color_fill_right`: 右侧面内部颜色
-        * `color_fill_front`: 正面内部颜色
-        * `color_fill_back`: 后面内部颜色
-        * `color_outline_up`: 上表面边框颜色
-        * `color_outline_down`: 下表面边框颜色
-        * `color_outline_left`: 左侧面边框颜色
-        * `color_outline_right`: 右侧面边框颜色
-        * `color_outline_front`: 正面边框颜色
-        * `color_outline_back`: 后面边框颜色
-        """
-        canvas._geos.append(self)
-        self.canvas = canvas
-        coords = [[x + l, y + w, z + h]
-                  for l in (0, length) for w in (0, width) for h in (0, height)]
-        self.sides = [
-            Side(canvas, coords[0], coords[1], coords[3], coords[2],
-                 width=boardwidth, fill=color_fill_back, outline=color_outline_back),
-            Side(canvas, coords[0], coords[1], coords[5], coords[4],
-                 width=boardwidth, fill=color_fill_left, outline=color_outline_left),
-            Side(canvas, coords[0], coords[2], coords[6], coords[4],
-                 width=boardwidth, fill=color_fill_down, outline=color_outline_down),
-            Side(canvas, coords[1], coords[3], coords[7], coords[5],
-                 width=boardwidth, fill=color_fill_up, outline=color_outline_up),
-            Side(canvas, coords[2], coords[3], coords[7], coords[6],
-                 width=boardwidth, fill=color_fill_right, outline=color_outline_right),
-            Side(canvas, coords[4], coords[5], coords[7], coords[6],
-                 width=boardwidth, fill=color_fill_front, outline=color_outline_front),
-        ]
-
-
-class Tetrahedron(Geometry):
-    """四面体"""
-
-    def __init__(
-        self,
-        canvas,  # type: Canvas3D | Space
-        point_1,  # type: tuple[float, float, float]
-        point_2,  # type: tuple[float, float, float]
-        point_3,  # type: tuple[float, float, float]
-        point_4,  # type: tuple[float, float, float]
-        *,
-        boardwidth=1,  # type: int
-        color_fill=("", "", "", ""),  # type: tuple[str, str, str, str]
-        color_outline=("#000000", "#000000", "#000000", "#000000")
-        # type: tuple[str, str, str, str]
-    ):  # type: (...) -> None
-        """
-        * `canvas`: 父画布
-        * `point_1`: 第一个顶点
-        * `point_2`: 第二个顶点
-        * `point_3`: 第三个顶点
-        * `point_4`: 第四个顶点
-        * `boardwidth`: 边框线条宽度
-        * `color_fill`: 内部颜色序列
-        * `color_outline`: 边框颜色序列
-        """
-        canvas._geos.append(self)
-        self.canvas = canvas
-        self.sides = [
-            Side(canvas, point_1, point_2, point_3, width=boardwidth,
-                 fill=color_fill[0], outline=color_outline[0]),
-            Side(canvas, point_1, point_2, point_4, width=boardwidth,
-                 fill=color_fill[1], outline=color_outline[0]),
-            Side(canvas, point_1, point_3, point_4, width=boardwidth,
-                 fill=color_fill[2], outline=color_outline[0]),
-            Side(canvas, point_2, point_3, point_4, width=boardwidth,
-                 fill=color_fill[3], outline=color_outline[0]),
-        ]
```

### Comparing `tkintertools-3.0.0b1/tkintertools.egg-info/PKG-INFO` & `tkintertools-3.0.0b2/tkintertools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: tkintertools is a UI framework based on the Canvas class of tkinter
 Author-email: Xiaokang2022 <2951256653@qq.com>
 Maintainer-email: Xiaokang2022 <2951256653@qq.com>
 License: MIT License
         
-        Copyright (c) 2024 小康2022
+        Copyright (c) 2024 Xiaokang2022
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -36,35 +36,41 @@
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Typing :: Typed
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: darkdetect
 Requires-Dist: darkdetect[macos-listener]
 
+> [!IMPORTANT]  
+> Due to the growing nature of the project, the original name `tkintertools` is no longer in line with its original intended, so the project is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put them in the discussion forum.  
+> 由于本项目的不断壮大，原名称 `tkintertools` 已不符合其本意，故本项目准备在进入 `3.0.0.rc1` 版本时更名为 “tkinter advanced canvas UI framework”（`tacUI`）。如有其它想法或建议，可在讨论区中提出。
+
 <h1 align="center">tkintertools</h1>
 
 <p align="center"><img alt="logo" src="https://xiaokang2022.github.io/tkintertools/logo.png" title="Logo" /></p>
 
 <p align="center">
 <code>tkintertools</code> 是一个基于 <code>tkinter</code> 的 <code>Canvas</code> 类的 UI 框架
 <br/>
 <code>tkintertools</code> is a UI framework based on the <code>Canvas</code> class of <code>tkinter</code>
 </p>
 
 <p align="center">
-<a href="."><img alt="Version" src="https://img.shields.io/pypi/v/tkintertools?label=Version" title="Version" /></a>
-<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/pypi/l/tkintertools?label=License" title="License" /></a>
-<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads" title="Downloads" /></a>
+<a href="https://github.com/Xiaokang2022/tkintertools/releases"><img alt="Version" src="https://img.shields.io/github/v/release/Xiaokang2022/tkintertools?include_prereleases&logo=github&label=Version" title="Latest Version" /></a>
+<a href="./LICENSE.txt"><img alt="License" src="https://img.shields.io/github/license/Xiaokang2022/tkintertools?logo=github&label=License" title="License" /></a>
+<a href="https://pypistats.org/packages/tkintertools"><img alt="Downloads" src="https://img.shields.io/pypi/dm/tkintertools?label=Downloads&logo=pypi&logoColor=skyblue" title="Downloads" /></a>
 <a href="https://pepy.tech/project/tkintertools"><img alt="Total Downloads" src="https://static.pepy.tech/badge/tkintertools" title="Total Downloads" /></a>
-<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size" title="Code Size"/></a>
+<a href="https://github.com/Xiaokang2022/tkintertools"><img alt="Size" src="https://img.shields.io/github/languages/code-size/Xiaokang2022/tkintertools?label=Size&logo=github" title="Code Size"/></a>
 <br/>
 <a href="https://github.com/Xiaokang2022/tkintertools/watchers"><img alt="Watchers" src="https://img.shields.io/github/watchers/Xiaokang2022/tkintertools?label=Watchers&logo=github&style=flat" title="Watchers" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/forks"><img alt="Forks" src="https://img.shields.io/github/forks/Xiaokang2022/tkintertools?label=Forks&logo=github&style=flat" title="Forks" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/Xiaokang2022/tkintertools?label=Stars&color=gold&logo=github&style=flat" title="Stars" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/issues"><img alt="Issues" src="https://img.shields.io/github/issues/Xiaokang2022/tkintertools?label=Issues&logo=github" title="Issues" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/pulls"><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/Xiaokang2022/tkintertools?label=Pull%20Requests&logo=github" title="Pull Requests" /></a>
 <a href="https://github.com/Xiaokang2022/tkintertools/discussions"><img alt="Discussions" src="https://img.shields.io/github/discussions/Xiaokang2022/tkintertools?label=Discussions&logo=github" title="Discussions" /></a>
@@ -80,59 +86,84 @@
             <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date&theme=dark" />
             <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
             <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=Xiaokang2022/tkintertools&type=Date" />
         </picture>
     </a>
 </p>
 
-Install - 模块安装
------------------
+📦 Installation - 安装
+-----------------------
 
-### Stable Version - 稳定版本
+### ✅ Stable Version - 稳定版本
 
 * 🔖 Version - 最新版本 : `2.6.21`
 * 🕓 Release - 发布日期 : 2024-01-01
 * ✨ Feature - 更新内容 : [News-2.6.21](https://xiaokang2022.github.io/tkintertools/news/2.6.21/News/)
 
 ```sh
 pip install tkintertools
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
 
 [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
 
 [![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/#%E4%B8%89%E9%80%9A%E8%BF%87-after-%E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB)
 
 </details>
 
-### Development Version - 开发版本
+### 🔥 Development Version - 开发版本
 
-* 🔖 Version - 最新版本 : `3.0.0.beta1`
-* 🕓 Release - 发布日期 : 2024-05-17
-* ✨ Feature - 更新内容 : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
+* 🔖 Version - 最新版本 : `3.0.0.beta2`
+* 🕓 Release - 发布日期 : 2024-06-03
+* ✨ Feature - 更新内容 : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/)
 
 ```sh
-
+pip install tkintertools==3.0.0b2
 ```
 
-<details open><summary>Preview - 预览</summary>
+<details open><summary>👁️ Preview - 预览</summary>
+
+* **Windows 11 Dark Theme**
+
+![Light - Win11](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png)
+
+* **Windows 10 Light Theme**
+
+![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-win10.png)
+
+* **Ubuntu 24.04 (GNOME) Dark Theme**
 
-[![Light Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+![Light - Ubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png)
 
-[![Dark Theme](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95)
+* **Kubuntu 24.04 (KDE) Light Theme**
+
+![Light - Kubuntu](https://xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png)
+
+* **macOS Dark Theme**
+
+![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-mac.png)
 
 </details>
 
-> [!IMPORTANT]  
+> [!WARNING]  
 > `tkt 2.*` has been discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*` can be difficult.  
 > `tkt 2.*` 已放弃支持，如需获取新的功能，请使用 `tkt 3.*`。同时请注意，`tkt 3.*` 与 `tkt 2.*` 几乎完全不兼容，将项目从 `tkt 2.*` 移植到 `tkt 3.*` 可能会十分困难。
 
-More - 更多
------------
+📦 Dependency packages - 依赖包
+-------------------------------
+
+### 1️⃣ darkdetect
+
+* 🔖 Version - 版本 : `0.8.0`
+* 📑 License - 许可 : BSD 3-Clause
+* 🔗 GitHub - 仓库 : [darkdetect](https://github.com/albertosottile/darkdetect)
+
+👀 More - 更多
+---------------
 
 * 📋 Todo - 待办事项: [TODO.md](TODO.md)
 * 📑 License - 项目许可: [LICENSE.txt](LICENSE.txt)
 * 📘 Changelog - 更新日志: [CHANGELOG.md](CHANGELOG.md)
 * 📕 Security Policy - 安全策略: [SECURITY.md](SECURITY.md)
 * 📗 Contribution Guide - 贡献指南: [CONTRIBUTING.md](CONTRIBUTING.md)
 * 📙 Code of Conduct - 行为准则: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 3.0.0b1 Summary: tkintertools
+Metadata-Version: 2.1 Name: tkintertools Version: 3.0.0b2 Summary: tkintertools
 is a UI framework based on the Canvas class of tkinter Author-email:
 Xiaokang2022 <2951256653@qq.com> Maintainer-email: Xiaokang2022
-<2951256653@qq.com> License: MIT License Copyright (c) 2024 å°åº·2022
+<2951256653@qq.com> License: MIT License Copyright (c) 2024 Xiaokang2022
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions: The above copyright notice and this
 permission notice shall be included in all copies or substantial portions of
@@ -22,55 +22,72 @@
 platform,themed Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: MacOS Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Software Development :: Widget Sets Classifier:
-Typing :: Typed Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.txt Requires-Dist: darkdetect[macos-listener]
+Typing :: Typed Classifier: Development Status :: 4 - Beta Requires-Python:
+>=3.10 Description-Content-Type: text/markdown License-File: LICENSE.txt
+Requires-Dist: darkdetect Requires-Dist: darkdetect[macos-listener] >
+[!IMPORTANT] > Due to the growing nature of the project, the original name
+`tkintertools` is no longer in line with its original intended, so the project
+is going to be renamed to "tkinter advanced canvas UI framework" (`tacUI`) in
+version `3.0.0.rc1`. If you have any other ideas or suggestions, you can put
+them in the discussion forum. > ç±äºæ¬é¡¹ç®çä¸æ­å£®å¤§ï¼ååç§°
+`tkintertools` å·²ä¸ç¬¦åå¶æ¬æï¼ææ¬é¡¹ç®åå¤å¨è¿å¥ `3.0.0.rc1`
+çæ¬æ¶æ´åä¸º âtkinter advanced canvas UI
+frameworkâï¼`tacUI`ï¼ãå¦æå¶å®æ³æ³æå»ºè®®ï¼å¯å¨è®¨è®ºåºä¸­æåºã
                           ************ ttkkiinntteerrttoooollss ************
                                     [logo]
        tkintertools æ¯ä¸ä¸ªåºäº tkinter ç Canvas ç±»ç UI æ¡æ¶
       tkintertools is a UI framework based on the Canvas class of tkinter
              _[_V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_D_o_w_n_l_o_a_d_s_]_[_T_o_t_a_l_ _D_o_w_n_l_o_a_d_s_]_[_S_i_z_e_]
          _[_W_a_t_c_h_e_r_s_]_[_F_o_r_k_s_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_P_u_l_l_ _R_e_q_u_e_s_t_s_]_[_D_i_s_c_u_s_s_i_o_n_s_]
                                   _[_I_n_s_i_g_h_t_s_]
                              _[_S_t_a_r_ _H_i_s_t_o_r_y_ _C_h_a_r_t_]
-Install - æ¨¡åå®è£ ----------------- ### Stable Version - ç¨³å®çæ¬ *
-ð Version - ææ°çæ¬ : `2.6.21` * ð Release - åå¸æ¥æ : 2024-01-
-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://xiaokang2022.github.io/
-tkintertools/news/2.6.21/News/) ```sh pip install tkintertools ``` Preview -
-é¢è§ [![Preview UI](https://xiaokang2022.github.io/tkintertools/tutorials/
-images/1.2-2.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/1-
-2/#21-%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6)
-[![Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/
-7.3-3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
+ð¦ Installation - å®è£ ----------------------- ### â Stable Version -
+ç¨³å®çæ¬ * ð Version - ææ°çæ¬ : `2.6.21` * ð Release -
+åå¸æ¥æ : 2024-01-01 * â¨ Feature - æ´æ°åå®¹ : [News-2.6.21](https://
+xiaokang2022.github.io/tkintertools/news/2.6.21/News/) ```sh pip install
+tkintertools ``` ðï¸ Preview - é¢è§ [![Preview UI](https://
+xiaokang2022.github.io/tkintertools/tutorials/images/1.2-2.1-2.png)](https://
+xiaokang2022.github.io/tkintertools/tutorials/1-2/#21-
+%E9%AB%98%E5%BA%A6%E5%8F%AF%E9%85%8D%E7%BD%AE%E7%9A%84%E6%8E%A7%E4%BB%B6) [!
+[Preview 3D](https://xiaokang2022.github.io/tkintertools/tutorials/images/7.3-
+3.1-2.png)](https://xiaokang2022.github.io/tkintertools/tutorials/7-3/
 #%E4%B8%89%E9%80%9A%E8%BF%87-after-
 %E6%96%B9%E6%B3%95%E5%AE%9E%E7%8E%B0%E7%AE%80%E5%8D%95%E5%8A%A8%E7%94%BB) ###
-Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
-`3.0.0.beta1` * ð Release - åå¸æ¥æ : 2024-05-17 * â¨ Feature -
-æ´æ°åå®¹ : [News-3.0.0](https://xiaokang2022.github.io/tkintertools/news/
-3.0.0/News/) ```sh ``` Preview - é¢è§ [![Light Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/light.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) [![Dark Theme](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/dark.png)](https://
-xiaokang2022.github.io/tkintertools/news/3.0.0/News/#base-test---
-%E5%9F%BA%E7%A1%80%E6%B5%8B%E8%AF%95) > [!IMPORTANT] > `tkt 2.*` has been
-discontinued, for new features, please use `tkt 3.*`. Also note that `tkt 3.*`
-is almost completely incompatible with `tkt 2.*`, and porting a project from
-`tkt 2.*` to `tkt 3.*` can be difficult. > `tkt 2.*`
+ð¥ Development Version - å¼åçæ¬ * ð Version - ææ°çæ¬ :
+`3.0.0.beta2` * ð Release - åå¸æ¥æ : 2024-06-03 * â¨ Feature -
+æ´æ°åå®¹ : [News-3.0.0b2](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/News/) ```sh pip install tkintertools==3.0.0b2 ``` ðï¸ Preview -
+é¢è§ * **Windows 11 Dark Theme** ![Light - Win11](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/dark-win11.png) * **Windows 10
+Light Theme** ![Dark - Win10](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/light-win10.png) * **Ubuntu 24.04 (GNOME) Dark Theme** ![Light - Ubuntu]
+(https://xiaokang2022.github.io/tkintertools/news/3.0.0/dark-ubuntu.png) *
+**Kubuntu 24.04 (KDE) Light Theme** ![Light - Kubuntu](https://
+xiaokang2022.github.io/tkintertools/news/3.0.0/light-kubuntu.png) * **macOS
+Dark Theme** ![Dark - MacOS](https://xiaokang2022.github.io/tkintertools/news/
+3.0.0/dark-mac.png) > [!WARNING] > `tkt 2.*` has been discontinued, for new
+features, please use `tkt 3.*`. Also note that `tkt 3.*` is almost completely
+incompatible with `tkt 2.*`, and porting a project from `tkt 2.*` to `tkt 3.*`
+can be difficult. > `tkt 2.*`
 å·²æ¾å¼æ¯æï¼å¦éè·åæ°çåè½ï¼è¯·ä½¿ç¨ `tkt
 3.*`ãåæ¶è¯·æ³¨æï¼`tkt 3.*` ä¸ `tkt 2.*`
 å ä¹å®å¨ä¸å¼å®¹ï¼å°é¡¹ç®ä» `tkt 2.*` ç§»æ¤å° `tkt 3.*`
-å¯è½ä¼ååå°é¾ã More - æ´å¤ ----------- * ð Todo - å¾åäºé¡¹:
-[TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯: [LICENSE.txt](LICENSE.txt) *
-ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md](CHANGELOG.md) * ð Security
-Policy - å®å¨ç­ç¥: [SECURITY.md](SECURITY.md) * ð Contribution Guide -
-è´¡ç®æå: [CONTRIBUTING.md](CONTRIBUTING.md) * ð Code of Conduct -
-è¡ä¸ºåå: [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) * ð Tutorials and
-Documents - æç¨åææ¡£: [Tutorials & Documents](https://
-xiaokang2022.github.io/tkintertools/) * ð Repository Mirrors -
-å­å¨åºéåæº: [GitHub](https://github.com/Xiaokang2022/tkintertools) |
-[Gitee](https://gitee.com/xiaokang-2022/tkintertools) | [GitCode](https://
-gitcode.com/Xiaokang2022/tkintertools/overview)
+å¯è½ä¼ååå°é¾ã ð¦ Dependency packages - ä¾èµå -----------------
+-------------- ### 1ï¸â£ darkdetect * ð Version - çæ¬ : `0.8.0` * ð
+License - è®¸å¯ : BSD 3-Clause * ð GitHub - ä»åº : [darkdetect](https://
+github.com/albertosottile/darkdetect) ð More - æ´å¤ --------------- * ð
+Todo - å¾åäºé¡¹: [TODO.md](TODO.md) * ð License - é¡¹ç®è®¸å¯:
+[LICENSE.txt](LICENSE.txt) * ð Changelog - æ´æ°æ¥å¿: [CHANGELOG.md]
+(CHANGELOG.md) * ð Security Policy - å®å¨ç­ç¥: [SECURITY.md]
+(SECURITY.md) * ð Contribution Guide - è´¡ç®æå: [CONTRIBUTING.md]
+(CONTRIBUTING.md) * ð Code of Conduct - è¡ä¸ºåå: [CODE_OF_CONDUCT.md]
+(CODE_OF_CONDUCT.md) * ð Tutorials and Documents - æç¨åææ¡£:
+[Tutorials & Documents](https://xiaokang2022.github.io/tkintertools/) * ð
+Repository Mirrors - å­å¨åºéåæº: [GitHub](https://github.com/
+Xiaokang2022/tkintertools) | [Gitee](https://gitee.com/xiaokang-2022/
+tkintertools) | [GitCode](https://gitcode.com/Xiaokang2022/tkintertools/
+overview)
```

### Comparing `tkintertools-3.0.0b1/tkintertools.egg-info/SOURCES.txt` & `tkintertools-3.0.0b2/tkintertools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 tkintertools/__init__.py
-tkintertools/constants.py
-tkintertools/core.py
 tkintertools.egg-info/PKG-INFO
 tkintertools.egg-info/SOURCES.txt
 tkintertools.egg-info/dependency_links.txt
 tkintertools.egg-info/requires.txt
 tkintertools.egg-info/top_level.txt
 tkintertools/animation/__init__.py
 tkintertools/animation/animations.py
 tkintertools/animation/controllers.py
 tkintertools/color/__init__.py
 tkintertools/color/colormap.py
+tkintertools/color/hsl.py
 tkintertools/color/rgb.py
+tkintertools/core/__init__.py
+tkintertools/core/constants.py
+tkintertools/core/containers.py
+tkintertools/core/virtual.py
 tkintertools/standard/__init__.py
 tkintertools/standard/dialogs.py
 tkintertools/standard/features.py
 tkintertools/standard/images.py
 tkintertools/standard/shapes.py
 tkintertools/standard/texts.py
 tkintertools/standard/widgets.py
@@ -79,8 +82,12 @@
 tkintertools/theme/Switch/Rectangle.out.dark.json
 tkintertools/theme/Switch/Rectangle.out.light.json
 tkintertools/theme/Switch/SemicircularRectangle.dark.json
 tkintertools/theme/Switch/SemicircularRectangle.light.json
 tkintertools/theme/UnderlineButton/Information.dark.json
 tkintertools/theme/UnderlineButton/Information.light.json
 tkintertools/three/__init__.py
-tkintertools/three/engine.py
+tkintertools/three/engine.py
+tkintertools/three/geometries.py
+tkintertools/toolbox/__init__.py
+tkintertools/toolbox/enhanced.py
+tkintertools/toolbox/tools.py
```

