# Comparing `tmp/songfinder-1.0.0-py3-none-any.whl.zip` & `tmp/songfinder-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 235081 bytes, number of entries: 69
+Zip file size: 235372 bytes, number of entries: 70
 -rw-r--r--  2.0 unx     9856 b- defN 20-Feb-02 00:00 songfinder/__init__.py
+-rw-r--r--  2.0 unx      163 b- defN 20-Feb-02 00:00 songfinder/__main__.py
 -rw-r--r--  2.0 unx     8455 b- defN 20-Feb-02 00:00 songfinder/accords.py
 -rw-r--r--  2.0 unx     5023 b- defN 20-Feb-02 00:00 songfinder/background.py
 -rw-r--r--  2.0 unx     1103 b- defN 20-Feb-02 00:00 songfinder/cache.py
 -rw-r--r--  2.0 unx     5159 b- defN 20-Feb-02 00:00 songfinder/classDiapo.py
 -rw-r--r--  2.0 unx     4806 b- defN 20-Feb-02 00:00 songfinder/classPaths.py
 -rw-r--r--  2.0 unx     8131 b- defN 20-Feb-02 00:00 songfinder/classSet.py
 -rw-r--r--  2.0 unx    16797 b- defN 20-Feb-02 00:00 songfinder/classSettings.py
@@ -49,23 +50,23 @@
 -rw-r--r--  2.0 unx     3518 b- defN 20-Feb-02 00:00 songfinder/elements/passage.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 songfinder/gui/__init__.py
 -rw-r--r--  2.0 unx     1991 b- defN 20-Feb-02 00:00 songfinder/gui/diapoListGui.py
 -rw-r--r--  2.0 unx    17057 b- defN 20-Feb-02 00:00 songfinder/gui/editGui.py
 -rw-r--r--  2.0 unx     5056 b- defN 20-Feb-02 00:00 songfinder/gui/fullScreenPresent.py
 -rw-r--r--  2.0 unx     3129 b- defN 20-Feb-02 00:00 songfinder/gui/guiHelper.py
 -rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 songfinder/gui/inputFrame.py
--rw-r--r--  2.0 unx    19535 b- defN 20-Feb-02 00:00 songfinder/gui/interface.py
+-rw-r--r--  2.0 unx    19545 b- defN 20-Feb-02 00:00 songfinder/gui/interface.py
 -rw-r--r--  2.0 unx    25485 b- defN 20-Feb-02 00:00 songfinder/gui/preferences.py
 -rw-r--r--  2.0 unx     4696 b- defN 20-Feb-02 00:00 songfinder/gui/presentGui.py
 -rw-r--r--  2.0 unx    20022 b- defN 20-Feb-02 00:00 songfinder/gui/screen.py
 -rw-r--r--  2.0 unx    12192 b- defN 20-Feb-02 00:00 songfinder/gui/searchGui.py
 -rw-r--r--  2.0 unx    18203 b- defN 20-Feb-02 00:00 songfinder/gui/selectionListGui.py
 -rw-r--r--  2.0 unx     7366 b- defN 20-Feb-02 00:00 songfinder/gui/simpleProgress.py
 -rw-r--r--  2.0 unx     3297 b- defN 20-Feb-02 00:00 songfinder/gui/splash.py
 -rw-r--r--  2.0 unx     3288 b- defN 20-Feb-02 00:00 songfinder/gui/themes.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 songfinder/lib/__init__.py
 -rw-r--r--  2.0 unx     3100 b- defN 20-Feb-02 00:00 songfinder/data/documentation/README.md
