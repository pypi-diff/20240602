# Comparing `tmp/janim-1.2.1.tar.gz` & `tmp/janim-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.2.1.tar` & `janim-1.2.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0      153 2024-05-30 07:45:35.530129 janim-1.2.1/.gitignore
--rw-r--r--   0        0        0     1011 2024-05-30 07:45:35.530129 janim-1.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1085 2024-05-30 07:45:35.534129 janim-1.2.1/LICENSE
--rw-r--r--   0        0        0     1208 2024-05-30 07:45:35.534129 janim-1.2.1/README.md
--rw-r--r--   0        0        0       68 2024-05-30 07:45:35.578128 janim-1.2.1/janim/__init__.py
--rw-r--r--   0        0        0     3412 2024-05-30 07:45:35.578128 janim-1.2.1/janim/__main__.py
--rw-r--r--   0        0        0     4108 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/animation.py
--rw-r--r--   0        0        0     6203 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/composition.py
--rw-r--r--   0        0        0     5842 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/creation.py
--rw-r--r--   0        0        0      784 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/display.py
--rw-r--r--   0        0        0     3339 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/fading.py
--rw-r--r--   0        0        0     3799 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/growing.py
--rw-r--r--   0        0        0    12480 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/indication.py
--rw-r--r--   0        0        0     2375 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/movement.py
--rw-r--r--   0        0        0     1501 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/rotation.py
--rw-r--r--   0        0        0    28675 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/timeline.py
--rw-r--r--   0        0        0     8961 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/transform.py
--rw-r--r--   0        0        0     9907 2024-05-30 07:45:35.578128 janim-1.2.1/janim/anims/updater.py
--rw-r--r--   0        0        0     4360 2024-05-30 07:45:35.578128 janim-1.2.1/janim/camera/camera.py
--rw-r--r--   0        0        0     2768 2024-05-30 07:45:35.578128 janim-1.2.1/janim/camera/camera_info.py
--rw-r--r--   0        0        0     7387 2024-05-30 07:45:35.578128 janim-1.2.1/janim/cli.py
--rw-r--r--   0        0        0     8927 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/component.py
--rw-r--r--   0        0        0     2331 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/data.py
--rw-r--r--   0        0        0     2518 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/depth.py
--rw-r--r--   0        0        0     1239 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/image.py
--rw-r--r--   0        0        0    30723 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/points.py
--rw-r--r--   0        0        0     2733 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/radius.py
--rw-r--r--   0        0        0     7677 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/rgbas.py
--rw-r--r--   0        0        0    21993 2024-05-30 07:45:35.578128 janim-1.2.1/janim/components/vpoints.py
--rw-r--r--   0        0        0      236 2024-05-30 07:45:35.578128 janim-1.2.1/janim/constants/__init__.py
--rw-r--r--   0        0        0      162 2024-05-30 07:45:35.578128 janim-1.2.1/janim/constants/alignment.py
--rw-r--r--   0        0        0     1469 2024-05-30 07:45:35.578128 janim-1.2.1/janim/constants/colors.py
--rw-r--r--   0        0        0      614 2024-05-30 07:45:35.578128 janim-1.2.1/janim/constants/coord.py
--rw-r--r--   0        0        0      171 2024-05-30 07:45:35.578128 janim-1.2.1/janim/constants/degrees.py
--rw-r--r--   0        0        0     5265 2024-05-30 07:45:35.578128 janim-1.2.1/janim/examples.py
--rw-r--r--   0        0        0     1654 2024-05-30 07:45:35.578128 janim-1.2.1/janim/exception.py
--rw-r--r--   0        0        0    21829 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      319 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/application.py
--rw-r--r--   0        0        0      766 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/export.png
--rw-r--r--   0        0        0    16958 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/favicon.ico
--rw-r--r--   0        0        0     1458 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0     3722 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/font_table.py
--rw-r--r--   0        0        0     1508 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/glwidget.py
--rw-r--r--   0        0        0     1011 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5162 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     1764 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/search.png
--rw-r--r--   0        0        0     8115 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/selector.py
--rw-r--r--   0        0        0    24412 2024-05-30 07:45:35.582128 janim-1.2.1/janim/gui/timeline_view.py
--rw-r--r--   0        0        0     1699 2024-05-30 07:45:35.582128 janim-1.2.1/janim/imports.py
--rw-r--r--   0        0        0     7886 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/audio.py
--rw-r--r--   0        0        0     5190 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8569 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2093 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8078 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8471 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6679 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7653 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5077 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5071 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/image_item.py
--rw-r--r--   0        0        0    18849 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/item.py
--rw-r--r--   0        0        0     3149 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/points.py
--rw-r--r--   0        0        0     7446 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/relation.py
--rw-r--r--   0        0        0     2012 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5764 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1719 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4298 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     2979 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/svg/typst.py
--rw-r--r--   0        0        0       37 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    15877 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/text/text.py
--rw-r--r--   0        0        0     1053 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5204 2024-05-30 07:45:35.582128 janim-1.2.1/janim/items/vitem.py
--rw-r--r--   0        0        0      258 2024-05-30 07:45:35.582128 janim-1.2.1/janim/logger.py
--rw-r--r--   0        0        0     3242 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/base.py
--rw-r--r--   0        0        0     9282 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/impl.py
--rw-r--r--   0        0        0      427 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1200 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      502 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      167 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      533 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6752 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      190 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1083 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/texture.py
--rw-r--r--   0        0        0     6771 2024-05-30 07:45:35.582128 janim-1.2.1/janim/render/writer.py
--rw-r--r--   0        0        0      931 2024-05-30 07:45:35.582128 janim-1.2.1/janim/typing.py
--rw-r--r--   0        0        0    16826 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/bezier.py
--rw-r--r--   0        0        0     5365 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/config.py
--rw-r--r--   0        0        0     5590 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/data.py
--rw-r--r--   0        0        0      618 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2400 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/file_ops.py
--rw-r--r--   0        0        0     4519 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/font.py
--rw-r--r--   0        0        0     6192 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5767 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/iterables.py
--rw-r--r--   0        0        0     1810 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/paths.py
--rw-r--r--   0        0        0     2601 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2566 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/refresh.py
--rw-r--r--   0        0        0     8074 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/signal.py
--rw-r--r--   0        0        0     1919 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/simple_functions.py
--rw-r--r--   0        0        0     9707 2024-05-30 07:45:35.582128 janim-1.2.1/janim/utils/space_ops.py
--rw-r--r--   0        0        0    18504 2024-05-30 07:45:35.582128 janim-1.2.1/logo.png
--rw-r--r--   0        0        0     1018 2024-05-30 07:45:35.582128 janim-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 janim-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2024-06-02 15:35:27.663867 janim-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1011 2024-06-02 15:35:27.663867 janim-1.2.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1085 2024-06-02 15:35:27.667867 janim-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1208 2024-06-02 15:35:27.667867 janim-1.2.2/README.md
+-rw-r--r--   0        0        0       68 2024-06-02 15:35:27.715868 janim-1.2.2/janim/__init__.py
+-rw-r--r--   0        0        0     3412 2024-06-02 15:35:27.715868 janim-1.2.2/janim/__main__.py
+-rw-r--r--   0        0        0     4108 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/animation.py
+-rw-r--r--   0        0        0     6250 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/composition.py
+-rw-r--r--   0        0        0     5842 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/creation.py
+-rw-r--r--   0        0        0      784 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/display.py
+-rw-r--r--   0        0        0     3339 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/fading.py
+-rw-r--r--   0        0        0     3799 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/growing.py
+-rw-r--r--   0        0        0    12480 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/indication.py
+-rw-r--r--   0        0        0     2375 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/movement.py
+-rw-r--r--   0        0        0     1501 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/rotation.py
+-rw-r--r--   0        0        0    28772 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/timeline.py
+-rw-r--r--   0        0        0     8961 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/transform.py
+-rw-r--r--   0        0        0     9907 2024-06-02 15:35:27.715868 janim-1.2.2/janim/anims/updater.py
+-rw-r--r--   0        0        0     4360 2024-06-02 15:35:27.715868 janim-1.2.2/janim/camera/camera.py
+-rw-r--r--   0        0        0     3414 2024-06-02 15:35:27.715868 janim-1.2.2/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     7387 2024-06-02 15:35:27.715868 janim-1.2.2/janim/cli.py
+-rw-r--r--   0        0        0     8927 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/component.py
+-rw-r--r--   0        0        0     2331 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/data.py
+-rw-r--r--   0        0        0     2518 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/depth.py
+-rw-r--r--   0        0        0     1239 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/image.py
+-rw-r--r--   0        0        0    30723 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/points.py
+-rw-r--r--   0        0        0     2733 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/radius.py
+-rw-r--r--   0        0        0     7677 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/rgbas.py
+-rw-r--r--   0        0        0    21993 2024-06-02 15:35:27.715868 janim-1.2.2/janim/components/vpoints.py
+-rw-r--r--   0        0        0      236 2024-06-02 15:35:27.715868 janim-1.2.2/janim/constants/__init__.py
+-rw-r--r--   0        0        0      162 2024-06-02 15:35:27.715868 janim-1.2.2/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1469 2024-06-02 15:35:27.715868 janim-1.2.2/janim/constants/colors.py
+-rw-r--r--   0        0        0      614 2024-06-02 15:35:27.715868 janim-1.2.2/janim/constants/coord.py
+-rw-r--r--   0        0        0      171 2024-06-02 15:35:27.715868 janim-1.2.2/janim/constants/degrees.py
+-rw-r--r--   0        0        0     5265 2024-06-02 15:35:27.715868 janim-1.2.2/janim/examples.py
+-rw-r--r--   0        0        0     1654 2024-06-02 15:35:27.715868 janim-1.2.2/janim/exception.py
+-rw-r--r--   0        0        0    21870 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      319 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/application.py
+-rw-r--r--   0        0        0      766 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/export.png
+-rw-r--r--   0        0        0    16958 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/favicon.ico
+-rw-r--r--   0        0        0     1458 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0     3722 2024-06-02 15:35:27.715868 janim-1.2.2/janim/gui/font_table.py
+-rw-r--r--   0        0        0     1508 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/glwidget.py
+-rw-r--r--   0        0        0     1011 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5162 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     1764 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/search.png
+-rw-r--r--   0        0        0     8115 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/selector.py
+-rw-r--r--   0        0        0    24504 2024-06-02 15:35:27.719868 janim-1.2.2/janim/gui/timeline_view.py
+-rw-r--r--   0        0        0     1699 2024-06-02 15:35:27.719868 janim-1.2.2/janim/imports.py
+-rw-r--r--   0        0        0     7886 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/audio.py
+-rw-r--r--   0        0        0     5190 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8569 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2093 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8078 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8471 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6679 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7653 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5077 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5071 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/image_item.py
+-rw-r--r--   0        0        0    18849 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/item.py
+-rw-r--r--   0        0        0     3149 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/points.py
+-rw-r--r--   0        0        0     7446 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/relation.py
+-rw-r--r--   0        0        0     2012 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5764 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1719 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4298 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     2979 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       37 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    15877 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/text/text.py
+-rw-r--r--   0        0        0     1053 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5204 2024-06-02 15:35:27.719868 janim-1.2.2/janim/items/vitem.py
+-rw-r--r--   0        0        0      258 2024-06-02 15:35:27.719868 janim-1.2.2/janim/logger.py
+-rw-r--r--   0        0        0     3242 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/base.py
+-rw-r--r--   0        0        0     9400 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/impl.py
+-rw-r--r--   0        0        0      427 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1200 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      506 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      167 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      537 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6752 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      190 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1083 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/texture.py
+-rw-r--r--   0        0        0     6771 2024-06-02 15:35:27.719868 janim-1.2.2/janim/render/writer.py
+-rw-r--r--   0        0        0      931 2024-06-02 15:35:27.719868 janim-1.2.2/janim/typing.py
+-rw-r--r--   0        0        0    16826 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5365 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/config.py
+-rw-r--r--   0        0        0     5590 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/data.py
+-rw-r--r--   0        0        0      618 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2400 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     4519 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/font.py
+-rw-r--r--   0        0        0     6192 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5767 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1810 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/paths.py
+-rw-r--r--   0        0        0     2601 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2566 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8074 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/signal.py
+-rw-r--r--   0        0        0     1919 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0     9707 2024-06-02 15:35:27.719868 janim-1.2.2/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    18504 2024-06-02 15:35:27.719868 janim-1.2.2/logo.png
+-rw-r--r--   0        0        0     1018 2024-06-02 15:35:27.719868 janim-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 janim-1.2.2/PKG-INFO
```

### Comparing `janim-1.2.1/.readthedocs.yaml` & `janim-1.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/LICENSE` & `janim-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/README.md` & `janim-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/__main__.py` & `janim-1.2.2/janim/__main__.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/animation.py` & `janim-1.2.2/janim/anims/animation.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/composition.py` & `janim-1.2.2/janim/anims/composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,17 @@
         '''
         计算子动画的时间范围
 
         该方法是被 :meth:`~.Timeline.prepare` 调用以计算的
         '''
         super().compute_global_range(at, duration)
 
