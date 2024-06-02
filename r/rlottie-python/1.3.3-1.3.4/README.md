# Comparing `tmp/rlottie_python-1.3.3.tar.gz` & `tmp/rlottie_python-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlottie_python-1.3.3.tar", last modified: Sat Mar  9 10:42:54 2024, max compression
+gzip compressed data, was "rlottie_python-1.3.4.tar", last modified: Thu Mar 21 14:25:40 2024, max compression
```

## Comparing `rlottie_python-1.3.3.tar` & `rlottie_python-1.3.4.tar`

### file list

```diff
@@ -1,332 +1,332 @@
--rw-r--r--   0        0        0      738 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/CMakeLists.txt
--rw-r--r--   0        0        0    26526 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/LICENSE
--rw-r--r--   0        0        0     4331 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/README.md
--rw-r--r--   0        0        0     1696 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/pyproject.toml
--rwxr-xr-x   0        0        0  1547163 2024-03-09 10:42:50.455734 rlottie_python-1.3.3/rlottie/.Gifs/1.gif
--rwxr-xr-x   0        0        0   868128 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.Gifs/2.gif
--rw-r--r--   0        0        0    11173 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.Gifs/logo.png
--rw-r--r--   0        0        0    87552 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.Gifs/rlottie.xcf
--rw-r--r--   0        0        0    17344 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.Gifs/rlottie_player.png
--rw-r--r--   0        0        0      616 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.appveyor.yml
--rw-r--r--   0        0        0     2592 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.clang-format
--rw-r--r--   0        0        0       32 2024-03-09 10:42:49.975730 rlottie_python-1.3.3/rlottie/.git
--rw-r--r--   0        0        0      116 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.gitignore
--rw-r--r--   0        0        0     1217 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/.travis.yml
--rw-r--r--   0        0        0      709 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/AUTHORS
--rw-r--r--   0        0        0     6246 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/CMakeLists.txt
--rw-r--r--   0        0        0      690 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/COPYING
--rw-r--r--   0        0        0    10977 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/README.md
--rwxr-xr-x   0        0        0      317 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/arm_build.sh
--rw-r--r--   0        0        0      320 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/arm_cross.txt
--rw-r--r--   0        0        0      322 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/cmake/config.h.in
--rw-r--r--   0        0        0      546 2024-03-09 10:42:50.459734 rlottie_python-1.3.3/rlottie/cmake/rlottieConfig.cmake.in
--rw-r--r--   0        0        0      474 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/CMakeLists.txt
--rw-r--r--   0        0        0     9226 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/demo.cpp
--rw-r--r--   0        0        0     2650 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/demo_marker.cpp
--rw-r--r--   0        0        0     4192 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/evasapp.cpp
--rw-r--r--   0        0        0     2957 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/evasapp.h
--rw-r--r--   0        0        0    27371 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/gif.h
--rw-r--r--   0        0        0     4908 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottie2gif.cpp
--rw-r--r--   0        0        0     4938 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottieperf.cpp
--rw-r--r--   0        0        0     5676 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottieview.cpp
--rw-r--r--   0        0        0    14747 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottieview.h
--rw-r--r--   0        0        0     7405 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottieviewer.cpp
--rw-r--r--   0        0        0     5437 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/lottieviewtest.cpp
--rw-r--r--   0        0        0     2107 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/meson.build
--rw-r--r--   0        0        0     3620 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/pathtest.cpp
--rw-r--r--   0        0        0    27806 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/1643-exploding-star.json
--rw-r--r--   0        0        0    11654 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/1667-firework.json
--rw-r--r--   0        0        0    12746 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/1st_animation.lottie
--rw-r--r--   0        0        0    43105 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json
--rw-r--r--   0        0        0   154297 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/29056-nepenthe-illustration.json
--rw-r--r--   0        0        0    10221 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/360º_degree.json
--rw-r--r--   0        0        0     2536 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/3d.json
--rw-r--r--   0        0        0    19081 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/4479-fireworks.json
--rw-r--r--   0        0        0     9299 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/5317-fireworkds.json
--rw-r--r--   0        0        0   138526 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/5344-honey-sack-hud.json
--rw-r--r--   0        0        0    16809 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/Indicators1.json
--rw-r--r--   0        0        0    16155 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json
--rw-r--r--   0        0        0     5361 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/StickAndBall.json
--rw-r--r--   0        0        0    54592 2024-03-09 10:42:50.463734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json
--rw-r--r--   0        0        0    40558 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json
--rw-r--r--   0        0        0    52068 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json
--rw-r--r--   0        0        0    53471 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json
--rw-r--r--   0        0        0   246148 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json
--rw-r--r--   0        0        0    48292 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json
--rw-r--r--   0        0        0    35702 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json
--rw-r--r--   0        0        0     6341 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/_alarm.json
--rw-r--r--   0        0        0     9845 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/a_cup_of_coffee.json
--rw-r--r--   0        0        0    34000 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/a_mountain.json
--rw-r--r--   0        0        0     2248 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/abstract_circle.json
--rw-r--r--   0        0        0    76171 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/acrobatics.json
--rw-r--r--   0        0        0    42273 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/anubis.json
--rw-r--r--   0        0        0     2643 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/ao.json
--rw-r--r--   0        0        0    32268 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/balloons_with_string.json
--rw-r--r--   0        0        0     5107 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/bell.json
--rw-r--r--   0        0        0     4382 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/birth_stone_logo.json
--rw-r--r--   0        0        0     8543 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/bounching_ball.json
--rw-r--r--   0        0        0    14809 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/browser.json
--rw-r--r--   0        0        0    30454 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/confetti.json
--rw-r--r--   0        0        0    14323 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/cooking.json
--rw-r--r--   0        0        0    18611 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/dna.json
--rw-r--r--   0        0        0     3790 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/done.json
--rw-r--r--   0        0        0     2352 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/dynamic_path_test.json
--rw-r--r--   0        0        0    13891 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/dynamic_property.json
--rw-r--r--   0        0        0    30573 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/eid_mubarak.json
--rw-r--r--   0        0        0    18230 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/emoji_shock.json
--rw-r--r--   0        0        0     8800 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/emoji_wink.json
--rw-r--r--   0        0        0    11372 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/file_transfer.json
--rw-r--r--   0        0        0    34388 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/fingerprint_success.json
--rw-r--r--   0        0        0    86448 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/funky_chicken.json
--rw-r--r--   0        0        0     9040 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/gears.json
--rw-r--r--   0        0        0    10251 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/gears_or_settings.json
--rw-r--r--   0        0        0    15143 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/glow_loading.json
--rw-r--r--   0        0        0     4056 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/gradient_animated_background.json
--rw-r--r--   0        0        0     4531 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/gradient_sleepy_loader.json
--rw-r--r--   0        0        0    10981 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/happy.json
--rw-r--r--   0        0        0    11403 2024-03-09 10:42:50.467734 rlottie_python-1.3.3/rlottie/example/resource/heart.json
--rw-r--r--   0        0        0    16888 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/hourglass.json
--rw-r--r--   0        0        0   142760 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/image_embedded.json
--rw-r--r--   0        0        0      815 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/image_test.json
--rw-r--r--   0        0        0   101560 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/images/img_0.png
--rw-r--r--   0        0        0    28898 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/imprint.json
--rw-r--r--   0        0        0    62909 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/insta_camera.json
--rw-r--r--   0        0        0    57591 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/intelia_logo_animation.json
--rw-r--r--   0        0        0    10119 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/it's_lunch_time!.json
--rw-r--r--   0        0        0    76453 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/jolly_walker.json
--rw-r--r--   0        0        0     2531 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/layout.edc
--rw-r--r--   0        0        0     9106 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/layout.edj
--rw-r--r--   0        0        0    12532 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/leap_frog_loader.json
--rw-r--r--   0        0        0     8074 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/like.json
--rw-r--r--   0        0        0    13208 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loader.json
--rw-r--r--   0        0        0     3337 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loader_4.json
--rw-r--r--   0        0        0    27260 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loader_animation.json
--rw-r--r--   0        0        0   526177 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loading.json
--rw-r--r--   0        0        0     5306 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loading_.json
--rw-r--r--   0        0        0     7512 2024-03-09 10:42:50.471734 rlottie_python-1.3.3/rlottie/example/resource/loading_animation.json
--rw-r--r--   0        0        0    22205 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/loading_rectangles.json
--rw-r--r--   0        0        0    57073 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json
--rw-r--r--   0        0        0    36565 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/maps.json
--rw-r--r--   0        0        0    32154 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/marker.json
--rw-r--r--   0        0        0      933 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/mask.json
--rw-r--r--   0        0        0     5944 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/material_wave_loading.json
--rw-r--r--   0        0        0     3847 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/matte_two_item_with_lowerlayer.json
--rw-r--r--   0        0        0    20602 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/mnemonics.json
--rw-r--r--   0        0        0    10147 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/movie_loading.json
--rw-r--r--   0        0        0   103828 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/mughead.json
--rw-r--r--   0        0        0    56069 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/night_own.json
--rw-r--r--   0        0        0    33525 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/ondas.json
--rw-r--r--   0        0        0    42417 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/party_penguin.json
--rw-r--r--   0        0        0   105667 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/peli-canon.json
--rw-r--r--   0        0        0    78362 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/personal_character.json
--rw-r--r--   0        0        0     1808 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/polystar_anim.json
--rw-r--r--   0        0        0     1849 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/polystar_line_clockwise_trim.json
--rw-r--r--   0        0        0   248836 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/pumped_up.json
--rw-r--r--   0        0        0    13581 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/red_box.json
--rw-r--r--   0        0        0     9020 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/ripple_loading_animation.json
--rw-r--r--   0        0        0    12681 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/settings.json
--rw-r--r--   0        0        0    10510 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/spin,_lil_loader_v2.json
--rw-r--r--   0        0        0    28044 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/square_wheel.json
--rw-r--r--   0        0        0   180889 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/starts_transparent.json
--rw-r--r--   0        0        0     2859 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/static_dynamic_dash.json
--rw-r--r--   0        0        0     9738 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/telegram.json
--rw-r--r--   0        0        0     2192 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/test/repro_infinite_loop.json
--rw-r--r--   0        0        0     7283 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json
--rw-r--r--   0        0        0     7278 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json
--rw-r--r--   0        0        0     4427 2024-03-09 10:42:50.475735 rlottie_python-1.3.3/rlottie/example/resource/test/repro_sbof.json
--rw-r--r--   0        0        0   197687 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json
--rw-r--r--   0        0        0    49302 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/tile_grid_loading_animation.json
--rw-r--r--   0        0        0   348342 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/tractor.json
--rw-r--r--   0        0        0     8099 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/triib_manage.json
--rw-r--r--   0        0        0     7755 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/waves_.json
--rw-r--r--   0        0        0    27850 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/windmill.json
--rw-r--r--   0        0        0    70089 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/world_locations.json
--rw-r--r--   0        0        0    24031 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/worm.json
--rw-r--r--   0        0        0   202304 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/resource/you're_in!.json
--rw-r--r--   0        0        0     3952 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/uxsampletest.cpp
--rw-r--r--   0        0        0     1176 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/win32Player/Source.cpp
--rw-r--r--   0        0        0      320 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/win32Player/animation.h
--rw-r--r--   0        0        0      380 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/win32Player/framework.h
--rw-r--r--   0        0        0     1508 2024-03-09 10:42:50.479735 rlottie_python-1.3.3/rlottie/example/win32Player/resource.h
--rw-r--r--   0        0        0  2035712 2024-03-09 10:42:50.487735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottie.dll
--rw-r--r--   0        0        0    27826 2024-03-09 10:42:50.487735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottie.lib
--rw-r--r--   0        0        0    15904 2024-03-09 10:42:50.487735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.cpp
--rw-r--r--   0        0        0   244224 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.exe
--rw-r--r--   0        0        0      710 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.h
--rw-r--r--   0        0        0    46227 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.ico
--rw-r--r--   0        0        0     7298 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.rc
--rw-r--r--   0        0        0     1415 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.sln
--rw-r--r--   0        0        0     8120 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.vcxproj
--rw-r--r--   0        0        0     1884 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters
--rw-r--r--   0        0        0      165 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.user
--rw-r--r--   0        0        0    46227 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/small.ico
--rw-r--r--   0        0        0      307 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/example/win32Player/targetver.h
--rwxr-xr-x   0        0        0       56 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/format
--rw-r--r--   0        0        0       89 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/inc/CMakeLists.txt
--rw-r--r--   0        0        0      138 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/inc/meson.build
--rw-r--r--   0        0        0    17630 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/inc/rlottie.h
--rw-r--r--   0        0        0    11630 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/inc/rlottie_capi.h
--rw-r--r--   0        0        0     5193 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/inc/rlottiecommon.h
--rw-r--r--   0        0        0     6718 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.FTL
--rw-r--r--   0        0        0     1053 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.MIT
--rw-r--r--   0        0        0    16726 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.MPL
--rw-r--r--   0        0        0     2086 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.PIX
--rw-r--r--   0        0        0     5152 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.RPD
--rw-r--r--   0        0        0     1507 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.SKIA
--rw-r--r--   0        0        0     1073 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/licenses/COPYING.STB
--rw-r--r--   0        0        0     2984 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/meson.build
--rw-r--r--   0        0        0      920 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/meson_options.txt
--rw-r--r--   0        0        0       69 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/packaging/rlottie.manifest
--rw-r--r--   0        0        0     3024 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/packaging/rlottie.spec
--rw-r--r--   0        0        0      141 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/rlottie.expmap
--rw-r--r--   0        0        0      127 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/rlottie.pc.in
--rw-r--r--   0        0        0       79 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/CMakeLists.txt
--rw-r--r--   0        0        0       20 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/binding/CMakeLists.txt
--rw-r--r--   0        0        0      192 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/binding/c/CMakeLists.txt
--rw-r--r--   0        0        0    10348 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/binding/c/lottieanimation_capi.cpp
--rw-r--r--   0        0        0      267 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/binding/c/meson.build
--rw-r--r--   0        0        0       40 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/binding/meson.build
--rw-r--r--   0        0        0      586 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/CMakeLists.txt
--rw-r--r--   0        0        0    14622 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/lottieanimation.cpp
--rw-r--r--   0        0        0    12847 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/lottiefiltermodel.h
--rw-r--r--   0        0        0    46032 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/lottieitem.cpp
--rw-r--r--   0        0        0    19984 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/lottieitem.h
--rw-r--r--   0        0        0    11381 2024-03-09 10:42:50.495735 rlottie_python-1.3.3/rlottie/src/lottie/lottieitem_capi.cpp
--rw-r--r--   0        0        0     2216 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottiekeypath.cpp
--rw-r--r--   0        0        0     2097 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottiekeypath.h
--rw-r--r--   0        0        0     5145 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottieloader.cpp
--rw-r--r--   0        0        0    12452 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottiemodel.cpp
--rw-r--r--   0        0        0    35956 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottiemodel.h
--rw-r--r--   0        0        0    72932 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottieparser.cpp
--rw-r--r--   0        0        0        0 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/lottieproxymodel.cpp
--rw-r--r--   0        0        0      437 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/meson.build
--rw-r--r--   0        0        0    10695 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/allocators.h
--rw-r--r--   0        0        0     2281 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h
--rw-r--r--   0        0        0   121069 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/document.h
--rw-r--r--   0        0        0    10681 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/encodedstream.h
--rw-r--r--   0        0        0    29281 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/encodings.h
--rw-r--r--   0        0        0     3870 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/error/en.h
--rw-r--r--   0        0        0     6213 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/error/error.h
--rw-r--r--   0        0        0     3001 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/filereadstream.h
--rw-r--r--   0        0        0     3146 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/filewritestream.h
--rw-r--r--   0        0        0     4034 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/fwd.h
--rw-r--r--   0        0        0     9143 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/biginteger.h
--rw-r--r--   0        0        0     2066 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/clzll.h
--rw-r--r--   0        0        0    11509 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/diyfp.h
--rw-r--r--   0        0        0     8125 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/dtoa.h
--rw-r--r--   0        0        0     2994 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/ieee754.h
--rw-r--r--   0        0        0    10131 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/itoa.h
--rw-r--r--   0        0        0     6641 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/meta.h
--rw-r--r--   0        0        0     3595 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/pow10.h
--rw-r--r--   0        0        0    26141 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/regex.h
--rw-r--r--   0        0        0     7184 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/stack.h
--rw-r--r--   0        0        0     2199 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/strfunc.h
--rw-r--r--   0        0        0     8994 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/strtod.h
--rw-r--r--   0        0        0     1419 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/swap.h
--rw-r--r--   0        0        0     4082 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/istreamwrapper.h
--rw-r--r--   0        0        0     2560 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/memorybuffer.h
--rw-r--r--   0        0        0     2667 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/memorystream.h
--rw-r--r--   0        0        0     8372 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h
--rw-r--r--   0        0        0     9386 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/msinttypes/stdint.h
--rw-r--r--   0        0        0     2331 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/ostreamwrapper.h
--rw-r--r--   0        0        0    60889 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/pointer.h
--rw-r--r--   0        0        0    10539 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/prettywriter.h
--rw-r--r--   0        0        0    24161 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/rapidjson.h
--rw-r--r--   0        0        0    93838 2024-03-09 10:42:50.499735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/reader.h
--rw-r--r--   0        0        0   103633 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/schema.h
--rw-r--r--   0        0        0     6753 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/stream.h
--rw-r--r--   0        0        0     3993 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/stringbuffer.h
--rw-r--r--   0        0        0    26877 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/writer.h
--rw-r--r--   0        0        0      175 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/zip/CMakeLists.txt
--rw-r--r--   0        0        0      146 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/zip/meson.build
--rw-r--r--   0        0        0   395893 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/zip/miniz.h
--rw-r--r--   0        0        0    12561 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/zip/zip.cpp
--rw-r--r--   0        0        0     5010 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/lottie/zip/zip.h
--rw-r--r--   0        0        0     1871 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/meson.build
--rw-r--r--   0        0        0     1267 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/CMakeLists.txt
--rw-r--r--   0        0        0      286 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/CMakeLists.txt
--rw-r--r--   0        0        0      304 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/meson.build
--rw-r--r--   0        0        0    12132 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_math.cpp
--rw-r--r--   0        0        0    14680 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_math.h
--rw-r--r--   0        0        0    46945 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_raster.cpp
--rw-r--r--   0        0        0    39675 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_raster.h
--rw-r--r--   0        0        0    62535 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_stroker.cpp
--rw-r--r--   0        0        0    10128 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_stroker.h
--rw-r--r--   0        0        0     8325 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_types.h
--rw-r--r--   0        0        0      801 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/meson.build
--rw-r--r--   0        0        0      306 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/pixman/CMakeLists.txt
--rw-r--r--   0        0        0      310 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/pixman/meson.build
--rw-r--r--   0        0        0    19930 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.S
--rw-r--r--   0        0        0    37637 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.h
--rw-r--r--   0        0        0     1036 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/stb/CMakeLists.txt
--rw-r--r--   0        0        0     1028 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/stb/meson.build
--rw-r--r--   0        0        0     1355 2024-03-09 10:42:50.503735 rlottie_python-1.3.3/rlottie/src/vector/stb/stb_image.cpp
--rw-r--r--   0        0        0   261660 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/stb/stb_image.h
--rw-r--r--   0        0        0     5584 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/varenaalloc.cpp
--rw-r--r--   0        0        0     8807 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/varenaalloc.h
--rw-r--r--   0        0        0     3658 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbezier.cpp
--rw-r--r--   0        0        0     4584 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbezier.h
--rw-r--r--   0        0        0     5772 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbitmap.cpp
--rw-r--r--   0        0        0     3630 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbitmap.h
--rw-r--r--   0        0        0     2168 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbrush.cpp
--rw-r--r--   0        0        0     2981 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vbrush.h
--rw-r--r--   0        0        0     3215 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vcowptr.h
--rw-r--r--   0        0        0     7123 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdasher.cpp
--rw-r--r--   0        0        0     2352 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdasher.h
--rw-r--r--   0        0        0    22094 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdebug.cpp
--rw-r--r--   0        0        0     5749 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdebug.h
--rw-r--r--   0        0        0     3895 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawable.cpp
--rw-r--r--   0        0        0     3014 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawable.h
--rw-r--r--   0        0        0    25053 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper.cpp
--rw-r--r--   0        0        0     7837 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper.h
--rw-r--r--   0        0        0     5615 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_common.cpp
--rw-r--r--   0        0        0      615 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_neon.cpp
--rw-r--r--   0        0        0     8117 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_sse2.cpp
--rw-r--r--   0        0        0     1749 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/velapsedtimer.cpp
--rw-r--r--   0        0        0     1615 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/velapsedtimer.h
--rw-r--r--   0        0        0     8411 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vglobal.h
--rw-r--r--   0        0        0     6375 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vimageloader.cpp
--rw-r--r--   0        0        0      450 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vimageloader.h
--rw-r--r--   0        0        0     3730 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vinterpolator.cpp
--rw-r--r--   0        0        0     2680 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vinterpolator.h
--rw-r--r--   0        0        0     2996 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vline.h
--rw-r--r--   0        0        0    18367 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vmatrix.cpp
--rw-r--r--   0        0        0     4041 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vmatrix.h
--rw-r--r--   0        0        0     4841 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpainter.cpp
--rw-r--r--   0        0        0     2422 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpainter.h
--rw-r--r--   0        0        0    22546 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpath.cpp
--rw-r--r--   0        0        0     9067 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpath.h
--rw-r--r--   0        0        0     2413 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpathmesure.cpp
--rw-r--r--   0        0        0     1586 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpathmesure.h
--rw-r--r--   0        0        0     6289 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vpoint.h
--rw-r--r--   0        0        0    15316 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vraster.cpp
--rw-r--r--   0        0        0     1746 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vraster.h
--rw-r--r--   0        0        0     1955 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vrect.cpp
--rw-r--r--   0        0        0     5642 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vrect.h
--rw-r--r--   0        0        0    20545 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vrle.cpp
--rw-r--r--   0        0        0     4252 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vrle.h
--rw-r--r--   0        0        0     2396 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vsharedptr.h
--rw-r--r--   0        0        0     5031 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vstackallocator.h
--rw-r--r--   0        0        0     2494 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/vector/vtaskqueue.h
--rw-r--r--   0        0        0      236 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/wasm/meson.build
--rw-r--r--   0        0        0    55577 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/src/wasm/rlottiewasm.cpp
--rw-r--r--   0        0        0      904 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/CMakeLists.txt
--rw-r--r--   0        0        0     1113 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/meson.build
--rw-r--r--   0        0        0      822 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/test_lottieanimation.cpp
--rw-r--r--   0        0        0      889 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/test_lottieanimation_capi.cpp
--rw-r--r--   0        0        0     7171 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/test_vpath.cpp
--rw-r--r--   0        0        0     1149 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/test_vrect.cpp
--rw-r--r--   0        0        0      132 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/testsuite.cpp
--rw-r--r--   0        0        0     1131 2024-03-09 10:42:50.507735 rlottie_python-1.3.3/rlottie/test/wasm_test.html
--rw-r--r--   0        0        0      173 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/vs2019/config.h
--rw-r--r--   0        0        0     1434 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/vs2019/rlottie.sln
--rw-r--r--   0        0        0    13672 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/vs2019/rlottie.vcxproj
--rw-r--r--   0        0        0    15217 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/vs2019/rlottie.vcxproj.filters
--rw-r--r--   0        0        0      168 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/vs2019/rlottie.vcxproj.user
--rwxr-xr-x   0        0        0      625 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/wasm_build.sh
--rw-r--r--   0        0        0      588 2024-03-09 10:42:50.511735 rlottie_python-1.3.3/rlottie/wasm_cross.txt
--rwxr-xr-x   0        0        0      142 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/rlottie_python/__init__.py
--rwxr-xr-x   0        0        0     3917 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/rlottie_python/_rlottiecommon.py
--rw-r--r--   0        0        0        0 2024-03-09 10:42:49.395725 rlottie_python-1.3.3/rlottie_python/py.typed
--rwxr-xr-x   0        0        0    29089 2024-03-09 10:42:49.399725 rlottie_python-1.3.3/rlottie_python/rlottie_wrapper.py
--rw-r--r--   0        0        0    35453 1970-01-01 00:00:00.000000 rlottie_python-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0      738 2024-03-21 14:25:36.226340 rlottie_python-1.3.4/CMakeLists.txt
+-rw-r--r--   0        0        0    26526 2024-03-21 14:25:36.226340 rlottie_python-1.3.4/LICENSE
+-rw-r--r--   0        0        0     4292 2024-03-21 14:25:36.226340 rlottie_python-1.3.4/README.md
+-rw-r--r--   0        0        0     1828 2024-03-21 14:25:36.226340 rlottie_python-1.3.4/pyproject.toml
+-rwxr-xr-x   0        0        0  1547163 2024-03-21 14:25:37.610343 rlottie_python-1.3.4/rlottie/.Gifs/1.gif
+-rwxr-xr-x   0        0        0   868128 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.Gifs/2.gif
+-rw-r--r--   0        0        0    11173 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.Gifs/logo.png
+-rw-r--r--   0        0        0    87552 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.Gifs/rlottie.xcf
+-rw-r--r--   0        0        0    17344 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.Gifs/rlottie_player.png
+-rw-r--r--   0        0        0      616 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.appveyor.yml
+-rw-r--r--   0        0        0     2592 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.clang-format
+-rw-r--r--   0        0        0       32 2024-03-21 14:25:36.962342 rlottie_python-1.3.4/rlottie/.git
+-rw-r--r--   0        0        0      116 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.gitignore
+-rw-r--r--   0        0        0     1217 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/.travis.yml
+-rw-r--r--   0        0        0      709 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/AUTHORS
+-rw-r--r--   0        0        0     6246 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/CMakeLists.txt
+-rw-r--r--   0        0        0      690 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/COPYING
+-rw-r--r--   0        0        0    10977 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/README.md
+-rwxr-xr-x   0        0        0      317 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/arm_build.sh
+-rw-r--r--   0        0        0      320 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/arm_cross.txt
+-rw-r--r--   0        0        0      322 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/cmake/config.h.in
+-rw-r--r--   0        0        0      546 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/cmake/rlottieConfig.cmake.in
+-rw-r--r--   0        0        0      474 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/CMakeLists.txt
+-rw-r--r--   0        0        0     9226 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/demo.cpp
+-rw-r--r--   0        0        0     2650 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/demo_marker.cpp
+-rw-r--r--   0        0        0     4192 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/evasapp.cpp
+-rw-r--r--   0        0        0     2957 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/evasapp.h
+-rw-r--r--   0        0        0    27371 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/gif.h
+-rw-r--r--   0        0        0     4908 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottie2gif.cpp
+-rw-r--r--   0        0        0     4938 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottieperf.cpp
+-rw-r--r--   0        0        0     5676 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottieview.cpp
+-rw-r--r--   0        0        0    14747 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottieview.h
+-rw-r--r--   0        0        0     7405 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottieviewer.cpp
+-rw-r--r--   0        0        0     5437 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/lottieviewtest.cpp
+-rw-r--r--   0        0        0     2107 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/meson.build
+-rw-r--r--   0        0        0     3620 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/pathtest.cpp
+-rw-r--r--   0        0        0    27806 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/resource/1643-exploding-star.json
+-rw-r--r--   0        0        0    11654 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/resource/1667-firework.json
+-rw-r--r--   0        0        0    12746 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/resource/1st_animation.lottie
+-rw-r--r--   0        0        0    43105 2024-03-21 14:25:37.618343 rlottie_python-1.3.4/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json
+-rw-r--r--   0        0        0   154297 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/29056-nepenthe-illustration.json
+-rw-r--r--   0        0        0    10221 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/360º_degree.json
+-rw-r--r--   0        0        0     2536 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/3d.json
+-rw-r--r--   0        0        0    19081 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/4479-fireworks.json
+-rw-r--r--   0        0        0     9299 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/5317-fireworkds.json
+-rw-r--r--   0        0        0   138526 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/5344-honey-sack-hud.json
+-rw-r--r--   0        0        0    16809 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/Indicators1.json
+-rw-r--r--   0        0        0    16155 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json
+-rw-r--r--   0        0        0     5361 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/StickAndBall.json
+-rw-r--r--   0        0        0    54592 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json
+-rw-r--r--   0        0        0    40558 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json
+-rw-r--r--   0        0        0    52068 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json
+-rw-r--r--   0        0        0    53471 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json
+-rw-r--r--   0        0        0   246148 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json
+-rw-r--r--   0        0        0    48292 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json
+-rw-r--r--   0        0        0    35702 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json
+-rw-r--r--   0        0        0     6341 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/_alarm.json
+-rw-r--r--   0        0        0     9845 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/a_cup_of_coffee.json
+-rw-r--r--   0        0        0    34000 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/a_mountain.json
+-rw-r--r--   0        0        0     2248 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/abstract_circle.json
+-rw-r--r--   0        0        0    76171 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/acrobatics.json
+-rw-r--r--   0        0        0    42273 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/anubis.json
+-rw-r--r--   0        0        0     2643 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/ao.json
+-rw-r--r--   0        0        0    32268 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/balloons_with_string.json
+-rw-r--r--   0        0        0     5107 2024-03-21 14:25:37.622343 rlottie_python-1.3.4/rlottie/example/resource/bell.json
+-rw-r--r--   0        0        0     4382 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/birth_stone_logo.json
+-rw-r--r--   0        0        0     8543 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/bounching_ball.json
+-rw-r--r--   0        0        0    14809 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/browser.json
+-rw-r--r--   0        0        0    30454 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/confetti.json
+-rw-r--r--   0        0        0    14323 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/cooking.json
+-rw-r--r--   0        0        0    18611 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/dna.json
+-rw-r--r--   0        0        0     3790 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/done.json
+-rw-r--r--   0        0        0     2352 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/dynamic_path_test.json
+-rw-r--r--   0        0        0    13891 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/dynamic_property.json
+-rw-r--r--   0        0        0    30573 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/eid_mubarak.json
+-rw-r--r--   0        0        0    18230 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/emoji_shock.json
+-rw-r--r--   0        0        0     8800 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/emoji_wink.json
+-rw-r--r--   0        0        0    11372 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/file_transfer.json
+-rw-r--r--   0        0        0    34388 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/fingerprint_success.json
+-rw-r--r--   0        0        0    86448 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/funky_chicken.json
+-rw-r--r--   0        0        0     9040 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/gears.json
+-rw-r--r--   0        0        0    10251 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/gears_or_settings.json
+-rw-r--r--   0        0        0    15143 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/glow_loading.json
+-rw-r--r--   0        0        0     4056 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/gradient_animated_background.json
+-rw-r--r--   0        0        0     4531 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/gradient_sleepy_loader.json
+-rw-r--r--   0        0        0    10981 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/happy.json
+-rw-r--r--   0        0        0    11403 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/heart.json
+-rw-r--r--   0        0        0    16888 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/hourglass.json
+-rw-r--r--   0        0        0   142760 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/image_embedded.json
+-rw-r--r--   0        0        0      815 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/image_test.json
+-rw-r--r--   0        0        0   101560 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/images/img_0.png
+-rw-r--r--   0        0        0    28898 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/imprint.json
+-rw-r--r--   0        0        0    62909 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/insta_camera.json
+-rw-r--r--   0        0        0    57591 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/intelia_logo_animation.json
+-rw-r--r--   0        0        0    10119 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/it's_lunch_time!.json
+-rw-r--r--   0        0        0    76453 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/jolly_walker.json
+-rw-r--r--   0        0        0     2531 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/layout.edc
+-rw-r--r--   0        0        0     9106 2024-03-21 14:25:37.626343 rlottie_python-1.3.4/rlottie/example/resource/layout.edj
+-rw-r--r--   0        0        0    12532 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/leap_frog_loader.json
+-rw-r--r--   0        0        0     8074 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/like.json
+-rw-r--r--   0        0        0    13208 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loader.json
+-rw-r--r--   0        0        0     3337 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loader_4.json
+-rw-r--r--   0        0        0    27260 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loader_animation.json
+-rw-r--r--   0        0        0   526177 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loading.json
+-rw-r--r--   0        0        0     5306 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loading_.json
+-rw-r--r--   0        0        0     7512 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loading_animation.json
+-rw-r--r--   0        0        0    22205 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/loading_rectangles.json
+-rw-r--r--   0        0        0    57073 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json
+-rw-r--r--   0        0        0    36565 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/maps.json
+-rw-r--r--   0        0        0    32154 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/marker.json
+-rw-r--r--   0        0        0      933 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/mask.json
+-rw-r--r--   0        0        0     5944 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/material_wave_loading.json
+-rw-r--r--   0        0        0     3847 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/matte_two_item_with_lowerlayer.json
+-rw-r--r--   0        0        0    20602 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/mnemonics.json
+-rw-r--r--   0        0        0    10147 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/movie_loading.json
+-rw-r--r--   0        0        0   103828 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/mughead.json
+-rw-r--r--   0        0        0    56069 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/night_own.json
+-rw-r--r--   0        0        0    33525 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/ondas.json
+-rw-r--r--   0        0        0    42417 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/party_penguin.json
+-rw-r--r--   0        0        0   105667 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/peli-canon.json
+-rw-r--r--   0        0        0    78362 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/personal_character.json
+-rw-r--r--   0        0        0     1808 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/polystar_anim.json
+-rw-r--r--   0        0        0     1849 2024-03-21 14:25:37.630343 rlottie_python-1.3.4/rlottie/example/resource/polystar_line_clockwise_trim.json
+-rw-r--r--   0        0        0   248836 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/pumped_up.json
+-rw-r--r--   0        0        0    13581 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/red_box.json
+-rw-r--r--   0        0        0     9020 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/ripple_loading_animation.json
+-rw-r--r--   0        0        0    12681 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/settings.json
+-rw-r--r--   0        0        0    10510 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/spin,_lil_loader_v2.json
+-rw-r--r--   0        0        0    28044 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/square_wheel.json
+-rw-r--r--   0        0        0   180889 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/starts_transparent.json
+-rw-r--r--   0        0        0     2859 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/static_dynamic_dash.json
+-rw-r--r--   0        0        0     9738 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/telegram.json
+-rw-r--r--   0        0        0     2192 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/test/repro_infinite_loop.json
+-rw-r--r--   0        0        0     7283 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json
+-rw-r--r--   0        0        0     7278 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json
+-rw-r--r--   0        0        0     4427 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/test/repro_sbof.json
+-rw-r--r--   0        0        0   197687 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json
+-rw-r--r--   0        0        0    49302 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/tile_grid_loading_animation.json
+-rw-r--r--   0        0        0   348342 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/tractor.json
+-rw-r--r--   0        0        0     8099 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/triib_manage.json
+-rw-r--r--   0        0        0     7755 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/waves_.json
+-rw-r--r--   0        0        0    27850 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/windmill.json
+-rw-r--r--   0        0        0    70089 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/world_locations.json
+-rw-r--r--   0        0        0    24031 2024-03-21 14:25:37.634343 rlottie_python-1.3.4/rlottie/example/resource/worm.json
+-rw-r--r--   0        0        0   202304 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/resource/you're_in!.json
+-rw-r--r--   0        0        0     3952 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/uxsampletest.cpp
+-rw-r--r--   0        0        0     1176 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/win32Player/Source.cpp
+-rw-r--r--   0        0        0      320 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/win32Player/animation.h
+-rw-r--r--   0        0        0      380 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/win32Player/framework.h
+-rw-r--r--   0        0        0     1508 2024-03-21 14:25:37.638343 rlottie_python-1.3.4/rlottie/example/win32Player/resource.h
+-rw-r--r--   0        0        0  2035712 2024-03-21 14:25:37.646343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottie.dll
+-rw-r--r--   0        0        0    27826 2024-03-21 14:25:37.646343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottie.lib
+-rw-r--r--   0        0        0    15904 2024-03-21 14:25:37.646343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.cpp
+-rw-r--r--   0        0        0   244224 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.exe
+-rw-r--r--   0        0        0      710 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.h
+-rw-r--r--   0        0        0    46227 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.ico
+-rw-r--r--   0        0        0     7298 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.rc
+-rw-r--r--   0        0        0     1415 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.sln
+-rw-r--r--   0        0        0     8120 2024-03-21 14:25:37.650343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.vcxproj
+-rw-r--r--   0        0        0     1884 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters
+-rw-r--r--   0        0        0      165 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.vcxproj.user
+-rw-r--r--   0        0        0    46227 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/example/win32Player/small.ico
+-rw-r--r--   0        0        0      307 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/example/win32Player/targetver.h
+-rwxr-xr-x   0        0        0       56 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/format
+-rw-r--r--   0        0        0       89 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/inc/CMakeLists.txt
+-rw-r--r--   0        0        0      138 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/inc/meson.build
+-rw-r--r--   0        0        0    17630 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/inc/rlottie.h
+-rw-r--r--   0        0        0    11630 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/inc/rlottie_capi.h
+-rw-r--r--   0        0        0     5193 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/inc/rlottiecommon.h
+-rw-r--r--   0        0        0     6718 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.FTL
+-rw-r--r--   0        0        0     1053 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.MIT
+-rw-r--r--   0        0        0    16726 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.MPL
+-rw-r--r--   0        0        0     2086 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.PIX
+-rw-r--r--   0        0        0     5152 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.RPD
+-rw-r--r--   0        0        0     1507 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.SKIA
+-rw-r--r--   0        0        0     1073 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/licenses/COPYING.STB
+-rw-r--r--   0        0        0     2984 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/meson.build
+-rw-r--r--   0        0        0      920 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/meson_options.txt
+-rw-r--r--   0        0        0       69 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/packaging/rlottie.manifest
+-rw-r--r--   0        0        0     3024 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/packaging/rlottie.spec
+-rw-r--r--   0        0        0      141 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/rlottie.expmap
+-rw-r--r--   0        0        0      127 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/rlottie.pc.in
+-rw-r--r--   0        0        0       79 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/CMakeLists.txt
+-rw-r--r--   0        0        0       20 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/binding/CMakeLists.txt
+-rw-r--r--   0        0        0      192 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/binding/c/CMakeLists.txt
+-rw-r--r--   0        0        0    10348 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/binding/c/lottieanimation_capi.cpp
+-rw-r--r--   0        0        0      267 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/binding/c/meson.build
+-rw-r--r--   0        0        0       40 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/binding/meson.build
+-rw-r--r--   0        0        0      586 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/CMakeLists.txt
+-rw-r--r--   0        0        0    14622 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieanimation.cpp
+-rw-r--r--   0        0        0    12847 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottiefiltermodel.h
+-rw-r--r--   0        0        0    46032 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieitem.cpp
+-rw-r--r--   0        0        0    19984 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieitem.h
+-rw-r--r--   0        0        0    11381 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieitem_capi.cpp
+-rw-r--r--   0        0        0     2216 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottiekeypath.cpp
+-rw-r--r--   0        0        0     2097 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottiekeypath.h
+-rw-r--r--   0        0        0     5145 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieloader.cpp
+-rw-r--r--   0        0        0    12452 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottiemodel.cpp
+-rw-r--r--   0        0        0    35956 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottiemodel.h
+-rw-r--r--   0        0        0    72932 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieparser.cpp
+-rw-r--r--   0        0        0        0 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/lottieproxymodel.cpp
+-rw-r--r--   0        0        0      437 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/meson.build
+-rw-r--r--   0        0        0    10695 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/allocators.h
+-rw-r--r--   0        0        0     2281 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h
+-rw-r--r--   0        0        0   121069 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/document.h
+-rw-r--r--   0        0        0    10681 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/encodedstream.h
+-rw-r--r--   0        0        0    29281 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/encodings.h
+-rw-r--r--   0        0        0     3870 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/error/en.h
+-rw-r--r--   0        0        0     6213 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/error/error.h
+-rw-r--r--   0        0        0     3001 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/filereadstream.h
+-rw-r--r--   0        0        0     3146 2024-03-21 14:25:37.654343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/filewritestream.h
+-rw-r--r--   0        0        0     4034 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/fwd.h
+-rw-r--r--   0        0        0     9143 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/biginteger.h
+-rw-r--r--   0        0        0     2066 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/clzll.h
+-rw-r--r--   0        0        0    11509 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/diyfp.h
+-rw-r--r--   0        0        0     8125 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/dtoa.h
+-rw-r--r--   0        0        0     2994 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/ieee754.h
+-rw-r--r--   0        0        0    10131 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/itoa.h
+-rw-r--r--   0        0        0     6641 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/meta.h
+-rw-r--r--   0        0        0     3595 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/pow10.h
+-rw-r--r--   0        0        0    26141 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/regex.h
+-rw-r--r--   0        0        0     7184 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/stack.h
+-rw-r--r--   0        0        0     2199 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/strfunc.h
+-rw-r--r--   0        0        0     8994 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/strtod.h
+-rw-r--r--   0        0        0     1419 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/swap.h
+-rw-r--r--   0        0        0     4082 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/istreamwrapper.h
+-rw-r--r--   0        0        0     2560 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/memorybuffer.h
+-rw-r--r--   0        0        0     2667 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/memorystream.h
+-rw-r--r--   0        0        0     8372 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h
+-rw-r--r--   0        0        0     9386 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/msinttypes/stdint.h
+-rw-r--r--   0        0        0     2331 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/ostreamwrapper.h
+-rw-r--r--   0        0        0    60889 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/pointer.h
+-rw-r--r--   0        0        0    10539 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/prettywriter.h
+-rw-r--r--   0        0        0    24161 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/rapidjson.h
+-rw-r--r--   0        0        0    93838 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/reader.h
+-rw-r--r--   0        0        0   103633 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/schema.h
+-rw-r--r--   0        0        0     6753 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/stream.h
+-rw-r--r--   0        0        0     3993 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/stringbuffer.h
+-rw-r--r--   0        0        0    26877 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/writer.h
+-rw-r--r--   0        0        0      175 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/zip/CMakeLists.txt
+-rw-r--r--   0        0        0      146 2024-03-21 14:25:37.658343 rlottie_python-1.3.4/rlottie/src/lottie/zip/meson.build
+-rw-r--r--   0        0        0   395893 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/lottie/zip/miniz.h
+-rw-r--r--   0        0        0    12561 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/lottie/zip/zip.cpp
+-rw-r--r--   0        0        0     5010 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/lottie/zip/zip.h
+-rw-r--r--   0        0        0     1871 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/meson.build
+-rw-r--r--   0        0        0     1267 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/CMakeLists.txt
+-rw-r--r--   0        0        0      286 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/CMakeLists.txt
+-rw-r--r--   0        0        0      304 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/meson.build
+-rw-r--r--   0        0        0    12132 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_math.cpp
+-rw-r--r--   0        0        0    14680 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_math.h
+-rw-r--r--   0        0        0    46945 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_raster.cpp
+-rw-r--r--   0        0        0    39675 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_raster.h
+-rw-r--r--   0        0        0    62535 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_stroker.cpp
+-rw-r--r--   0        0        0    10128 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_stroker.h
+-rw-r--r--   0        0        0     8325 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_types.h
+-rw-r--r--   0        0        0      801 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/meson.build
+-rw-r--r--   0        0        0      306 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/pixman/CMakeLists.txt
+-rw-r--r--   0        0        0      310 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/pixman/meson.build
+-rw-r--r--   0        0        0    19930 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/pixman/pixman-arm-neon-asm.S
+-rw-r--r--   0        0        0    37637 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/pixman/pixman-arm-neon-asm.h
+-rw-r--r--   0        0        0     1036 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/stb/CMakeLists.txt
+-rw-r--r--   0        0        0     1028 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/stb/meson.build
+-rw-r--r--   0        0        0     1355 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/stb/stb_image.cpp
+-rw-r--r--   0        0        0   261660 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/stb/stb_image.h
+-rw-r--r--   0        0        0     5584 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/varenaalloc.cpp
+-rw-r--r--   0        0        0     8807 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/varenaalloc.h
+-rw-r--r--   0        0        0     3658 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbezier.cpp
+-rw-r--r--   0        0        0     4584 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbezier.h
+-rw-r--r--   0        0        0     5772 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbitmap.cpp
+-rw-r--r--   0        0        0     3630 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbitmap.h
+-rw-r--r--   0        0        0     2168 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbrush.cpp
+-rw-r--r--   0        0        0     2981 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vbrush.h
+-rw-r--r--   0        0        0     3215 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vcowptr.h
+-rw-r--r--   0        0        0     7123 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdasher.cpp
+-rw-r--r--   0        0        0     2352 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdasher.h
+-rw-r--r--   0        0        0    22094 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdebug.cpp
+-rw-r--r--   0        0        0     5749 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdebug.h
+-rw-r--r--   0        0        0     3895 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdrawable.cpp
+-rw-r--r--   0        0        0     3014 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdrawable.h
+-rw-r--r--   0        0        0    25053 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper.cpp
+-rw-r--r--   0        0        0     7837 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper.h
+-rw-r--r--   0        0        0     5615 2024-03-21 14:25:37.662343 rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_common.cpp
+-rw-r--r--   0        0        0      615 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_neon.cpp
+-rw-r--r--   0        0        0     8117 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_sse2.cpp
+-rw-r--r--   0        0        0     1749 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/velapsedtimer.cpp
+-rw-r--r--   0        0        0     1615 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/velapsedtimer.h
+-rw-r--r--   0        0        0     8411 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vglobal.h
+-rw-r--r--   0        0        0     6375 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vimageloader.cpp
+-rw-r--r--   0        0        0      450 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vimageloader.h
+-rw-r--r--   0        0        0     3730 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vinterpolator.cpp
+-rw-r--r--   0        0        0     2680 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vinterpolator.h
+-rw-r--r--   0        0        0     2996 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vline.h
+-rw-r--r--   0        0        0    18367 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vmatrix.cpp
+-rw-r--r--   0        0        0     4041 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vmatrix.h
+-rw-r--r--   0        0        0     4841 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpainter.cpp
+-rw-r--r--   0        0        0     2422 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpainter.h
+-rw-r--r--   0        0        0    22546 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpath.cpp
+-rw-r--r--   0        0        0     9067 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpath.h
+-rw-r--r--   0        0        0     2413 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpathmesure.cpp
+-rw-r--r--   0        0        0     1586 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpathmesure.h
+-rw-r--r--   0        0        0     6289 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vpoint.h
+-rw-r--r--   0        0        0    15316 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vraster.cpp
+-rw-r--r--   0        0        0     1746 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vraster.h
+-rw-r--r--   0        0        0     1955 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vrect.cpp
+-rw-r--r--   0        0        0     5642 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vrect.h
+-rw-r--r--   0        0        0    20545 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vrle.cpp
+-rw-r--r--   0        0        0     4252 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vrle.h
+-rw-r--r--   0        0        0     2396 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vsharedptr.h
+-rw-r--r--   0        0        0     5031 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vstackallocator.h
+-rw-r--r--   0        0        0     2494 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/vector/vtaskqueue.h
+-rw-r--r--   0        0        0      236 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/wasm/meson.build
+-rw-r--r--   0        0        0    55577 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/src/wasm/rlottiewasm.cpp
+-rw-r--r--   0        0        0      904 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/CMakeLists.txt
+-rw-r--r--   0        0        0     1113 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/meson.build
+-rw-r--r--   0        0        0      822 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/test_lottieanimation.cpp
+-rw-r--r--   0        0        0      889 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/test_lottieanimation_capi.cpp
+-rw-r--r--   0        0        0     7171 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/test_vpath.cpp
+-rw-r--r--   0        0        0     1149 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/test_vrect.cpp
+-rw-r--r--   0        0        0      132 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/testsuite.cpp
+-rw-r--r--   0        0        0     1131 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/test/wasm_test.html
+-rw-r--r--   0        0        0      173 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/vs2019/config.h
+-rw-r--r--   0        0        0     1434 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/vs2019/rlottie.sln
+-rw-r--r--   0        0        0    13672 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/vs2019/rlottie.vcxproj
+-rw-r--r--   0        0        0    15217 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/vs2019/rlottie.vcxproj.filters
+-rw-r--r--   0        0        0      168 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/vs2019/rlottie.vcxproj.user
+-rwxr-xr-x   0        0        0      625 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/wasm_build.sh
+-rw-r--r--   0        0        0      588 2024-03-21 14:25:37.666343 rlottie_python-1.3.4/rlottie/wasm_cross.txt
+-rwxr-xr-x   0        0        0      142 2024-03-21 14:25:36.230340 rlottie_python-1.3.4/src/rlottie_python/__init__.py
+-rwxr-xr-x   0        0        0     3917 2024-03-21 14:25:36.230340 rlottie_python-1.3.4/src/rlottie_python/_rlottiecommon.py
+-rw-r--r--   0        0        0        0 2024-03-21 14:25:36.230340 rlottie_python-1.3.4/src/rlottie_python/py.typed
+-rwxr-xr-x   0        0        0    29089 2024-03-21 14:25:36.230340 rlottie_python-1.3.4/src/rlottie_python/rlottie_wrapper.py
+-rw-r--r--   0        0        0    35712 1970-01-01 00:00:00.000000 rlottie_python-1.3.4/PKG-INFO
```

### Comparing `rlottie_python-1.3.3/CMakeLists.txt` & `rlottie_python-1.3.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/LICENSE` & `rlottie_python-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/README.md` & `rlottie_python-1.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,48 +16,22 @@
 - [Credits](#credits)
 
 ## Installing
 
 Note that rlottie is included in the wheel package, you need not install librlottie.
 
 To install, run the following:
-```
-pip3 install wheel
+```bash
 pip3 install rlottie-python
 ```
 
-Optionally, install `Pillow`:
-```
-pip3 install Pillow
-```
-
-## Building from source
-
-To build wheel, run the following:
-```
-git clone --recursive https://github.com/laggykiller/rlottie-python.git
-cd rlottie-python
-pip3 install -r requirements.txt
-python3 -m build .
-```
-
-To install the built wheel, run `pip3 install dist/<name_of_the_wheel_file>.whl`
-
-If you want to install directly, run the following:
+`Pillow` is optional dependency. It is required for `render_pillow_frame()`,
+`save_frame()` and `save_animation()`. To also install Pillow, run:
 ```bash
-git clone --recursive https://github.com/laggykiller/rlottie-python.git
-cd rlottie-python
-pip3 install -r requirements.txt
-pip3 install .
-```
-
-To run tests:
-```bash
-pip install pytest
-pytest
+pip3 install rlottie-python[full]
 ```
 
 ## Examples
 Getting information about an lottie animation
 ```python
 from rlottie_python import LottieAnimation
 
@@ -132,10 +106,40 @@
 ```
 
 ## Comparing to other library
 The `lottie` (https://pypi.org/project/lottie/) python package is also capable of working with lottie files and telegram animated stickers (tgs). It is also able to support many input/output formats and vector graphics, without any dependency on extenral libraries such as librlottie. However some images it creates is broken ([Example1](https://github.com/laggykiller/sticker-convert/issues/5) [Example2](https://gitlab.com/mattbas/python-lottie/-/issues/95)). It seems librlottie is more stable in terms of rendering frames.
 
 The `pyrlottie` (https://pypi.org/project/pyrlottie/) python package is also able to convert lottie and tgs files to webp/gif. However, it works by calling executables `gif2webp` and `lottie2gif` with subprocess, and it does not support macOS.
 
+## Building from source
+
+To build wheel, run the following:
+```bash
+git clone --recursive https://github.com/laggykiller/rlottie-python.git
+cd rlottie-python
+
+# To build wheel
+python3 -m build .
+
+# To install directly
+pip3 install .
+```
+
+## Development
+To run tests:
+```bash
+pip install pytest
+pytest
+```
+
+To lint:
+```bash
+pip install ruff mypy isort
+mypy
+isort .
+ruff check
+ruff format
+```
+
 ## Credits
 - rlottie library: https://github.com/Samsung/rlottie
 - Packaging: https://github.com/tttapa/py-build-cmake
```

### Comparing `rlottie_python-1.3.3/pyproject.toml` & `rlottie_python-1.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,37 @@
 dynamic = ["version"]
 
 [project.urls]
 Repository = "https://github.com/laggykiller/rlottie-python"
 Documentation = "https://rlottie-python.readthedocs.io/en/latest/"
 Tracker = "https://github.com/laggykiller/rlottie-python/issues"
 
+[project.optional-dependencies]
+full = [
+    "Pillow",
+]
+
+test = [
+    "pytest"
+]
+
+lint = [
+    "ruff",
+    "mypy",
+    "isort",
+    "types-Pillow",
+]
+
 [build-system] # How pip and other frontends should build this project
 requires = ["py-build-cmake~=0.2.0a12"]
 build-backend = "py_build_cmake.build"
 
 [tool.py-build-cmake.module] # Where to find the Python module to package
 name = "rlottie_python"
-directory = "."
+directory = "src"
 
 [tool.py-build-cmake.sdist] # What to include in source distributions
 include = ["CMakeLists.txt", "rlottie/*"]
 
 [tool.py-build-cmake.cmake] # How to build the CMake project
 build_type = "Release"
 source_path = "."
@@ -41,13 +57,13 @@
 [tool.py-build-cmake.mac.cmake] # macOS-specific options
 config = "Release"
 
 [tool.py-build-cmake.windows.cmake] # Windows-specific options
 config = "Release"
 
 [tool.pyright]
-include = ["rlottie_python", "tests", "example"]
+include = ["src", "tests", "example"]
 strict = ["*"]
 
 [tool.mypy]
 python_version = "3.9"
-files = ["rlottie_python", "tests", "example"]
+files = ["src", "tests", "example"]
```

### Comparing `rlottie_python-1.3.3/rlottie/.Gifs/1.gif` & `rlottie_python-1.3.4/rlottie/.Gifs/1.gif`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.Gifs/2.gif` & `rlottie_python-1.3.4/rlottie/.Gifs/2.gif`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.Gifs/logo.png` & `rlottie_python-1.3.4/rlottie/.Gifs/logo.png`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.Gifs/rlottie.xcf` & `rlottie_python-1.3.4/rlottie/.Gifs/rlottie.xcf`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.Gifs/rlottie_player.png` & `rlottie_python-1.3.4/rlottie/.Gifs/rlottie_player.png`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.appveyor.yml` & `rlottie_python-1.3.4/rlottie/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.clang-format` & `rlottie_python-1.3.4/rlottie/.clang-format`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/.travis.yml` & `rlottie_python-1.3.4/rlottie/.travis.yml`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/AUTHORS` & `rlottie_python-1.3.4/rlottie/AUTHORS`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/CMakeLists.txt` & `rlottie_python-1.3.4/rlottie/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/COPYING` & `rlottie_python-1.3.4/rlottie/COPYING`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/README.md` & `rlottie_python-1.3.4/rlottie/README.md`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/cmake/rlottieConfig.cmake.in` & `rlottie_python-1.3.4/rlottie/cmake/rlottieConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/demo.cpp` & `rlottie_python-1.3.4/rlottie/example/demo.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/demo_marker.cpp` & `rlottie_python-1.3.4/rlottie/example/demo_marker.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/evasapp.cpp` & `rlottie_python-1.3.4/rlottie/example/evasapp.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/evasapp.h` & `rlottie_python-1.3.4/rlottie/example/evasapp.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/gif.h` & `rlottie_python-1.3.4/rlottie/example/gif.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottie2gif.cpp` & `rlottie_python-1.3.4/rlottie/example/lottie2gif.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottieperf.cpp` & `rlottie_python-1.3.4/rlottie/example/lottieperf.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottieview.cpp` & `rlottie_python-1.3.4/rlottie/example/lottieview.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottieview.h` & `rlottie_python-1.3.4/rlottie/example/lottieview.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottieviewer.cpp` & `rlottie_python-1.3.4/rlottie/example/lottieviewer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/lottieviewtest.cpp` & `rlottie_python-1.3.4/rlottie/example/lottieviewtest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/meson.build` & `rlottie_python-1.3.4/rlottie/example/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/pathtest.cpp` & `rlottie_python-1.3.4/rlottie/example/pathtest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/1643-exploding-star.json` & `rlottie_python-1.3.4/rlottie/example/resource/1643-exploding-star.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/1667-firework.json` & `rlottie_python-1.3.4/rlottie/example/resource/1667-firework.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/1st_animation.lottie` & `rlottie_python-1.3.4/rlottie/example/resource/1st_animation.lottie`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/27746-joypixels-partying-face-emoji-animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/29056-nepenthe-illustration.json` & `rlottie_python-1.3.4/rlottie/example/resource/29056-nepenthe-illustration.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/360º_degree.json` & `rlottie_python-1.3.4/rlottie/example/resource/360º_degree.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/3d.json` & `rlottie_python-1.3.4/rlottie/example/resource/3d.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/4479-fireworks.json` & `rlottie_python-1.3.4/rlottie/example/resource/4479-fireworks.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/5317-fireworkds.json` & `rlottie_python-1.3.4/rlottie/example/resource/5317-fireworkds.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/5344-honey-sack-hud.json` & `rlottie_python-1.3.4/rlottie/example/resource/5344-honey-sack-hud.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/Indicators1.json` & `rlottie_python-1.3.4/rlottie/example/resource/Indicators1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json` & `rlottie_python-1.3.4/rlottie/example/resource/ModernPictogramsForLottie_LoudMute.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/StickAndBall.json` & `rlottie_python-1.3.4/rlottie/example/resource/StickAndBall.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/A Shapes_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/B Fills_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/C Strokes_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/D Transforms_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/E Interpolation_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/F Masks_All_01_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json` & `rlottie_python-1.3.4/rlottie/example/resource/UXSample_1920x1080/F Masks_All_02_1920x1080.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/_alarm.json` & `rlottie_python-1.3.4/rlottie/example/resource/_alarm.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/a_cup_of_coffee.json` & `rlottie_python-1.3.4/rlottie/example/resource/a_cup_of_coffee.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/a_mountain.json` & `rlottie_python-1.3.4/rlottie/example/resource/a_mountain.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/abstract_circle.json` & `rlottie_python-1.3.4/rlottie/example/resource/abstract_circle.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/acrobatics.json` & `rlottie_python-1.3.4/rlottie/example/resource/acrobatics.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/anubis.json` & `rlottie_python-1.3.4/rlottie/example/resource/anubis.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/ao.json` & `rlottie_python-1.3.4/rlottie/example/resource/ao.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/balloons_with_string.json` & `rlottie_python-1.3.4/rlottie/example/resource/balloons_with_string.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/bell.json` & `rlottie_python-1.3.4/rlottie/example/resource/bell.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/birth_stone_logo.json` & `rlottie_python-1.3.4/rlottie/example/resource/birth_stone_logo.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/bounching_ball.json` & `rlottie_python-1.3.4/rlottie/example/resource/bounching_ball.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/browser.json` & `rlottie_python-1.3.4/rlottie/example/resource/browser.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/confetti.json` & `rlottie_python-1.3.4/rlottie/example/resource/confetti.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/cooking.json` & `rlottie_python-1.3.4/rlottie/example/resource/cooking.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/dna.json` & `rlottie_python-1.3.4/rlottie/example/resource/dna.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/done.json` & `rlottie_python-1.3.4/rlottie/example/resource/done.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/dynamic_path_test.json` & `rlottie_python-1.3.4/rlottie/example/resource/dynamic_path_test.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/dynamic_property.json` & `rlottie_python-1.3.4/rlottie/example/resource/dynamic_property.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/eid_mubarak.json` & `rlottie_python-1.3.4/rlottie/example/resource/eid_mubarak.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/emoji_shock.json` & `rlottie_python-1.3.4/rlottie/example/resource/emoji_shock.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/emoji_wink.json` & `rlottie_python-1.3.4/rlottie/example/resource/emoji_wink.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/file_transfer.json` & `rlottie_python-1.3.4/rlottie/example/resource/file_transfer.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/fingerprint_success.json` & `rlottie_python-1.3.4/rlottie/example/resource/fingerprint_success.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/funky_chicken.json` & `rlottie_python-1.3.4/rlottie/example/resource/funky_chicken.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/gears.json` & `rlottie_python-1.3.4/rlottie/example/resource/gears.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/gears_or_settings.json` & `rlottie_python-1.3.4/rlottie/example/resource/gears_or_settings.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/glow_loading.json` & `rlottie_python-1.3.4/rlottie/example/resource/glow_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/gradient_animated_background.json` & `rlottie_python-1.3.4/rlottie/example/resource/gradient_animated_background.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/gradient_sleepy_loader.json` & `rlottie_python-1.3.4/rlottie/example/resource/gradient_sleepy_loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/happy.json` & `rlottie_python-1.3.4/rlottie/example/resource/happy.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/heart.json` & `rlottie_python-1.3.4/rlottie/example/resource/heart.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/hourglass.json` & `rlottie_python-1.3.4/rlottie/example/resource/hourglass.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/image_embedded.json` & `rlottie_python-1.3.4/rlottie/example/resource/image_embedded.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/image_test.json` & `rlottie_python-1.3.4/rlottie/example/resource/image_test.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/images/img_0.png` & `rlottie_python-1.3.4/rlottie/example/resource/images/img_0.png`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/imprint.json` & `rlottie_python-1.3.4/rlottie/example/resource/imprint.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/insta_camera.json` & `rlottie_python-1.3.4/rlottie/example/resource/insta_camera.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/intelia_logo_animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/intelia_logo_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/it's_lunch_time!.json` & `rlottie_python-1.3.4/rlottie/example/resource/it's_lunch_time!.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/jolly_walker.json` & `rlottie_python-1.3.4/rlottie/example/resource/jolly_walker.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/layout.edc` & `rlottie_python-1.3.4/rlottie/example/resource/layout.edc`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/layout.edj` & `rlottie_python-1.3.4/rlottie/example/resource/layout.edj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/leap_frog_loader.json` & `rlottie_python-1.3.4/rlottie/example/resource/leap_frog_loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/like.json` & `rlottie_python-1.3.4/rlottie/example/resource/like.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loader.json` & `rlottie_python-1.3.4/rlottie/example/resource/loader.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loader_4.json` & `rlottie_python-1.3.4/rlottie/example/resource/loader_4.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loader_animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/loader_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loading.json` & `rlottie_python-1.3.4/rlottie/example/resource/loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loading_.json` & `rlottie_python-1.3.4/rlottie/example/resource/loading_.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loading_animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/loading_rectangles.json` & `rlottie_python-1.3.4/rlottie/example/resource/loading_rectangles.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json` & `rlottie_python-1.3.4/rlottie/example/resource/looping_landscape_+_plane_+_clouds.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/maps.json` & `rlottie_python-1.3.4/rlottie/example/resource/maps.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/marker.json` & `rlottie_python-1.3.4/rlottie/example/resource/marker.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/mask.json` & `rlottie_python-1.3.4/rlottie/example/resource/mask.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/material_wave_loading.json` & `rlottie_python-1.3.4/rlottie/example/resource/material_wave_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/matte_two_item_with_lowerlayer.json` & `rlottie_python-1.3.4/rlottie/example/resource/matte_two_item_with_lowerlayer.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/mnemonics.json` & `rlottie_python-1.3.4/rlottie/example/resource/mnemonics.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/movie_loading.json` & `rlottie_python-1.3.4/rlottie/example/resource/movie_loading.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/mughead.json` & `rlottie_python-1.3.4/rlottie/example/resource/mughead.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/night_own.json` & `rlottie_python-1.3.4/rlottie/example/resource/night_own.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/ondas.json` & `rlottie_python-1.3.4/rlottie/example/resource/ondas.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/party_penguin.json` & `rlottie_python-1.3.4/rlottie/example/resource/party_penguin.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/peli-canon.json` & `rlottie_python-1.3.4/rlottie/example/resource/peli-canon.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/personal_character.json` & `rlottie_python-1.3.4/rlottie/example/resource/personal_character.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/polystar_anim.json` & `rlottie_python-1.3.4/rlottie/example/resource/polystar_anim.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/polystar_line_clockwise_trim.json` & `rlottie_python-1.3.4/rlottie/example/resource/polystar_line_clockwise_trim.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/pumped_up.json` & `rlottie_python-1.3.4/rlottie/example/resource/pumped_up.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/red_box.json` & `rlottie_python-1.3.4/rlottie/example/resource/red_box.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/ripple_loading_animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/ripple_loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/settings.json` & `rlottie_python-1.3.4/rlottie/example/resource/settings.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/spin,_lil_loader_v2.json` & `rlottie_python-1.3.4/rlottie/example/resource/spin,_lil_loader_v2.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/square_wheel.json` & `rlottie_python-1.3.4/rlottie/example/resource/square_wheel.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/starts_transparent.json` & `rlottie_python-1.3.4/rlottie/example/resource/starts_transparent.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/static_dynamic_dash.json` & `rlottie_python-1.3.4/rlottie/example/resource/static_dynamic_dash.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/telegram.json` & `rlottie_python-1.3.4/rlottie/example/resource/telegram.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/test/repro_infinite_loop.json` & `rlottie_python-1.3.4/rlottie/example/resource/test/repro_infinite_loop.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json` & `rlottie_python-1.3.4/rlottie/example/resource/test/repro_propertyhelper_type_confusion1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json` & `rlottie_python-1.3.4/rlottie/example/resource/test/repro_propertyhelper_type_confusion2.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/test/repro_sbof.json` & `rlottie_python-1.3.4/rlottie/example/resource/test/repro_sbof.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json` & `rlottie_python-1.3.4/rlottie/example/resource/test/repro_shapeproperty_type_confusion1.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/tile_grid_loading_animation.json` & `rlottie_python-1.3.4/rlottie/example/resource/tile_grid_loading_animation.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/tractor.json` & `rlottie_python-1.3.4/rlottie/example/resource/tractor.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/triib_manage.json` & `rlottie_python-1.3.4/rlottie/example/resource/triib_manage.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/waves_.json` & `rlottie_python-1.3.4/rlottie/example/resource/waves_.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/windmill.json` & `rlottie_python-1.3.4/rlottie/example/resource/windmill.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/world_locations.json` & `rlottie_python-1.3.4/rlottie/example/resource/world_locations.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/worm.json` & `rlottie_python-1.3.4/rlottie/example/resource/worm.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/resource/you're_in!.json` & `rlottie_python-1.3.4/rlottie/example/resource/you're_in!.json`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/uxsampletest.cpp` & `rlottie_python-1.3.4/rlottie/example/uxsampletest.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/Source.cpp` & `rlottie_python-1.3.4/rlottie/example/win32Player/Source.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/resource.h` & `rlottie_python-1.3.4/rlottie/example/win32Player/resource.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottie.dll` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottie.dll`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottie.lib` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottie.lib`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.cpp` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.exe` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.exe`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.h` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.ico` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.ico`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.rc` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.rc`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.sln` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.sln`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.vcxproj` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.vcxproj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters` & `rlottie_python-1.3.4/rlottie/example/win32Player/rlottiePlayer.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/example/win32Player/small.ico` & `rlottie_python-1.3.4/rlottie/example/win32Player/small.ico`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/inc/rlottie.h` & `rlottie_python-1.3.4/rlottie/inc/rlottie.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/inc/rlottie_capi.h` & `rlottie_python-1.3.4/rlottie/inc/rlottie_capi.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/inc/rlottiecommon.h` & `rlottie_python-1.3.4/rlottie/inc/rlottiecommon.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.FTL` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.FTL`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.MIT` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.MIT`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.MPL` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.MPL`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.PIX` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.PIX`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.RPD` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.RPD`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.SKIA` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.SKIA`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/licenses/COPYING.STB` & `rlottie_python-1.3.4/rlottie/licenses/COPYING.STB`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/meson.build` & `rlottie_python-1.3.4/rlottie/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/meson_options.txt` & `rlottie_python-1.3.4/rlottie/meson_options.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/packaging/rlottie.spec` & `rlottie_python-1.3.4/rlottie/packaging/rlottie.spec`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/binding/c/lottieanimation_capi.cpp` & `rlottie_python-1.3.4/rlottie/src/binding/c/lottieanimation_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/CMakeLists.txt` & `rlottie_python-1.3.4/rlottie/src/lottie/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieanimation.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieanimation.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottiefiltermodel.h` & `rlottie_python-1.3.4/rlottie/src/lottie/lottiefiltermodel.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieitem.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieitem.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieitem.h` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieitem.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieitem_capi.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieitem_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottiekeypath.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottiekeypath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottiekeypath.h` & `rlottie_python-1.3.4/rlottie/src/lottie/lottiekeypath.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieloader.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieloader.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottiemodel.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottiemodel.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottiemodel.h` & `rlottie_python-1.3.4/rlottie/src/lottie/lottiemodel.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/lottieparser.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/lottieparser.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/allocators.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/cursorstreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/document.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/encodedstream.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/encodings.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/error/en.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/error/error.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/filereadstream.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/filewritestream.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/fwd.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/biginteger.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/clzll.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/clzll.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/diyfp.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/dtoa.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/ieee754.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/itoa.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/meta.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/pow10.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/regex.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/stack.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/strfunc.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/strtod.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/internal/swap.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/istreamwrapper.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/memorybuffer.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/memorystream.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/msinttypes/stdint.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/ostreamwrapper.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/pointer.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/prettywriter.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/rapidjson.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/reader.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/schema.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/stream.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/stringbuffer.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/rapidjson/writer.h` & `rlottie_python-1.3.4/rlottie/src/lottie/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/zip/miniz.h` & `rlottie_python-1.3.4/rlottie/src/lottie/zip/miniz.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/zip/zip.cpp` & `rlottie_python-1.3.4/rlottie/src/lottie/zip/zip.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/lottie/zip/zip.h` & `rlottie_python-1.3.4/rlottie/src/lottie/zip/zip.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/meson.build` & `rlottie_python-1.3.4/rlottie/src/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/CMakeLists.txt` & `rlottie_python-1.3.4/rlottie/src/vector/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_math.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_math.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_math.h` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_math.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_raster.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_raster.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_raster.h` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_raster.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_stroker.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_stroker.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_stroker.h` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_stroker.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/freetype/v_ft_types.h` & `rlottie_python-1.3.4/rlottie/src/vector/freetype/v_ft_types.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/meson.build` & `rlottie_python-1.3.4/rlottie/src/vector/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.S` & `rlottie_python-1.3.4/rlottie/src/vector/pixman/pixman-arm-neon-asm.S`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/pixman/pixman-arm-neon-asm.h` & `rlottie_python-1.3.4/rlottie/src/vector/pixman/pixman-arm-neon-asm.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/stb/CMakeLists.txt` & `rlottie_python-1.3.4/rlottie/src/vector/stb/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/stb/meson.build` & `rlottie_python-1.3.4/rlottie/src/vector/stb/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/stb/stb_image.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/stb/stb_image.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/stb/stb_image.h` & `rlottie_python-1.3.4/rlottie/src/vector/stb/stb_image.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/varenaalloc.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/varenaalloc.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/varenaalloc.h` & `rlottie_python-1.3.4/rlottie/src/vector/varenaalloc.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbezier.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vbezier.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbezier.h` & `rlottie_python-1.3.4/rlottie/src/vector/vbezier.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbitmap.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vbitmap.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbitmap.h` & `rlottie_python-1.3.4/rlottie/src/vector/vbitmap.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbrush.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vbrush.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vbrush.h` & `rlottie_python-1.3.4/rlottie/src/vector/vbrush.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vcowptr.h` & `rlottie_python-1.3.4/rlottie/src/vector/vcowptr.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdasher.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdasher.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdasher.h` & `rlottie_python-1.3.4/rlottie/src/vector/vdasher.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdebug.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdebug.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdebug.h` & `rlottie_python-1.3.4/rlottie/src/vector/vdebug.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawable.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawable.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawable.h` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawable.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper.h` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_common.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_common.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_neon.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_neon.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vdrawhelper_sse2.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vdrawhelper_sse2.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/velapsedtimer.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/velapsedtimer.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/velapsedtimer.h` & `rlottie_python-1.3.4/rlottie/src/vector/velapsedtimer.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vglobal.h` & `rlottie_python-1.3.4/rlottie/src/vector/vglobal.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vimageloader.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vimageloader.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vinterpolator.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vinterpolator.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vinterpolator.h` & `rlottie_python-1.3.4/rlottie/src/vector/vinterpolator.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vline.h` & `rlottie_python-1.3.4/rlottie/src/vector/vline.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vmatrix.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vmatrix.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vmatrix.h` & `rlottie_python-1.3.4/rlottie/src/vector/vmatrix.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpainter.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vpainter.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpainter.h` & `rlottie_python-1.3.4/rlottie/src/vector/vpainter.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpath.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vpath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpath.h` & `rlottie_python-1.3.4/rlottie/src/vector/vpath.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpathmesure.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vpathmesure.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpathmesure.h` & `rlottie_python-1.3.4/rlottie/src/vector/vpathmesure.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vpoint.h` & `rlottie_python-1.3.4/rlottie/src/vector/vpoint.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vraster.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vraster.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vraster.h` & `rlottie_python-1.3.4/rlottie/src/vector/vraster.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vrect.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vrect.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vrect.h` & `rlottie_python-1.3.4/rlottie/src/vector/vrect.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vrle.cpp` & `rlottie_python-1.3.4/rlottie/src/vector/vrle.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vrle.h` & `rlottie_python-1.3.4/rlottie/src/vector/vrle.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vsharedptr.h` & `rlottie_python-1.3.4/rlottie/src/vector/vsharedptr.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vstackallocator.h` & `rlottie_python-1.3.4/rlottie/src/vector/vstackallocator.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/vector/vtaskqueue.h` & `rlottie_python-1.3.4/rlottie/src/vector/vtaskqueue.h`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/src/wasm/rlottiewasm.cpp` & `rlottie_python-1.3.4/rlottie/src/wasm/rlottiewasm.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/CMakeLists.txt` & `rlottie_python-1.3.4/rlottie/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/meson.build` & `rlottie_python-1.3.4/rlottie/test/meson.build`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/test_lottieanimation.cpp` & `rlottie_python-1.3.4/rlottie/test/test_lottieanimation.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/test_lottieanimation_capi.cpp` & `rlottie_python-1.3.4/rlottie/test/test_lottieanimation_capi.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/test_vpath.cpp` & `rlottie_python-1.3.4/rlottie/test/test_vpath.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/test_vrect.cpp` & `rlottie_python-1.3.4/rlottie/test/test_vrect.cpp`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/test/wasm_test.html` & `rlottie_python-1.3.4/rlottie/test/wasm_test.html`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/vs2019/rlottie.sln` & `rlottie_python-1.3.4/rlottie/vs2019/rlottie.sln`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/vs2019/rlottie.vcxproj` & `rlottie_python-1.3.4/rlottie/vs2019/rlottie.vcxproj`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/vs2019/rlottie.vcxproj.filters` & `rlottie_python-1.3.4/rlottie/vs2019/rlottie.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/wasm_build.sh` & `rlottie_python-1.3.4/rlottie/wasm_build.sh`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie/wasm_cross.txt` & `rlottie_python-1.3.4/rlottie/wasm_cross.txt`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie_python/_rlottiecommon.py` & `rlottie_python-1.3.4/src/rlottie_python/_rlottiecommon.py`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/rlottie_python/rlottie_wrapper.py` & `rlottie_python-1.3.4/src/rlottie_python/rlottie_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlottie_python-1.3.3/PKG-INFO` & `rlottie_python-1.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlottie-python
-Version: 1.3.3
+Version: 1.3.4
 Summary: A ctypes API for rlottie, with additional functions for getting Pillow Image.
 Keywords: rlottie lottie tgs ctypes
 Author-Email: chaudominic <chaudominic2@gmail.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -509,14 +509,23 @@
         
         That's all there is to it!
 Classifier: Topic :: Multimedia :: Graphics
 Project-URL: Repository, https://github.com/laggykiller/rlottie-python
 Project-URL: Documentation, https://rlottie-python.readthedocs.io/en/latest/
 Project-URL: Tracker, https://github.com/laggykiller/rlottie-python/issues
 Requires-Python: >=3.7
+Provides-Extra: full
+Provides-Extra: test
+Provides-Extra: lint
+Requires-Dist: Pillow; extra == "full"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: ruff; extra == "lint"
+Requires-Dist: mypy; extra == "lint"
+Requires-Dist: isort; extra == "lint"
+Requires-Dist: types-Pillow; extra == "lint"
 Description-Content-Type: text/markdown
 
 # rlottie-python
 
 A ctypes API for rlottie, with additional functions for getting Pillow Image and animated sequences, as well as telegram animated stickers (tgs).
 
 See example/example.py for example usage.
@@ -533,48 +542,22 @@
 - [Credits](#credits)
 
 ## Installing
 
 Note that rlottie is included in the wheel package, you need not install librlottie.
 
 To install, run the following:
-```
-pip3 install wheel
+```bash
 pip3 install rlottie-python
 ```
 
-Optionally, install `Pillow`:
-```
-pip3 install Pillow
-```
-
-## Building from source
-
-To build wheel, run the following:
-```
-git clone --recursive https://github.com/laggykiller/rlottie-python.git
-cd rlottie-python
-pip3 install -r requirements.txt
-python3 -m build .
-```
-
-To install the built wheel, run `pip3 install dist/<name_of_the_wheel_file>.whl`
-
-If you want to install directly, run the following:
+`Pillow` is optional dependency. It is required for `render_pillow_frame()`,
+`save_frame()` and `save_animation()`. To also install Pillow, run:
 ```bash
-git clone --recursive https://github.com/laggykiller/rlottie-python.git
-cd rlottie-python
-pip3 install -r requirements.txt
-pip3 install .
-```
-
-To run tests:
-```bash
-pip install pytest
-pytest
+pip3 install rlottie-python[full]
 ```
 
 ## Examples
 Getting information about an lottie animation
 ```python
 from rlottie_python import LottieAnimation
 
@@ -649,10 +632,40 @@
 ```
 
 ## Comparing to other library
 The `lottie` (https://pypi.org/project/lottie/) python package is also capable of working with lottie files and telegram animated stickers (tgs). It is also able to support many input/output formats and vector graphics, without any dependency on extenral libraries such as librlottie. However some images it creates is broken ([Example1](https://github.com/laggykiller/sticker-convert/issues/5) [Example2](https://gitlab.com/mattbas/python-lottie/-/issues/95)). It seems librlottie is more stable in terms of rendering frames.
 
 The `pyrlottie` (https://pypi.org/project/pyrlottie/) python package is also able to convert lottie and tgs files to webp/gif. However, it works by calling executables `gif2webp` and `lottie2gif` with subprocess, and it does not support macOS.
 
+## Building from source
+
+To build wheel, run the following:
+```bash
+git clone --recursive https://github.com/laggykiller/rlottie-python.git
+cd rlottie-python
+
+# To build wheel
+python3 -m build .
+
+# To install directly
+pip3 install .
+```
+
+## Development
+To run tests:
+```bash
+pip install pytest
+pytest
+```
+
+To lint:
+```bash
+pip install ruff mypy isort
+mypy
+isort .
+ruff check
+ruff format
+```
+
 ## Credits
 - rlottie library: https://github.com/Samsung/rlottie
 - Packaging: https://github.com/tttapa/py-build-cmake
```