-?rw-r--r--  2.0 unx     3975 b- defN 20-Feb-02 00:00 songfinder-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 songfinder-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      111 b- defN 20-Feb-02 00:00 songfinder-1.0.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     5899 b- defN 20-Feb-02 00:00 songfinder-1.0.0.dist-info/RECORD
-69 files, 576457 bytes uncompressed, 225777 bytes compressed:  60.8%
+?rw-r--r--  2.0 unx     3975 b- defN 20-Feb-02 00:00 songfinder-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 songfinder-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      111 b- defN 20-Feb-02 00:00 songfinder-1.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     5977 b- defN 20-Feb-02 00:00 songfinder-1.0.1.dist-info/RECORD
+70 files, 576708 bytes uncompressed, 225948 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: songfinder/__init__.py
 Comment: 
 
+Filename: songfinder/__main__.py
+Comment: 
+
 Filename: songfinder/accords.py
 Comment: 
 
 Filename: songfinder/background.py
 Comment: 
 
 Filename: songfinder/cache.py
@@ -189,20 +192,20 @@
 
 Filename: songfinder/lib/__init__.py
 Comment: 
 
 Filename: songfinder/data/documentation/README.md
 Comment: 
 
-Filename: songfinder-1.0.0.dist-info/METADATA
+Filename: songfinder-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: songfinder-1.0.0.dist-info/WHEEL
+Filename: songfinder-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: songfinder-1.0.0.dist-info/entry_points.txt
+Filename: songfinder-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: songfinder-1.0.0.dist-info/RECORD
+Filename: songfinder-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## songfinder/__init__.py

```diff
@@ -5,15 +5,15 @@
 import errno
 import sys
 import platform
 import logging
 import datetime
 from songfinder import logger_formatter
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "danbei"
 __appName__ = "songfinder"
 
 # Define root diretcory
 __chemin_root__ = os.getcwd()
 
 # Define data directory
```

## songfinder/gui/interface.py

```diff
@@ -491,15 +491,15 @@
         else:
             job = simpleProgress.UpdateJob(
                 function=pip.run,
                 options=[
                     "-m",
                     "pip",
                     "install",
-                    songfinder.__appName__,
+                    f"{songfinder.__appName__}[gui]",
                     "--upgrade",
                     "--user",
                 ],
                 timeOut=120,
             )
             progressBar = simpleProgress.Progress(
                 "Mise à jour de SongFinder", job, screens=self._screens
```

## Comparing `songfinder-1.0.0.dist-info/METADATA` & `songfinder-1.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: songfinder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Slide creation and presentation
 Author-email: Danbei <jean_raul@hotmail.fr>
 Requires-Python: >=3.6
 Requires-Dist: beautifulsoup4
 Requires-Dist: cython
 Requires-Dist: lxml
 Requires-Dist: markdown
```

## Comparing `songfinder-1.0.0.dist-info/RECORD` & `songfinder-1.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-songfinder/__init__.py,sha256=DxGPdkXrGwn1PeeY4WDmsJ0r49vFlEkNkCiuL36qUcs,9856
+songfinder/__init__.py,sha256=NUxikg2LytwSLF_l4Sdj5hGwTAKpCwEEq3iOzmJiXWc,9856
+songfinder/__main__.py,sha256=fOY9Hvo9z1kh2ImqVXL-G9aaZ69ws5WgYg8BWtGgqBg,163
 songfinder/accords.py,sha256=ZGR_pD3kIowC8NhrHtU5M0odyviBv0kH1A_Oh2c6h28,8455
 songfinder/background.py,sha256=LH0HRm-rP4QdBeQvLwaHTtL9zrT4vcNV9WWaBF_4Sjw,5023
 songfinder/cache.py,sha256=WdPaEvLlgcUZVuhU4FvZqbW3Lp8YxANL_hrmHqW0mY4,1103
 songfinder/classDiapo.py,sha256=pLyfDKvzNEzzGlUi9YuxtNErDsxzrND-K6iHx7ayJmI,5159
 songfinder/classPaths.py,sha256=DMFk_Q3SPVXeMVax-9o7ujuMV_GTN7HT6xZy_zGHNYc,4806
 songfinder/classSet.py,sha256=3LG-M27cGFQGG-6WvFORWsCrSqQWeY9H3GUL64wI-po,8131
 songfinder/classSettings.py,sha256=hUkdvy7XIDj3SpH78csVP8i4xfh0mGm0XAP-GtL9qTI,16797
