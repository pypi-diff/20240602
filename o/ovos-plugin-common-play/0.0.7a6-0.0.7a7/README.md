# Comparing `tmp/ovos_plugin_common_play-0.0.7a6.tar.gz` & `tmp/ovos_plugin_common_play-0.0.7a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos_plugin_common_play-0.0.7a6.tar", last modified: Tue May 28 01:08:14 2024, max compression
+gzip compressed data, was "ovos_plugin_common_play-0.0.7a7.tar", last modified: Sun Jun  2 21:14:04 2024, max compression
```

## Comparing `ovos_plugin_common_play-0.0.7a6.tar` & `ovos_plugin_common_play-0.0.7a7.tar`

### file list

```diff
@@ -1,865 +1,865 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.763388 ovos_plugin_common_play-0.0.7a6/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-28 01:08:14.763388 ovos_plugin_common_play-0.0.7a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.647388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.651388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)    17467 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    20787 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/mpris.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/mycroft_cps.py
--rw-r--r--   0 runner    (1001) docker     (127)    38201 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/player.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.647388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.651388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/desktop/OCP.desktop
--rw-r--r--   0 runner    (1001) docker     (127)    34972 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/desktop/OCP.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.647388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.655388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.663388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.671388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.675388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/news.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/open.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/porn.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)     2937 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/read.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.683388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/documentaries.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.687388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.695388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.699388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.707388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/documentaries.intent
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/phrase.rx
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/it-it/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.715388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.719388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.727388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.731388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.739388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.743388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.751388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Pause.voc
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/PlayResume.voc
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Track.voc
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio.intent
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio_only.voc
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.intent
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.voc
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/cant.play.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/converse_resume.voc
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/documentaries.intent
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/game.intent
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/just.one.moment.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/movietrailer.intent
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/music.intent
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/news.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/pause.intent
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.intent
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.what.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/porn.intent
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio_drama.intent
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/read.intent
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/setup.hints.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/short_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/silent_movie.intent
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/trailer.voc
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/video.intent
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/video_only.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.755388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.755388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2896 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml
--rw-r--r--   0 runner    (1001) docker     (127)    21593 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigOptionDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Home.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2788 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml
--rw-r--r--   0 runner    (1001) docker     (127)    21245 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Playlist.qml
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Search.qml
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.755388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.755388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/code/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/code/helper.js
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/code/nav.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.759388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/delegates/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4508 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/delegates/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.763388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/back.png
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/history.png
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/home.png
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/information.png
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playback-pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playback-start.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playback-stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-seek-backward.svg
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-seek-forward.svg
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-skip-backward.svg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-skip-forward.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34972 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    36598 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    48707 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp.png
--rw-r--r--   0 runner    (1001) docker     (127)    74222 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/search.png
--rw-r--r--   0 runner    (1001) docker     (127)    97623 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.763388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3171 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4927 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)    20391 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/search.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:08:14.647388 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:08:14.763388 ovos_plugin_common_play-0.0.7a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3832 2024-05-28 01:08:14.000000 ovos_plugin_common_play-0.0.7a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.727199 ovos_plugin_common_play-0.0.7a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-06-02 21:14:04.727199 ovos_plugin_common_play-0.0.7a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.619198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.623199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)    17847 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20632 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23097 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/mpris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/mycroft_cps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38242 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/player.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.619198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.623199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/desktop/OCP.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)    34972 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/desktop/OCP.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.619198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.631199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.635198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.643199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.647199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/news.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/open.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)      554 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/porn.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2937 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/read.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.655198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/documentaries.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)      106 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.659199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.667199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.675199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.679199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/documentaries.intent
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/phrase.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/it-it/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.683199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.691198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.695199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.699199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.707198 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.711199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.715199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Pause.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/PlayResume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Track.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audio_only.voc
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/behind_scenes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/cant.play.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/converse_resume.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/documentaries.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/game.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/just.one.moment.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/movietrailer.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/music.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/news.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/pause.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/play.what.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/porn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio_drama.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/read.intent
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/setup.hints.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/short_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/silent_movie.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/trailer.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/video.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/video_only.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.719199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.723199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2896 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    21593 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigOptionDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Home.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2788 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    21245 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Playlist.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Search.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.723199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.723199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/code/helper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/code/nav.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.723199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/delegates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4508 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/delegates/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.727199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/back.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/history.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/home.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/information.png
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-start.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playback-stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-seek-backward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-seek-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-skip-backward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-skip-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34972 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36598 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48707 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74222 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/search.png
+-rw-r--r--   0 runner    (1001) docker     (127)    97623 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.727199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3171 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4927 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 21:14:04.623199 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 21:14:04.727199 ovos_plugin_common_play-0.0.7a7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3832 2024-06-02 21:14:04.000000 ovos_plugin_common_play-0.0.7a7/setup.py
```

### Comparing `ovos_plugin_common_play-0.0.7a6/CHANGELOG.md` & `ovos_plugin_common_play-0.0.7a7/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Changelog
 
-## [0.0.7a6](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/tree/0.0.7a6) (2024-05-28)
+## [0.0.7a7](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/tree/0.0.7a7) (2024-06-02)
 