+        if not self.anims:
+            return
+
         factor = duration / self.maxt
 
         for anim in self.anims:
             anim.compute_global_range(
                 self.global_range.at + anim.local_range.at * factor,
                 anim.local_range.duration * factor
             )
```

### Comparing `janim-1.2.1/janim/anims/creation.py` & `janim-1.2.2/janim/anims/creation.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/display.py` & `janim-1.2.2/janim/anims/display.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/fading.py` & `janim-1.2.2/janim/anims/fading.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/growing.py` & `janim-1.2.2/janim/anims/growing.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/indication.py` & `janim-1.2.2/janim/anims/indication.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/movement.py` & `janim-1.2.2/janim/anims/movement.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/rotation.py` & `janim-1.2.2/janim/anims/rotation.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/timeline.py` & `janim-1.2.2/janim/anims/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             if not quiet:   # pragma: no cover
                 log.info(f'Building "{self.__class__.__name__}"')
                 start_time = time.time()
 
             self.construct()
 
             if self.current_time == 0:
-                self.forward(DEFAULT_DURATION)  # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
+                self.forward(DEFAULT_DURATION, _record_lineno=False)    # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
                 if not quiet:   # pragma: no cover
                     log.info(f'"{self.__class__.__name__}" 构建后没有产生时长，自动产生了 {DEFAULT_DURATION}s 的时长')
             self.cleanup_display()
             global_anim = TimelineAnim(self)
 
             if not quiet:   # pragma: no cover
                 elapsed = time.time() - start_time