@@ -48,22 +49,22 @@
 songfinder/elements/passage.py,sha256=Iai7tCtAubqnqpNJsx3YN867HwH3mN6CMS8Q8JhCsQ0,3518
 songfinder/gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 songfinder/gui/diapoListGui.py,sha256=NlRHc2NEZ5oVO-1MpBskpymmmFRicHQLHT1nbXf_Ffc,1991
 songfinder/gui/editGui.py,sha256=WYwGLUDcAndpcqkbF63ML6zufSJfZHNdlOn3lPMfjnE,17057
 songfinder/gui/fullScreenPresent.py,sha256=EOhc_CHzJ7j8FWTfBxvjg1-WR3l6XXZyuMJL2RjXCG4,5056
 songfinder/gui/guiHelper.py,sha256=EiqWG-l5uI044kYTLEvdhBWHJt7cauTEWJfnQt6FfCk,3129
 songfinder/gui/inputFrame.py,sha256=q-UBKfMy1fQIGkmr891OSIWVyMD66w7Iwo2sjaiIMUk,2369
-songfinder/gui/interface.py,sha256=PijrhUCSn1sv5KnBd-sIrZVMGrrfXnpjrFtJxbjCb1c,19535
+songfinder/gui/interface.py,sha256=3Seaf3kXtVQ8Q9n1lVnYIdV1ivb1i9o6aJ30PURPYMA,19545
 songfinder/gui/preferences.py,sha256=SVJlJA0J_GuLNYM59seY_Y_VbFMqSkHM0j6lKgUmdl8,25485
 songfinder/gui/presentGui.py,sha256=itF2I1VMalaARcNsC__6xQI3TMiSNnNwmrm1GROiuDs,4696
 songfinder/gui/screen.py,sha256=Haa-VmL2IJy53QCqUbhmDJISHDGS7ynOCZzs4cLoWbE,20022
 songfinder/gui/searchGui.py,sha256=EzxMZ09OAAM2R57G3Gwu_aVvtqmHi3bLENti9ENiel0,12192
 songfinder/gui/selectionListGui.py,sha256=Jbk8BDEMTCfqiNsl3lXvWgcOrXPP4osXDOlUovG0hUM,18203
 songfinder/gui/simpleProgress.py,sha256=FlNeLb34bwgaNrv4i7dJAG0IhNoKI3qq2XwWrOdog-0,7366
 songfinder/gui/splash.py,sha256=BK-qKcTaAeCrW4GAI5tTZ2ND0czVDfj07oAsKNbhfxQ,3297
 songfinder/gui/themes.py,sha256=aFLaunu6XzlcoFijepzN6gO2grPW54vKxCDltIuaP2o,3288
 songfinder/lib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 songfinder/data/documentation/README.md,sha256=YMF3jvzvUegosLU7mjSKzqYUQso7f-zo0R1IFsVa4gA,3100
-songfinder-1.0.0.dist-info/METADATA,sha256=8HZTSiCoPZoBgXnUlPIflE6bYJammJeY5FN4OupOnqY,3975
-songfinder-1.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-songfinder-1.0.0.dist-info/entry_points.txt,sha256=FzR4NZvrNoDXj7ysc3VrTXm9SGJ8Ad-aZsyn6tZOapE,111
-songfinder-1.0.0.dist-info/RECORD,,
+songfinder-1.0.1.dist-info/METADATA,sha256=FJcNxN8eDDLkQ4rK1zcgrXdiXM7DYFmMrG17Cjz7r0s,3975
+songfinder-1.0.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+songfinder-1.0.1.dist-info/entry_points.txt,sha256=FzR4NZvrNoDXj7ysc3VrTXm9SGJ8Ad-aZsyn6tZOapE,111
+songfinder-1.0.1.dist-info/RECORD,,
```