-[Full Changelog](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/compare/V0.0.7a5...0.0.7a6)
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/compare/V0.0.7a6...0.0.7a7)
+
+**Merged pull requests:**
+
+- default to OCP pipeline + support for utils 0.0.38 [\#119](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/pull/119) ([JarbasAl](https://github.com/JarbasAl))
+
+## [V0.0.7a6](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/tree/V0.0.7a6) (2024-05-28)
+
+[Full Changelog](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/compare/V0.0.7a5...V0.0.7a6)
 
 **Fixed bugs:**
 
 - fix/playlist\_again [\#117](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/pull/117) ([JarbasAl](https://github.com/JarbasAl))
 
 ## [V0.0.7a5](https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin/tree/V0.0.7a5) (2024-05-25)
```

### Comparing `ovos_plugin_common_play-0.0.7a6/LICENSE` & `ovos_plugin_common_play-0.0.7a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/PKG-INFO` & `ovos_plugin_common_play-0.0.7a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos_plugin_common_play
-Version: 0.0.7a6
+Version: 0.0.7a7
 Summary: OVOS common play audio service adapter plugin
 Home-page: https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos audio plugin
 Platform: UNKNOWN
```

### Comparing `ovos_plugin_common_play-0.0.7a6/README.md` & `ovos_plugin_common_play-0.0.7a7/README.md`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/__init__.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pprint import pformat
 
 from ovos_bus_client import Message
+from ovos_utils.log import LOG
+from ovos_workshop.decorators.ocp import *
+
 from ovos_plugin_common_play.ocp import OCP
 from ovos_plugin_common_play.ocp.base import OCPAudioPlayerBackend
-from ovos_utils.ocp import *
-from ovos_utils.log import LOG
+from ovos_plugin_common_play.ocp.constants import OCP_ID
 
 
 class OCPAudioBackend(OCPAudioPlayerBackend):
     """ This plugin makes regular mycroft skills that use the audio service
     go trough the OVOS common play framework, this plugin simply delegates
     the task by emitting bus messages expected by Ovos Common Play API. If
     configured it will also launch OCP itself """
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/launcher.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/launcher.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 from ovos_bus_client import MessageBusClient
-from ovos_plugin_common_play.ocp import OCP, OCP_ID
 from ovos_utils import wait_for_exit_signal
 
+from ovos_plugin_common_play.ocp import OCP
+from ovos_plugin_common_play.ocp.constants import OCP_ID
+
 
 def main():
     """
     Console script entrypoint
     USAGE: ovos-ocp-standalone
     """
     bus = MessageBusClient()
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/__init__.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 from threading import Event, Lock
 from ovos_config import Configuration
 from ovos_plugin_common_play.ocp.gui import OCPMediaPlayerGUI
 from ovos_plugin_common_play.ocp.player import OCPMediaPlayer
 from ovos_utils.gui import can_use_gui
 from ovos_utils.log import LOG
 from ovos_utils.messagebus import Message
-from ovos_utils.ocp import OCP_ID
+
 from padacioso import IntentContainer
 
 from ovos_workshop import OVOSAbstractApplication
 from ovos_workshop.decorators.ocp import *
 from ovos_plugin_manager.ocp import load_stream_extractors
 
+from ovos_plugin_common_play.ocp.constants import OCP_ID
+
 
 class OCP(OVOSAbstractApplication):
     intent2media = {
         "music": MediaType.MUSIC,
         "video": MediaType.VIDEO,
         "audiobook": MediaType.AUDIOBOOK,
         "radio": MediaType.RADIO,
@@ -121,18 +123,23 @@
         @param message: message associated with request
         """
         # homescreen / launch from .desktop
         self.gui.show_home(app_mode=True)
 
     @property
     def using_new_pipeline(self) -> bool:
-        # TODO - default to True in ovos-core 0.1.0
-        # more info: https://github.com/OpenVoiceOS/ovos-core/pull/456
-        moved_to_pipelines = Configuration().get("intents", {}).get("experimental_ocp_pipeline")
-        return moved_to_pipelines
+        # this is no longer configurable, most of this repo is dead code
+        # keep this check to allow smooth updates from the couple alpha versions this was live
+        if Configuration().get("intents", {}).get("experimental_ocp_pipeline"):
+            return True
+        # check for min version for default ovos-config to contain OCP pipeline
+        from ovos_config.version import VERSION_BUILD, VERSION_ALPHA, VERSION_MAJOR, VERSION_MINOR
+        if VERSION_BUILD > 13 or VERSION_MAJOR >= 1 or VERSION_MINOR >= 1:
+            return True
+        return VERSION_BUILD == 13 and VERSION_ALPHA >= 14
 
     def register_ocp_intents(self, message=None):
         if self.using_new_pipeline:
             LOG.debug("skipping Classic OCP intent registration")
             return
 
         with self._intent_registration_lock:
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/base.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from os.path import join, isfile
 
 from ovos_bus_client.message import Message
-from ovos_plugin_common_play.ocp.utils import extract_metadata
-from ovos_utils.log import LOG
-from ovos_utils.ocp import MediaState, PlayerState, OCP_ID, TrackState
-
-
 from ovos_config.locations import get_xdg_config_save_path
 from ovos_plugin_manager.templates.audio import AudioBackend
+from ovos_utils.log import LOG
+from ovos_workshop.decorators.ocp import MediaState, PlayerState, TrackState
+
+from ovos_plugin_common_play.ocp.constants import OCP_ID
+from ovos_plugin_common_play.ocp.utils import extract_metadata
 
 
 class OCPAbstractComponent:
     def __init__(self, player=None):
         """
         player: OCPInterface
         """
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/gui.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import enum
 from os.path import join, dirname
-
-from ovos_utils.ocp import OCP_ID, MediaType, PlayerState, LoopState, PlaybackType
+from threading import Timer
 from time import sleep
+
+from ovos_bus_client.apis.gui import GUIInterface
 from ovos_bus_client.message import Message
 from ovos_config import Configuration
 from ovos_utils.events import EventSchedulerInterface
-from ovos_bus_client.apis.gui import GUIInterface
 from ovos_utils.log import LOG
+from ovos_workshop.decorators.ocp import MediaType, PlayerState, LoopState, PlaybackType
 
+from ovos_plugin_common_play.ocp.constants import OCP_ID
 from ovos_plugin_common_play.ocp.utils import is_qtav_available
-from threading import Timer
 
 
 class VideoPlayerBackend(str, enum.Enum):
     AUTO = "auto"
     QTAV = "qtav"
     NATIVE = "native"
 
@@ -49,20 +50,20 @@
                               self.handle_play_skill_featured_media)
         self.event_scheduler_interface = \
             EventSchedulerInterface(skill_id=OCP_ID, bus=self.bus)
 
     @property
     def video_backend(self):
         return self.player.settings.get("video_player_backend") or \
-               VideoPlayerBackend.AUTO
+            VideoPlayerBackend.AUTO
 
     @property
     def home_screen_page(self):
         return "Home"
-    
+
     @property
     def disambiguation_playlists_page(self):
         return "SuggestionsView"
 
     @property
     def audio_player_page(self):
         return "OVOSAudioPlayer"
@@ -109,15 +110,15 @@
     # OCPMediaPlayer interface
     def update_ocp_skills(self):
         skills_cards = [
             {"skill_id": skill["skill_id"],
              "title": skill["skill_name"],
              "image": skill["thumbnail"],
              "media_type": skill.get("media_type") or [MediaType.GENERIC]
-        } for skill in self.player.media.get_featured_skills()]
+             } for skill in self.player.media.get_featured_skills()]
         self["skillCards"] = skills_cards
 
     def update_seekbar_capabilities(self):
         self["canResume"] = True
         self["canPause"] = True
         self["canPrev"] = self.player.can_prev
         self["canNext"] = self.player.can_next
@@ -138,27 +139,27 @@
     def update_current_track(self):
         self.update_seekbar_capabilities()
 
         self["media"] = self.player.now_playing.info
         self["uri"] = self.player.now_playing.uri
         self["title"] = self.player.now_playing.title
         self["image"] = self.player.now_playing.image or \
-            join(dirname(__file__), "res/ui/images/ocp.png")
+                        join(dirname(__file__), "res/ui/images/ocp.png")
         self["artist"] = self.player.now_playing.artist
         self["bg_image"] = self.player.now_playing.bg_image or \
-            join(dirname(__file__), "res/ui/images/ocp_bg.png")
+                           join(dirname(__file__), "res/ui/images/ocp_bg.png")
         self["duration"] = self.player.now_playing.length
         self["position"] = self.player.now_playing.position
         # options below control the web player
         # javascript can be executed on page load and page behaviour modified
         # default values provide crude protection against ads and popups
         # TODO default permissive or restrictive?
         self["javascript"] = self.player.now_playing.javascript
         self["javascriptCanOpenWindows"] = False  # TODO allow to be defined per track
-        self["allowUrlChange"] = False # TODO allow to be defined per track
+        self["allowUrlChange"] = False  # TODO allow to be defined per track
 
     def update_search_results(self):
         self["searchModel"] = {
             "data": [e.infocard for e in self.player.disambiguation]
         }
 
     def update_playlist(self):
@@ -177,53 +178,53 @@
 
     def manage_display(self, page_requested, timeout=None):
         # Home:
         # The home search page will always be shown at Protocol level index 0
         # This is to ensure that the home is always available to the user
         # regardless of what other pages are currently open
         # Swiping from the player to the left will always show the home page
-        
+
         # The home page will only be in view if the user is not currently playing an active track
         # If the user is playing a track, the player will be shown instead
         # This is to ensure that the user always returns to the player when they are playing a track
-        
+
         # The search_spinner_page has been integrated into the home page as an overlay
         # It will be shown when the user is searching for a track and will be hidden when the search is complete
         # on platforms that don't support the notification system
-        
+
         # Player:
         # Player loader will always be shown at Protocol level index 1
         # The merged playlist and disambiguation pages will always be shown at Protocol level index 2
-        
+
         # If the user has just opened the ocp home page, and nothing was played previously,
         # the player and merged playlist/disambiguation page will not be shown
-        
+
         # If the user has just opened the ocp home page, and a track was previously played,
         # the player and merged playlist/disambiguation page will always be shown
-        
+
         # If the player is not paused or stopped, the player will be shown instead of the home page
         # when ocp is opened
-        
+
         # Timeout is used to ensure that ocp is fully closed once the timeout has expired
-        
+
         sleep(0.2)
         player_status = self.player.state
         state2str = {PlayerState.PLAYING: "Playing", PlayerState.PAUSED: "Paused", PlayerState.STOPPED: "Stopped"}
         self["status"] = state2str[player_status]
         self["app_view_timeout_enabled"] = self.player.app_view_timeout_enabled
         self["app_view_timeout"] = self.player.app_view_timeout_value
         self["app_view_timeout_mode"] = self.player.app_view_timeout_mode
 
         LOG.debug(f"manage_display: page_requested: {page_requested}")
         LOG.debug(f"manage_display: player_status: {player_status}")
-                
+
         if page_requested == "home":
             self["homepage_index"] = 0
             self["displayBottomBar"] = False
-            
+
             # Check if the skills page has anything to show, only show it if it does
             if self["skillCards"]:
                 self["displayBottomBar"] = True
 
             if player_status == PlayerState.PLAYING:
                 self.show_page(self.player_loader_page, override_idle=True, override_animations=True)
             elif player_status == PlayerState.PAUSED:
@@ -234,24 +235,24 @@
         elif page_requested == "player":
             self["playerBackend"] = self._get_player_page()
             self.show_pages(self._get_pages_to_display(), 0, override_idle=True, override_animations=True)
 
         elif page_requested == "playlist":
             self["displaySuggestionBar"] = False
             self._show_suggestion_playlist()
-            
+
             if timeout is not None:
                 self.show_page(self.disambiguation_playlists_page, override_idle=timeout, override_animations=True)
             else:
                 self.show_page(self.disambiguation_playlists_page, override_idle=True, override_animations=True)
-                
+
         elif page_requested == "disambiguation":
             self["displaySuggestionBar"] = False
             self._show_suggestion_disambiguation()
-            
+
             if timeout is not None:
                 self.show_page(self.disambiguation_playlists_page, override_idle=timeout, override_animations=True)
             else:
                 self.show_page(self.disambiguation_playlists_page, override_idle=True, override_animations=True)
 
         if (self.player.app_view_timeout_enabled and page_requested == "player"
                 and self.player.app_view_timeout_mode == "all"):
@@ -260,15 +261,15 @@
     def cancel_app_view_timeout(self, restart=False):
         self.event_scheduler_interface.cancel_scheduled_event("ocp_app_view_timer")
         if restart:
             self.schedule_app_view_timeout()
 
     def schedule_app_view_pause_timeout(self):
         if (self.player.app_view_timeout_enabled
-            and self.player.app_view_timeout_mode == "pause"
+                and self.player.app_view_timeout_mode == "pause"
                 and self.player.state == PlayerState.PAUSED):
             self.schedule_app_view_timeout()
 
     def schedule_app_view_timeout(self):
         self.event_scheduler_interface.schedule_event(
             self.timeout_app_view, self.player.app_view_timeout_value, data=None, name="ocp_app_view_timer")
 
@@ -328,40 +329,40 @@
             # TODO ?
             return self.audio_service_page
 
     def _get_pages_to_display(self):
         # determine pages to be shown
         self["playerBackend"] = self._get_player_page()
         LOG.debug(f"pages to display backend: {self['playerBackend']}")
-        
+
         if len(self.player.disambiguation):
             self["displaySuggestionBar"] = False
             self._show_suggestion_disambiguation()
-            
+
         if len(self.player.tracks):
             self["displaySuggestionBar"] = False
             self._show_suggestion_playlist()
 
-        if len(self.player.disambiguation) and len(self.player.tracks):   
+        if len(self.player.disambiguation) and len(self.player.tracks):
             self["displaySuggestionBar"] = True
             self._show_suggestion_playlist()
-            
+
         pages = [self.player_loader_page, self.disambiguation_playlists_page]
 
         return pages
 
     def _show_home_search(self):
         self.send_event("ocp.gui.show.home.view.search")
 
     def _show_home_skills(self):
         self.send_event("ocp.gui.show.home.view.skills")
 
     def _show_suggestion_playlist(self):
         self.send_event("ocp.gui.show.suggestion.view.playlist")
-     
+
     def _show_suggestion_disambiguation(self):
         self.send_event("ocp.gui.show.suggestion.view.disambiguation")
 
     # gui <-> playlists
     def handle_play_from_playlist(self, message):
         LOG.debug("Playback requested from playlist results")
         media = message.data["playlistData"]
@@ -370,15 +371,15 @@
                 self.player.play_media(track)
                 break
         else:
             LOG.error("Track is not part of loaded playlist!")
 
     def handle_play_from_search(self, message):
         LOG.debug("Playback requested from search results")
-        media = message.data["playlistData"]        
+        media = message.data["playlistData"]
         for track in self.player.disambiguation:
             if track == media:  # found track
                 self.player.play_media(track)
                 break
         else:
             LOG.error("Track is not part of search results!")
 
@@ -413,15 +414,15 @@
                 show_results = True
         except:
             pass
 
         # show search results, release screen after 60 seconds
         if show_results:
             self.manage_display("playlist", timeout=60)
-            
+
     def display_notification(self, text, style="info"):
         """ Display a notification on the screen instead of spinner on platform that support it """
         self.show_controlled_notification(text, style=style)
         self.reset_timeout_notification()
 
     def clear_notification(self):
         """ Remove the notification on the screen """
@@ -443,15 +444,15 @@
         self.show_home(app_mode=persist_home)
         sleep(0.2)
         self.send_event("ocp.gui.show.busy.overlay")
         self["footer_text"] = "Querying Skills\n\n"
 
     def remove_search_spinner(self):
         self.send_event("ocp.gui.hide.busy.overlay")
-        
+
     def remove_homescreen(self):
         self.release()
 
 
 class OCPExternalGuiInterface(GUIInterface):
     def __init__(self, skill_id):
         super(OCPExternalGuiInterface, self).__init__(skill_id=skill_id)
@@ -463,51 +464,51 @@
     # All skills that use this interface must implement the following pages that will override the OCP GUI
     # pages:
     # - Home / Login / Search, this is the page that will be shown when the skill is launched
     # - Player / Player Loaders, this is the page that will be shown when the skill is launched and the skill is playing
     # - Extra / Disambiguation / Playlist, this is the page that will be shown when the skill is launched and the skill is playing
     # - Custom, allow the skill to show any custom page it wants
     # Page management lifecycle will be handled by the skill itself
-    
+
     def bind(self, player):
         self.player = player
         super().set_bus(self.bus)
 
     def register_screen_type(self, page_url, page_type):
         for page in self.ocp_registered_pages:
             if page["type"] == page_type:
                 return
-    
+
         page_to_register = {
             "page_url": page_url,
             "type": page_type
         }
         self.ocp_registered_pages[page_type] = page_to_register
-    
+
     def get_screen_type(self, page_type):
         return self.ocp_registered_pages[page_type]
-    
+
     def show_screen(self, page_type, override_idle=False, override_animations=False):
         page_to_show = self.get_screen_type(page_type)
         self.show_page(page_to_show["page_url"], override_idle=override_idle, override_animations=override_animations)
-    
+
     def show_home(self, override_idle=False, override_animations=False):
         self.show_screen("home", override_idle, override_animations)
-    
+
     def show_player(self, override_idle=False, override_animations=False):
         self.show_screen("player", override_idle, override_animations)
-    
+
     def show_extra(self, override_idle=False, override_animations=False):
         self.show_screen("extra", override_idle, override_animations)
-        
+
     def remove_screen(self, page_type):
         page_to_remove = self.get_screen_type(page_type)
         self.remove_page(page_to_remove["page_url"])
-    
+
     def remove_home(self):
         self.remove_screen("home")
-    
+
     def remove_player(self):
         self.remove_screen("player")
-    
+
     def remove_extra(self):
         self.remove_screen("extra")
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/media.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/mycroft_cps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,312 +1,314 @@
-from os.path import join, dirname
-from typing import Union
-from ovos_bus_client.client import MessageBusClient
-from ovos_bus_client.message import Message
-from ovos_utils.json_helper import merge_dict
-from ovos_utils.log import LOG
-from ovos_utils.ocp import MediaEntry as _ME, Playlist
-from ovos_utils.ocp import OCP_ID, MediaState, TrackState, PlaybackType, MediaType
-
-from ovos_plugin_common_play.ocp.utils import ocp_plugins
-
-
-class MediaEntry(_ME):
-    def __init__(self, title="", uri="", skill_id=OCP_ID,
-                 image=None, match_confidence=0,
-                 playback=PlaybackType.UNDEFINED,
-                 status=TrackState.DISAMBIGUATION, phrase=None,
-                 position=0, length=0, bg_image=None, skill_icon=None,
-                 artist=None, is_cps=False, cps_data=None, javascript="",
-                 **kwargs):
-        uri = uri or ""
-        super().__init__(
-            title=title,
-            match_confidence=match_confidence,
-            playback=PlaybackType(playback) if isinstance(playback, int) else playback,
-            status=status,
-            length=length,
-            image=image or join(dirname(__file__), "res/ui/images/ocp_bg.png"),
-            skill_icon=skill_icon or join(dirname(__file__), "res/ui/images/ocp.png"),
-            javascript=javascript,
-            uri=f'file://{uri}' if uri.startswith('/') else uri,
-            skill_id=skill_id,
-            media_type=kwargs.get("media_type") or MediaType.GENERIC
-        )
-        self.artist = artist
-        self.position = position
-        self.phrase = phrase
-        self.bg_image = bg_image or join(dirname(__file__), "res/ui/images/ocp_bg.png")
-        self.is_cps = is_cps
-        self.data = kwargs
-        self.cps_data = cps_data or {}
+import time
+from datetime import timedelta
+from os.path import abspath
+
+from ovos_bus_client.message import Message, dig_for_message
+from ovos_bus_client.util import wait_for_reply
+from ovos_workshop.decorators.ocp import MediaType, PlaybackType
+
+from ovos_plugin_common_play.ocp.base import OCPAbstractComponent
+from ovos_plugin_common_play.ocp.constants import OCP_ID
+
+
+def ensure_uri(s):
+    """Interprete paths as file:// uri's.
+
+    Args:
+        s: string to be checked
+
+    Returns:
+        if s is uri, s is returned otherwise file:// is prepended
+    """
+    if isinstance(s, str):
+        if '://' not in s:
+            return 'file://' + abspath(s)
+        else:
+            return s
+    elif isinstance(s, (tuple, list)):
+        if '://' not in s[0]:
+            return 'file://' + abspath(s[0]), s[1]
+        else:
+            return s
+    else:
+        raise ValueError('Invalid track')
+
+
+class MycroftAudioService:
+    """AudioService class for interacting with the mycroft-core audio subsystem
+
+    Args:
+        bus: Mycroft messagebus connection
+    """
+
+    def __init__(self, bus):
+        self.bus = bus
+
+    @staticmethod
+    def _format_msg(msg_type, msg_data=None):
+        # this method ensures all skills are .forward from the utterance
+        # that triggered the skill, this ensures proper routing and metadata
+        msg_data = msg_data or {}
+        msg = dig_for_message()
+        if msg:
+            msg = msg.forward(msg_type, msg_data)
+        else:
+            msg = Message(msg_type, msg_data)
+        # at this stage source == skills, lets indicate audio service took over
+        sauce = msg.context.get("source")
+        if sauce == "skills":
+            msg.context["source"] = OCP_ID
+        return msg
+
+    def queue(self, tracks=None):
+        """Queue up a track to playing playlist.
+
+        Args:
+            tracks: track uri or list of track uri's
+                    Each track can be added as a tuple with (uri, mime)
+                    to give a hint of the mime type to the system
+        """
+        tracks = tracks or []
+        if isinstance(tracks, (str, tuple)):
+            tracks = [tracks]
+        elif not isinstance(tracks, list):
+            raise ValueError
+        tracks = [ensure_uri(t) for t in tracks]
+        msg = self._format_msg('mycroft.audio.service.queue',
+                               {'tracks': tracks})
+        self.bus.emit(msg)
+
+    def play(self, tracks=None, utterance=None, repeat=None):
+        """Start playback.
+
+        Args:
+            tracks: track uri or list of track uri's
+                    Each track can be added as a tuple with (uri, mime)
+                    to give a hint of the mime type to the system
+            utterance: forward utterance for further processing by the
+                        audio service.
+            repeat: if the playback should be looped
+        """
+        repeat = repeat or False
+        tracks = tracks or []
+        utterance = utterance or ''
+        if isinstance(tracks, (str, tuple)):
+            tracks = [tracks]
+        elif not isinstance(tracks, list):
+            raise ValueError
+        tracks = [ensure_uri(t) for t in tracks]
+        msg = self._format_msg('mycroft.audio.service.play',
+                               {'tracks': tracks,
+                                'utterance': utterance,
+                                'repeat': repeat})
+        self.bus.emit(msg)
+
+    def stop(self):
+        """Stop the track."""
+        msg = self._format_msg('mycroft.audio.service.stop')
+        self.bus.emit(msg)
+
+    def next(self):
+        """Change to next track."""
+        msg = self._format_msg('mycroft.audio.service.next')
+        self.bus.emit(msg)
+
+    def prev(self):
+        """Change to previous track."""
+        msg = self._format_msg('mycroft.audio.service.prev')
+        self.bus.emit(msg)
+
+    def pause(self):
+        """Pause playback."""
+        msg = self._format_msg('mycroft.audio.service.pause')
+        self.bus.emit(msg)
+
+    def resume(self):
+        """Resume paused playback."""
+        msg = self._format_msg('mycroft.audio.service.resume')
+        self.bus.emit(msg)
+
+    def get_track_length(self):
+        """
+        getting the duration of the audio in seconds
+        """
+        length = 0
+        msg = self._format_msg('mycroft.audio.service.get_track_length')
+        info = self.bus.wait_for_response(msg, timeout=1)
+        if info:
+            length = info.data.get("length", 0)
+        return length / 1000  # convert to seconds
+
+    def get_track_position(self):
+        """
+        get current position in seconds
+        """
+        pos = 0
+        msg = self._format_msg('mycroft.audio.service.get_track_position')
+        info = self.bus.wait_for_response(msg, timeout=1)
+        if info:
+            pos = info.data.get("position", 0)
+        return pos / 1000  # convert to seconds
+
+    def set_track_position(self, seconds):
+        """Seek X seconds.
+
+        Arguments:
+            seconds (int): number of seconds to seek, if negative rewind
+        """
+        msg = self._format_msg('mycroft.audio.service.set_track_position',
+                               {"position": seconds * 1000})  # convert to ms
+        self.bus.emit(msg)
+
+    def seek(self, seconds=1):
+        """Seek X seconds.
+
+        Args:
+            seconds (int): number of seconds to seek, if negative rewind
+        """
+        if isinstance(seconds, timedelta):
+            seconds = seconds.total_seconds()
+        if seconds < 0:
+            self.seek_backward(abs(seconds))
+        else:
+            self.seek_forward(seconds)
 
-    @property
-    def info(self) -> dict:
-        """
-        Return a dict representation of this MediaEntry + infocard for QML model
-        """
-        return merge_dict(self.as_dict, self.infocard)
+    def seek_forward(self, seconds=1):
+        """Skip ahead X seconds.
 
+        Args:
+            seconds (int): number of seconds to skip
+        """
+        if isinstance(seconds, timedelta):
+            seconds = seconds.total_seconds()
+        msg = self._format_msg('mycroft.audio.service.seek_forward',
+                               {"seconds": seconds})
+        self.bus.emit(msg)
 
-class NowPlaying(MediaEntry):
-    def __init__(self, *args, **kwargs):
-        MediaEntry.__init__(self, *args, **kwargs)
-        self._player = None
+    def seek_backward(self, seconds=1):
+        """Rewind X seconds
 
-    @property
-    def as_dict(self) -> dict:
+         Args:
+            seconds (int): number of seconds to rewind
         """
-        Return a dict reporesentation of this MediaEntry
-        """
-        return {k: v for k, v in self.__dict__.items()
-                if not k.startswith("_")}
+        if isinstance(seconds, timedelta):
+            seconds = seconds.total_seconds()
+        msg = self._format_msg('mycroft.audio.service.seek_backward',
+                               {"seconds": seconds})
+        self.bus.emit(msg)
 
-    @property
-    def bus(self) -> MessageBusClient:
-        """
-        Return the MessageBusClient inherited from the bound OCPMediaPlayer
-        """
-        return self._player.bus
+    def track_info(self):
+        """Request information of current playing track.
 
-    @property
-    def _settings(self) -> dict:
+        Returns:
+            Dict with track info.
         """
-        Return the dict settings inherited from the bound OCPMediaPlayer
-        """
-        return self._player.settings
+        msg = self._format_msg('mycroft.audio.service.track_info')
+        info = self.bus.wait_for_response(
+            msg, reply_type='mycroft.audio.service.track_info_reply',
+            timeout=1)
+        return info.data if info else {}
 
-    def as_entry(self) -> MediaEntry:
-        """
-        Return a MediaEntry representation of this object
+    def available_backends(self):
+        """Return available audio backends.
+
+        Returns:
+            dict with backend names as keys
         """
-        return MediaEntry.from_dict(self.as_dict)
+        msg = self._format_msg('mycroft.audio.service.list_backends')
+        response = self.bus.wait_for_response(msg)
+        return response.data if response else {}
+
+    @property
+    def is_playing(self):
+        """True if the audioservice is playing, else False."""
+        return self.track_info() != {}
+
+
+class MycroftCommonPlayInterface(OCPAbstractComponent):
+    """ interface for mycroft common play """
+
+    def __init__(self, player=None):
+        super().__init__(player)
+        self.query_replies = {}
+        self.query_extensions = {}
+        self.waiting = False
+        self.start_ts = 0
+        if player:
+            self.bind(player)
 
     def bind(self, player):
-        """
-        Bind an OCPMediaPlayer object to this NowPlaying instance. Registers
-        messagebus event handlers and defines `self._player`
-        @param player: OCPMediaPlayer instance to bind
-        """
-        # needs to start with _ to avoid json serialization errors
         self._player = player
-        self._player.add_event("ovos.common_play.track.state",
-                               self.handle_track_state_change)
-        self._player.add_event("ovos.common_play.media.state",
-                               self.handle_media_state_change)
-        self._player.add_event("ovos.common_play.play",
-                               self.handle_external_play)
-        self._player.add_event("ovos.common_play.playback_time",
-                               self.handle_sync_seekbar)
-        self._player.add_event('gui.player.media.service.get.meta',
-                               self.handle_player_metadata_request)
-        self._player.add_event('mycroft.audio.service.track_info_reply',
-                               self.handle_sync_trackinfo)
-        self._player.add_event('mycroft.audio.service.play',
-                               self.handle_audio_service_play)
-        self._player.add_event('mycroft.audio.playing_track',
-                               self.handle_audio_service_play_start)
-
-    def shutdown(self):
-        """
-        Remove NowPlaying events from the MessageBusClient
-        """
-        self._player.remove_event("ovos.common_play.track.state")
-        self._player.remove_event("ovos.common_play.playback_time")
-        self._player.remove_event('gui.player.media.service.get.meta')
-        self._player.remove_event('mycroft.audio_only.service.track_info_reply')
-
-    def reset(self):
-        """
-        Reset the NowPlaying MediaEntry to default parameters
-        """
-        LOG.debug("Resetting NowPlaying")
-        self.title = ""
-        self.artist = None
-        self.skill_icon = None
-        self.skill_id = None
-        self.position = 0
-        self.length = None
-        self.is_cps = False
-        self.cps_data = {}
-        self.data = {}
-        self.phrase = None
-        self.javascript = ""
-        self.playback = PlaybackType.UNDEFINED
-        self.status = TrackState.DISAMBIGUATION
-
-    def update(self, entry: Union[dict, MediaEntry], skipkeys: list = None, newonly: bool = False):
-        """
-        Update this MediaEntry and emit `gui.player.media.service.set.meta`
-        @param entry: dict or MediaEntry object to update this object with
-        @param skipkeys: list of keys to not change
-        @param newonly: if True, only adds new keys; existing keys are unchanged
-        """
-        if isinstance(entry, MediaEntry):
-            entry = entry.as_dict
-        super().update(entry, skipkeys, newonly)
-        # uri updates should not be skipped
-        if newonly and entry.get("uri"):
-            super().update({"uri": entry["uri"]})
-        # sync with gui media player on track change
-        if not self._player:
-            LOG.error("Instance not bound! Call `bind` before trying to use "
-                      "the messagebus.")
-            return
-        self.bus.emit(Message("gui.player.media.service.set.meta",
-                              {"title": self.title,
-                               "image": self.image,
-                               "artist": self.artist}))
-
-    def extract_stream(self):
-        """
-        Get metadata from ocp_plugins and add it to this MediaEntry
-        """
-        uri = self.uri
-        if not uri:
-            raise ValueError("No URI to extract stream from")
-        if self.playback == PlaybackType.VIDEO:
-            video = True
-        else:
-            video = False
-        meta = ocp_plugins().extract_stream(uri, video)
-        # update media entry with new data
-        if meta:
-            LOG.info(f"OCP plugins metadata: {meta}")
-            self.update(meta, newonly=True)
-        elif not any((uri.startswith(s) for s in ["http", "file", "/"])):
-            LOG.info(f"OCP WARNING: plugins returned no metadata for uri {uri}")
-
-    # events from gui_player/audio_service
-    def handle_external_play(self, message):
-        """
-        Handle 'ovos.common_play.play' Messages. Update the metadata with new
-        data received unconditionally, otherwise previous song keys might
-        bleed into the new track
-        @param message: Message associated with request
-        """
-        if message.data.get("tracks"):
-            # backwards compat / old style
-            playlist = message.data["tracks"]
-            media = playlist[0]
-        else:
-            media = message.data.get("media", {})
-        if media:
-            self.update(media, newonly=False)
-
-    def handle_player_metadata_request(self, message):
-        """
-        Handle 'gui.player.media.service.get.meta' Messages. Emit a response for
-        the GUI to handle new metadata.
-        @param message: Message associated with request
-        """
-        self.bus.emit(message.reply("gui.player.media.service.set.meta",
-                                    {"title": self.title,
-                                     "image": self.image,
-                                     "artist": self.artist}))
-
-    def handle_track_state_change(self, message):
-        """
-        Handle 'ovos.common_play.track.state' Messages. Update status
-        @param message: Message with updated `state` data
-        @return:
-        """
-        state = message.data.get("state")
-        if state is None:
-            raise ValueError(f"Got state update message with no state: "
-                             f"{message}")
-        if isinstance(state, int):
-            state = TrackState(state)
-        if not isinstance(state, TrackState):
-            raise ValueError(f"Expected int or TrackState, but got: {state}")
-
-        if state == self.status:
-            return
-        self.status = state
-        LOG.info(f"TrackState changed: {repr(state)}")
-
-        if state == TrackState.PLAYING_SKILL:
-            # skill is handling playback internally
-            pass
-        elif state == TrackState.PLAYING_AUDIOSERVICE:
-            # audio service is handling playback
-            pass
-        elif state == TrackState.PLAYING_VIDEO:
-            # ovos common play is handling playback in GUI
-            pass
-        elif state == TrackState.PLAYING_AUDIO:
-            # ovos common play is handling playback in GUI
-            pass
-
-        elif state == TrackState.DISAMBIGUATION:
-            # alternative results # TODO its this 1 track or a list ?
-            pass
-        elif state in [TrackState.QUEUED_SKILL,
-                       TrackState.QUEUED_VIDEO,
-                       TrackState.QUEUED_AUDIOSERVICE]:
-            # audio service is handling playback and this is in playlist
-            pass
-
-    def handle_media_state_change(self, message):
-        """
-        Handle 'ovos.common_play.media.state' Messages. If ended, reset.
-        @param message: Message with updated MediaState
-        """
-        state = message.data.get("state")
-        if state is None:
-            raise ValueError(f"Got state update message with no state: "
-                             f"{message}")
-        if isinstance(state, int):
-            state = MediaState(state)
-        if not isinstance(state, MediaState):
-            raise ValueError(f"Expected int or TrackState, but got: {state}")
-        # Don't do anything. Let OCP manage this object's state
-        # if state == MediaState.END_OF_MEDIA:
-        #     # playback ended, allow next track to change metadata again
-        #     self.reset()
-
-    def handle_sync_seekbar(self, message):
-        """
-        Handle 'ovos.common_play.playback_time' Messages sent by audio backend
-        @param message: Message with 'length' and 'position' data
-        """
-        self.length = message.data["length"]
-        self.position = message.data["position"]
-
-    def handle_sync_trackinfo(self, message):
-        """
-        Handle 'mycroft.audio.service.track_info_reply' Messages with current
-        media defined in message.data
-        @param message: Message with dict MediaEntry data
-        """
-        self.update(message.data)
-
-    def handle_audio_service_play(self, message):
-        """
-        Handle 'mycroft.audio.service.play' Messages with list of tracks in data
-        @param message: Message with 'tracks' data
-        """
-        tracks = message.data.get("tracks") or []
-        # only present in ovos-core
-        skill_id = message.context.get("skill_id") or 'mycroft.audio_interface'
-        for idx, track in enumerate(tracks):
-            # TODO try to extract metadata from uri (latency ?)
-            if idx == 0:
-                self.update(
-                    {"uri": track,
-                     "title": track.split("/")[-1],
-                     "status": TrackState.QUEUED_AUDIOSERVICE,
-                     'skill_id': skill_id,
-                     "playback": PlaybackType.AUDIO_SERVICE}
-                )
-            else:
-                # TODO sync playlist ?
-                pass
+        self.add_event("play:query.response",
+                       self.handle_cps_response)
 
-    def handle_audio_service_play_start(self, message):
-        """
-        Handle 'mycroft.audio.playing_track' Messages
-        @param message: Message notifying playback has started
-        """
-        self.update(
-            {"status": TrackState.PLAYING_AUDIOSERVICE,
-             "playback": PlaybackType.AUDIO_SERVICE})
+    @property
+    def cps_status(self):
+        return wait_for_reply('play:status.query',
+                              reply_type="play:status.response",
+                              bus=self.bus).data
+
+    def handle_cps_response(self, message):
+        search_phrase = message.data["phrase"]
+
+        if ("searching" in message.data and
+                search_phrase in self.query_extensions):
+            # Manage requests for time to complete searches
+            skill_id = message.data["skill_id"]
+            if message.data["searching"]:
+                # extend the timeout by N seconds
+                # IGNORED HERE, used in mycroft-playback-control skill
+                if skill_id not in self.query_extensions[search_phrase]:
+                    self.query_extensions[search_phrase].append(skill_id)
+            else:
+                # Search complete, don't wait on this skill any longer
+                if skill_id in self.query_extensions[search_phrase]:
+                    self.query_extensions[search_phrase].remove(skill_id)
+
+        elif search_phrase in self.query_replies:
+            # Collect all replies until the timeout
+            self.query_replies[message.data["phrase"]].append(message.data)
+
+            # forward response in OCP format
+            data = self.cps2ocp(message.data)
+            self.bus.emit(message.forward(
+                "ovos.common_play.query.response", data))
+
+    def send_query(self, phrase, media_type=MediaType.GENERIC):
+        self.query_replies[phrase] = []
+        self.query_extensions[phrase] = []
+        self.bus.emit(Message('play:query', {"phrase": phrase,
+                                             "question_type": media_type}))
+
+    def get_results(self, phrase):
+        if self.query_replies.get(phrase):
+            return self.query_replies[phrase]
+        return []
+
+    def search(self, phrase, media_type=MediaType.GENERIC,
+               timeout=5):
+        self.send_query(phrase, media_type)
+        self.waiting = True
+        start_ts = time.time()
+        while self.waiting and time.time() - start_ts <= timeout:
+            time.sleep(0.2)
+        self.waiting = False
+        return self.get_results(phrase)
+
+    @staticmethod
+    def cps2ocp(res, media_type=MediaType.GENERIC):
+        data = {
+            "playback": PlaybackType.SKILL,
+            "media_type": media_type,
+            "is_cps": True,
+            "cps_data": res['callback_data'],
+            "skill_id": res["skill_id"],
+            "phrase": res["phrase"],
+            'match_confidence': res["conf"] * 100,
+            "title": res["phrase"],
+            "artist": res["skill_id"]
+        }
+        return {'phrase': res["phrase"],
+                "is_old_style": True,
+                'results': [data],
+                'searching': False,
+                'skill_id': res["skill_id"]}
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/mpris.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/mpris.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dbus_next.aio import MessageBus as DbusMessageBus
 from dbus_next.constants import BusType
 from dbus_next.message import Message as DbusMessage, \
     MessageType as DbusMessageType
 from dbus_next.service import ServiceInterface, method, dbus_property, PropertyAccess
 from ovos_bus_client.message import Message
 from ovos_utils.log import LOG
-from ovos_utils.ocp import TrackState, PlaybackType, PlayerState, LoopState
+from ovos_workshop.decorators.ocp import TrackState, PlaybackType, PlayerState, LoopState
 
 
 class MprisPlayerCtl(Thread):
     """ detects other media players in the system and integrates with them
     - stop internal playback when an external player starts
     - display gui with data from external media player
     - provide voice control over the external player
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/player.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import random
 from os.path import join, dirname
 from time import sleep
 from typing import List, Union
 
 from ovos_bus_client.message import Message
-
 from ovos_config import Configuration
-from ovos_plugin_common_play.ocp.gui import OCPMediaPlayerGUI
-from ovos_plugin_common_play.ocp.media import NowPlaying
-from ovos_plugin_common_play.ocp.mpris import MprisPlayerCtl
-from ovos_plugin_common_play.ocp.mycroft_cps import MycroftAudioService
-from ovos_plugin_common_play.ocp.search import OCPSearch
 from ovos_utils.gui import is_gui_connected, is_gui_running
 from ovos_utils.log import LOG
 from ovos_utils.messagebus import Message
-from ovos_utils.ocp import OCP_ID, Playlist, LoopState, MediaState, PlayerState, TrackState, PlaybackType, PlaybackMode, \
-    MediaEntry
 from ovos_workshop import OVOSAbstractApplication
+from ovos_workshop.decorators.ocp import LoopState, MediaState, PlayerState, TrackState, PlaybackType, PlaybackMode
+
+from ovos_plugin_common_play.ocp.constants import OCP_ID
+from ovos_plugin_common_play.ocp.gui import OCPMediaPlayerGUI
+from ovos_plugin_common_play.ocp.media import NowPlaying, Playlist, MediaEntry, _ME
+from ovos_plugin_common_play.ocp.mpris import MprisPlayerCtl
+from ovos_plugin_common_play.ocp.mycroft_cps import MycroftAudioService
+from ovos_plugin_common_play.ocp.search import OCPSearch
 
 try:
     from ovos_utils.ocp import dict2entry
 except ImportError:  # older utils version
     dict2entry = MediaEntry.from_dict
 
 
@@ -242,18 +242,18 @@
         notify any GUI or MPRIS clients. Adds `track` to `playlist`
         @param track: MediaEntry or dict representation of a MediaEntry to play
         """
         LOG.debug(f"Playing: {track}")
         if isinstance(track, dict):
             LOG.debug("Handling dict track")
             track = dict2entry(track)
-        if not isinstance(track, (MediaEntry, Playlist)):
+        if not isinstance(track, (_ME, Playlist)):
             raise ValueError(f"Expected MediaEntry/Playlist, but got: {track}")
         self.now_playing.reset()  # reset now_playing to remove old metadata
-        if isinstance(track, MediaEntry):
+        if isinstance(track, _ME):
             # single track entry (MediaEntry)
             self.now_playing.update(track)
             # copy now_playing (without event handlers) to playlist
             # entry = self.now_playing.as_entry()
             if track not in self.playlist:  # compared by uri
                 self.playlist.add_entry(track)
         elif isinstance(track, Playlist):
@@ -323,15 +323,15 @@
         Start playing the requested media, replacing any current playback.
         @param track: dict or MediaEntry to start playing
         @param disambiguation: list of tracks returned from search
         @param playlist: list of tracks in the current playlist
         """
         if isinstance(track, dict):
             track = dict2entry(track)
-        if not isinstance(track, (MediaEntry, Playlist)):
+        if not isinstance(track, (_ME, Playlist)):
             raise TypeError(f"Expected MediaEntry/Playlist, got: {track}")
         if isinstance(track, Playlist) and not playlist:
             playlist = track
             track = playlist[0]
         if self.mpris:
             self.mpris.stop()
         if self.state == PlayerState.PLAYING:
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/desktop/OCP.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/desktop/OCP.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ca-es/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/cs-cz/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/da-dk/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/pause.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/de-de/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/en-us/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/behind_scenes.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/es-es/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/fr-fr/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/hu-hu/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/nl-nl/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pl-pl/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/pt-pt/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/behind_scenes.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/documentaries.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/setup.hints.dialog`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/short_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/silent_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/ru-ru/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-fi/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/movietrailer.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/play.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/sv-se/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Music.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Next.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Play.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/Prev.voc`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/audiobook.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/bw_movie.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/comic.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/featured.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/hentai.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/next.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/open.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/podcast.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/prev.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/radio.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/resume.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/locale/tr-tr/tv.intent`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/AudioPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Disambiguation.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Home.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/NowPlayingHomeBar.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OCPSkillsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSAudioPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSeekControlQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSSyncPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSVideoPlayerQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/OVOSWebPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/PlayerLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Playlist.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/Search.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SpectrumWaveDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/SuggestionsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/+mediacenter/VideoPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/AudioPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigDelegateLayoutItem.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigSliderDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/ConfigSwitchDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Disambiguation.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/GenericCloseControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Home.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Home.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/NowPlayingHomeBar.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OCPSkillsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSAudioPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSeekControlQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSSyncPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSVideoPlayerQtAv.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/OVOSWebPlayer.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/PlayerLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Playlist.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Playlist.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/Search.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/Search.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/SpectrumWaveDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/SuggestionsView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/VideoPlayerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/code/nav.js` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/code/nav.js`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/delegates/GridSkillCard.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/back.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/back.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/back.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/back.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/history.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/history.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/home.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/home.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/information.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/information.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-album-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-mute.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-next.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-pause.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-play.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-play.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-repeat.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-playlist-shuffle.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-previous.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-playlist.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat-track.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-repeat.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-stop.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/media-unmute.svg`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-dark.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp-light.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/ocp_bg.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/search.png` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/search.png`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/qmldir` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/qmldir`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/GridTileView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/res/ui/views/TileView.qml`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/search.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import random
 import time
 from os.path import join, isfile
 from threading import RLock, Lock
 from typing import List
 
+from ovos_bus_client.message import Message
+from ovos_bus_client.util import get_mycroft_bus
 from ovos_config.locations import get_xdg_config_save_path
+from ovos_plugin_manager.ocp import available_extractors
 from ovos_utils.gui import is_gui_connected, is_gui_running
 from ovos_utils.log import LOG
-from ovos_bus_client.message import Message
-from ovos_bus_client.util import get_mycroft_bus
+from ovos_workshop.decorators.ocp import MediaType, PlaybackType, PlaybackMode
 
 from ovos_plugin_common_play.ocp.base import OCPAbstractComponent
+from ovos_plugin_common_play.ocp.constants import OCP_ID
 from ovos_plugin_common_play.ocp.media import Playlist
-from ovos_utils.ocp import OCP_ID, MediaType, TrackState, PlaybackType, PlaybackMode
-from ovos_plugin_manager.ocp import available_extractors
 
 
 class OCPQuery:
     cast2audio = [
         MediaType.MUSIC,
         MediaType.PODCAST,
         MediaType.AUDIOBOOK,
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play/ocp/utils.py` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play/ocp/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import shutil
 from os import makedirs
 from os.path import expanduser, isfile, join, dirname, exists
-from typing import List
 
-from ovos_ocp_files_plugin.plugin import OCPFilesMetadataExtractor
 from ovos_plugin_manager.ocp import load_stream_extractors, available_extractors
 
 
 def ocp_plugins():
     return load_stream_extractors()
 
 
@@ -15,14 +13,15 @@
     return exists("/usr/include/qt/QtAV") or \
         exists("/usr/lib/qt/qml/QtAV") or \
         exists("/usr/lib/libQtAV.so")
 
 
 def extract_metadata(uri):
     # backwards compat
+    from ovos_ocp_files_plugin.plugin import OCPFilesMetadataExtractor
     return OCPFilesMetadataExtractor.extract_metadata(uri)
 
 
 def create_desktop_file():
     res = join(dirname(__file__), "res", "desktop")
     desktop_path = expanduser("~/.local/share/applications")
     icon_path = expanduser("~/.local/share/icons")
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/PKG-INFO` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-plugin-common-play
-Version: 0.0.7a6
+Version: 0.0.7a7
 Summary: OVOS common play audio service adapter plugin
 Home-page: https://github.com/OpenVoiceOS/ovos-ocp-audio-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: ovos audio plugin
 Platform: UNKNOWN
```

### Comparing `ovos_plugin_common_play-0.0.7a6/ovos_plugin_common_play.egg-info/SOURCES.txt` & `ovos_plugin_common_play-0.0.7a7/ovos_plugin_common_play.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos_plugin_common_play-0.0.7a6/setup.py` & `ovos_plugin_common_play-0.0.7a7/setup.py`

 * *Files identical despite different names*