@@ -218,22 +218,21 @@
     def schedule(self, at: float, func: Callable, *args, **kwargs) -> None:
         '''
         计划执行
 
         会在进度达到 ``at`` 时，对 ``func`` 进行调用，
         可传入 ``*args`` 和 ``**kwargs``
         '''
-        rough_at = round(at, 4)   # 防止因为精度误差使得本来计划更迟的任务被更早地执行了
+        rough_at = math.ceil(at * 1e4) / 1e4    # 防止因为精度误差使得本来计划更迟的任务被更早地执行了
         task = Timeline.ScheduledTask(rough_at, func, args, kwargs)
         insort(self.scheduled_tasks, task, key=lambda x: x.at)
-        task.at = at
 
     # region progress
 
-    def forward(self, dt: float = 1, *, _detect_changes=True) -> None:
+    def forward(self, dt: float = 1, *, _detect_changes=True, _record_lineno=True) -> None:
         '''
         向前推进 ``dt`` 秒
         '''
         if dt <= 0:
             raise ValueError('dt 必须大于 0')
 
         if _detect_changes:
@@ -244,20 +243,21 @@
         while self.scheduled_tasks and self.scheduled_tasks[0].at <= to_time:
             task = self.scheduled_tasks.pop(0)
             self.current_time = task.at
             task.func(*task.args, **task.kwargs)
 
         self.current_time = to_time
 
-        self.times_of_code.append(
-            Timeline.TimeOfCode(
-                self.current_time,
-                self.get_construct_lineno() or -1
+        if _record_lineno:
+            self.times_of_code.append(
+                Timeline.TimeOfCode(
+                    self.current_time,
+                    self.get_construct_lineno() or -1
+                )
             )
-        )
 
     def forward_to(self, t: float, *, _detect_changes=True) -> None:
         '''
         向前推进到 ``t`` 秒的时候
         '''
         self.forward(t - self.current_time, _detect_changes=_detect_changes)
 
@@ -792,15 +792,15 @@
                 timeline = self.timeline
                 camera_info = timeline.camera.current().points.info
                 anti_alias_radius = self.cfg.anti_alias_width / 2 * camera_info.scaled_factor
 
                 set_global_uniforms(
                     ctx,
                     ('JA_VIEW_MATRIX', camera_info.view_matrix.T.flatten()),
-                    ('JA_DISTANCE_FROM_PLANE', camera_info.distance_from_plane),
+                    ('JA_FIXED_DIST_FROM_PLANE', camera_info.fixed_distance_from_plane),
                     ('JA_PROJ_MATRIX', camera_info.proj_matrix.T.flatten()),
                     ('JA_FRAME_RADIUS', camera_info.frame_radius),
                     ('JA_ANTI_ALIAS_RADIUS', anti_alias_radius)
                 )
 
                 with ContextSetter(Renderer.data_ctx, RenderData(ctx=ctx,
                                                                  camera_info=camera_info,
```

### Comparing `janim-1.2.1/janim/anims/transform.py` & `janim-1.2.2/janim/anims/transform.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/anims/updater.py` & `janim-1.2.2/janim/anims/updater.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/camera/camera.py` & `janim-1.2.2/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/camera/camera_info.py` & `janim-1.2.2/janim/camera/camera_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,25 +15,31 @@
     center: np.ndarray
     horizontal_vect: np.ndarray
     vertical_vect: np.ndarray
 
     horizontal_dist: float = field(init=False)
     vertical_dist: float = field(init=False)
 
+    distance_from_plane: float = field(init=False)
+    fixed_distance_from_plane: float = field(init=False)
+
     camera_location: np.ndarray = field(init=False)
 
     view_matrix: np.ndarray = field(init=False)
     proj_matrix: np.ndarray = field(init=False)
     proj_view_matrix: np.ndarray = field(init=False)
     frame_radius: np.ndarray = field(init=False)
 
     def __post_init__(self):
         self.horizontal_dist = get_norm(self.horizontal_vect)
         self.vertical_dist = get_norm(self.vertical_vect)
 
+        self.distance_from_plane = self._compute_distance_from_plane(self.vertical_dist)
+        self.fixed_distance_from_plane = self._compute_distance_from_plane(self.vertical_dist / self.scaled_factor)
+
         self.camera_location = self._compute_camera_location()
 
         self.view_matrix = self._compute_view_matrix()
         self.proj_matrix = self._compute_proj_matrix()
         self.proj_view_matrix = np.dot(self.proj_matrix, self.view_matrix)
         self.frame_radius = np.array([self.horizontal_dist, self.vertical_dist]) / 2
 
@@ -45,18 +51,24 @@
         aligned = np.hstack([
             points,
             np.full((len(points), 1), 1)
         ])
         mapped = np.dot(aligned, self.proj_view_matrix.T)
         return mapped[:, :2] / mapped[:, 3].reshape((len(mapped), 1))
 
-    @property
-    def distance_from_plane(self) -> float:
-        up = self.vertical_vect
-        return get_norm(up) / 2 / math.tan(math.radians(self.fov / 2))
+    def map_fixed_in_frame_points(self, points: VectArray) -> np.ndarray:
+        aligned = np.hstack([
+            points - [0, 0, self.fixed_distance_from_plane],
+            np.full((len(points), 1), 1)
+        ])
+        mapped = np.dot(aligned, self.proj_matrix.T)
+        return mapped[:, :2] / mapped[:, 3].reshape((len(mapped), 1))
+
+    def _compute_distance_from_plane(self, vertical_length: float) -> float:
+        return vertical_length / 2 / math.tan(math.radians(self.fov / 2))
 
     def _compute_camera_location(self) -> np.ndarray:
         right = self.horizontal_vect
         up = self.vertical_vect
         normal = get_unit_normal(right, up)
         return self.center + normal * self.distance_from_plane
```

### Comparing `janim-1.2.1/janim/cli.py` & `janim-1.2.2/janim/cli.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/component.py` & `janim-1.2.2/janim/components/component.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/data.py` & `janim-1.2.2/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/depth.py` & `janim-1.2.2/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/image.py` & `janim-1.2.2/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/points.py` & `janim-1.2.2/janim/components/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/radius.py` & `janim-1.2.2/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/rgbas.py` & `janim-1.2.2/janim/components/rgbas.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/components/vpoints.py` & `janim-1.2.2/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/constants/colors.py` & `janim-1.2.2/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/constants/coord.py` & `janim-1.2.2/janim/constants/coord.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/examples.py` & `janim-1.2.2/janim/examples.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/exception.py` & `janim-1.2.2/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/anim_viewer.py` & `janim-1.2.2/janim/gui/anim_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
         self.time_label = QLabel()
         self.name_edit = QLineEdit()
         self.btn_export = QPushButton()
         self.btn_export.setIcon(QIcon(os.path.join(get_janim_dir(), 'gui', 'export.png')))
         self.btn_export.setFocusPolicy(Qt.FocusPolicy.NoFocus)
 
         stb = self.statusBar()
+        stb.setFixedHeight(stb.height())
         stb.setContentsMargins(0, 0, 0, 0)
         stb.addWidget(self.fps_label)
         stb.addPermanentWidget(self.name_edit)
         stb.addPermanentWidget(self.time_label)
         stb.addPermanentWidget(self.btn_export)
 
     def setup_central_widget(self) -> None:
@@ -325,30 +326,14 @@
                 traceback.print_exc()
             log.error('重新构建失败')
             return
 
         range = self.timeline_view.range
         self.set_anim(anim)
 
-        # 向 vscode 客户端发送重新构建了的信息
-        if self.socket is not None:
-            msg = json.dumps(dict(
-                janim=dict(
-                    type='rebuilt'
-                )
-            ))
-            for client in self.clients:
-                self.socket.writeDatagram(
-                    QByteArray.fromStdString(msg),
-                    *client
-                )
-
-            time = self.timeline_view.progress_to_time(self.timeline_view.progress())
-            self.send_lineno(self.anim.timeline.get_lineno_at_time(time))
-
         if not stay_same:
             self.anim.anim_on(0)
             self.timeline_view.set_progress(0)
         else:
             # 把原来进度（所在第几帧）转换到新的进度
             # 如果帧率没变，则进度不变
             # 如果帧率变了，例如从 30fps 到 60fps，则进度 43 对应 进度 86（乘了 2）
@@ -359,14 +344,30 @@
 
             # 设置 range 是为了保留动画标签的相对位置
             # 比如，本来是 0~1s 和 1~2s 分别一个动画
             # 重新构建后，只剩下了 0~1s 的动画
             # 那么仍保留原来的显示范围，使得 0~1s 的显示位置不变，虽然显示范围超出了持续时间
             self.timeline_view.range = range
 
+        # 向 vscode 客户端发送重新构建了的信息
+        if self.socket is not None:
+            msg = json.dumps(dict(
+                janim=dict(
+                    type='rebuilt'
+                )
+            ))
+            for client in self.clients:
+                self.socket.writeDatagram(
+                    QByteArray.fromStdString(msg),
+                    *client
+                )
+
+            time = self.timeline_view.progress_to_time(self.timeline_view.progress())
+            self.send_lineno(self.anim.timeline.get_lineno_at_time(time))
+
     def on_select_triggered(self) -> None:
         if self.selector is None:
             self.selector = Selector(self)
             self.selector.destroyed.connect(self.on_selector_destroyed)
         else:
             self.selector.clear()
```

### Comparing `janim-1.2.1/janim/gui/audio_player.py` & `janim-1.2.2/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/export.png` & `janim-1.2.2/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/favicon.ico` & `janim-1.2.2/janim/gui/favicon.ico`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/fixed_ratio_widget.py` & `janim-1.2.2/janim/gui/fixed_ratio_widget.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/font_table.py` & `janim-1.2.2/janim/gui/font_table.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/glwidget.py` & `janim-1.2.2/janim/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/precise_timer.py` & `janim-1.2.2/janim/gui/precise_timer.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/richtext_editor.py` & `janim-1.2.2/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/search.png` & `janim-1.2.2/janim/gui/search.png`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/selector.py` & `janim-1.2.2/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/gui/timeline_view.py` & `janim-1.2.2/janim/gui/timeline_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,16 +178,16 @@
                                       QValueAxis)
 
         audio = info.audio
 
         clip_begin = info.clip_range.at
         clip_end = info.clip_range.end
         if near is not None:
-            clip_begin = max(clip_begin, near - info.range.at - 4)
-            clip_end = min(clip_end, near - info.range.at + 4)
+            clip_begin = max(clip_begin, near - info.range.at + info.clip_range.at - 4)
+            clip_end = min(clip_end, near - info.range.at + info.clip_range.at + 4)
 
         range_begin = info.range.at + (clip_begin - info.clip_range.at)
         range_end = range_begin + (clip_end - clip_begin)
 
         begin = int(clip_begin * audio.framerate)
         end = int(clip_end * audio.framerate)
 
@@ -589,14 +589,15 @@
         p.setRenderHint(QPainter.RenderHint.Antialiasing, True)
         self.paint_line(p, self.progress_to_time(self._progress))
         p.setRenderHint(QPainter.RenderHint.Antialiasing, False)
 
         # 绘制视野区域指示（底部的长条）
         left = self.range.at / self.anim.global_range.duration * self.width()
         width = self.range.duration / self.anim.global_range.duration * self.width()
+        width = max(width, self.range_tip_height)
         p.setPen(Qt.PenStyle.NoPen)
         p.setBrush(QColor(77, 102, 132))
         p.drawRoundedRect(
             left,
             self.height() - self.range_tip_height,
             width,
             self.range_tip_height,
```

### Comparing `janim-1.2.1/janim/imports.py` & `janim-1.2.2/janim/imports.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/audio.py` & `janim-1.2.2/janim/items/audio.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/boolean_ops.py` & `janim-1.2.2/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/coordinate/coordinate_systems.py` & `janim-1.2.2/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/coordinate/functions.py` & `janim-1.2.2/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/coordinate/number_line.py` & `janim-1.2.2/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/geometry/arc.py` & `janim-1.2.2/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/geometry/arrow.py` & `janim-1.2.2/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/geometry/line.py` & `janim-1.2.2/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/geometry/polygon.py` & `janim-1.2.2/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/image_item.py` & `janim-1.2.2/janim/items/image_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/item.py` & `janim-1.2.2/janim/items/item.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/points.py` & `janim-1.2.2/janim/items/points.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/relation.py` & `janim-1.2.2/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/shape_matchers.py` & `janim-1.2.2/janim/items/shape_matchers.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/svg/brace.py` & `janim-1.2.2/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/svg/brace.svg` & `janim-1.2.2/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/svg/svg_item.py` & `janim-1.2.2/janim/items/svg/svg_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/svg/typst.py` & `janim-1.2.2/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/text/text.py` & `janim-1.2.2/janim/items/text/text.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/value_tracker.py` & `janim-1.2.2/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/items/vitem.py` & `janim-1.2.2/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/render/base.py` & `janim-1.2.2/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/render/impl.py` & `janim-1.2.2/janim/render/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,18 +108,20 @@
         is_camera_changed = id(new_camera_info) != id(self.prev_camera_info)
 
         if new_fix_in_frame != self.prev_fix_in_frame \
                 or id(new_radius) != id(self.prev_radius) \
                 or id(new_points) != id(self.prev_points) \
                 or is_camera_changed:
             if new_fix_in_frame:
-                clip_box = np.array(item.points.self_box.get_corners())[:, :2]
+                clip_box = render_data.camera_info.map_fixed_in_frame_points(
+                    np.array(item.points.self_box.get_corners())
+                )
             else:
                 clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
-                clip_box *= render_data.camera_info.frame_radius
+            clip_box *= render_data.camera_info.frame_radius
 
             buff = new_radius.max() + render_data.anti_alias_radius
             clip_min = np.min(clip_box, axis=0) - buff
             clip_max = np.max(clip_box, axis=0) + buff
             clip_box = np.array([
                 clip_min,
                 [clip_min[0], clip_max[1]],
@@ -162,18 +164,18 @@
             self.vbo_fill_color.write(bytes)
             self.prev_fill = new_fill
 
         if id(new_points) != id(self.prev_points) \
                 or new_fix_in_frame != self.prev_fix_in_frame \
                 or is_camera_changed:
             if new_fix_in_frame:
-                mapped = new_points[:, :2]
+                mapped = render_data.camera_info.map_fixed_in_frame_points(new_points)
             else:
                 mapped = render_data.camera_info.map_points(new_points)
-                mapped *= render_data.camera_info.frame_radius
+            mapped *= render_data.camera_info.frame_radius
 
             bytes = np.hstack([
                 mapped,
                 item.points.get_closepath_flags()[:, np.newaxis],
                 np.zeros((len(mapped), 1))
             ]).astype('f4').tobytes()
```

### Comparing `janim-1.2.1/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.2.2/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/render/shaders/image.vert.glsl` & `janim-1.2.2/janim/render/shaders/image.vert.glsl`

 * *Files 24% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 in vec2 in_texcoord;
 
 out vec4 v_color;
 out vec2 v_texcoord;
 
 uniform bool JA_FIX_IN_FRAME;
 uniform mat4 JA_VIEW_MATRIX;
-uniform float JA_DISTANCE_FROM_PLANE;
+uniform float JA_FIXED_DIST_FROM_PLANE;
 uniform mat4 JA_PROJ_MATRIX;
 
 void main()
 {
 	if (JA_FIX_IN_FRAME) {
-		gl_Position = JA_PROJ_MATRIX * vec4(in_point - vec3(0.0, 0.0, JA_DISTANCE_FROM_PLANE), 1.0);
+		gl_Position = JA_PROJ_MATRIX * vec4(in_point - vec3(0.0, 0.0, JA_FIXED_DIST_FROM_PLANE), 1.0);
 	} else {
 		gl_Position = JA_PROJ_MATRIX * JA_VIEW_MATRIX * vec4(in_point, 1.0);
 	}
 	gl_Position.z *= 0.1;
 	v_color = in_color;
 	v_texcoord = in_texcoord;
 }
```

### Comparing `janim-1.2.1/janim/render/shaders/vitem.frag.glsl` & `janim-1.2.2/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/render/texture.py` & `janim-1.2.2/janim/render/texture.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/render/writer.py` & `janim-1.2.2/janim/render/writer.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/typing.py` & `janim-1.2.2/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/bezier.py` & `janim-1.2.2/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/config.py` & `janim-1.2.2/janim/utils/config.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/data.py` & `janim-1.2.2/janim/utils/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/dict_ops.py` & `janim-1.2.2/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/file_ops.py` & `janim-1.2.2/janim/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/font.py` & `janim-1.2.2/janim/utils/font.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/font_manager.py` & `janim-1.2.2/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/iterables.py` & `janim-1.2.2/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/paths.py` & `janim-1.2.2/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/rate_functions.py` & `janim-1.2.2/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/refresh.py` & `janim-1.2.2/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/signal.py` & `janim-1.2.2/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/simple_functions.py` & `janim-1.2.2/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/janim/utils/space_ops.py` & `janim-1.2.2/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/logo.png` & `janim-1.2.2/logo.png`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/pyproject.toml` & `janim-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janim-1.2.1/PKG-INFO` & `janim-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 1.2.1
+Version: 1.2.2
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: janim Version: 1.2.1 Summary: a library for simple
+Metadata-Version: 2.1 Name: janim Version: 1.2.2 Summary: a library for simple
 animation effects Author: jkjkil4 Requires-Python: >=3.12 Description-Content-
 Type: text/markdown Classifier: Programming Language :: Python Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: colour Requires-Dist: rich Requires-
 Dist: moderngl Requires-Dist: tqdm Requires-Dist: psutil Requires-Dist: skia-
 pathops Requires-Dist: fontTools Requires-Dist: freetype-py Requires-Dist:
 pillow Requires-Dist: svgelements Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc" Requires-Dist: furo ; extra
```

