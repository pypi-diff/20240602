# Comparing `tmp/python_datapack-0.2.2.tar.gz` & `tmp/python_datapack-0.2.3.tar.gz`

## Comparing `python_datapack-0.2.2.tar` & `python_datapack-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.2/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.2/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.2/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.2/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.2/copy_in_local.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item.png
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item_release.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.2/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.2/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.3/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.3/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.3/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.3/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.3/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/invisible_item.png
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/invisible_item_release.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.3/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.3/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.3/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.3/PKG-INFO
```

### Comparing `python_datapack-0.2.2/src/python_datapack/__init__.py` & `python_datapack-0.2.3/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/constants.py` & `python_datapack-0.2.3/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/enhance_config.py` & `python_datapack-0.2.3/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/finalyze.py` & `python_datapack-0.2.3/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/initialize.py` & `python_datapack-0.2.3/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/verify_database.py` & `python_datapack-0.2.3/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.2.3/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.2.3/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/headers.py` & `python_datapack-0.2.3/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/lang.py` & `python_datapack-0.2.3/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/loading.py` & `python_datapack-0.2.3/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.2.3/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/main.py` & `python_datapack-0.2.3/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/datapack/recipes.py` & `python_datapack-0.2.3/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.2.3/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/main.py` & `python_datapack-0.2.3/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/shared_import.py` & `python_datapack-0.2.3/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/utils.py` & `python_datapack-0.2.3/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/invisible_item.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item_release.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/invisible_item_release.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.2.3/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.2.3/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.2.3/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.2.3/src/python_datapack/resource_pack/item_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 		# Copy used textures
 		if content.get("textures"):
 			for texture in content["textures"].values():
 				texture_path = "/".join(texture.split(":")[-1].split("/")[1:])
 				source = f"{config['textures_folder']}/{texture_path}.png"
 				destination = f"{dest_base_textu}/{texture_path}.png"
 				super_copy(source, destination)
+				if os.path.exists(source + ".mcmeta"):
+					super_copy(source + ".mcmeta", destination + ".mcmeta")
 			
 		# Write content
 		write_to_file(f"{dest_base_model}/{item}{on_off}.json", super_json_dump(content, max_level = 4))
 
 
 
 def main(config: dict):
```

### Comparing `python_datapack-0.2.2/src/python_datapack/resource_pack/main.py` & `python_datapack-0.2.3/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.2.3/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.2.3/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/database_helper.py` & `python_datapack-0.2.3/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/ingredients.py` & `python_datapack-0.2.3/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/io.py` & `python_datapack-0.2.3/src/python_datapack/utils/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -116,28 +116,43 @@
 	return new_dict
 
 # The majority of files will be written at the end of the program to prevent excessive disk access (reading + appending + writing)
 FILES_TO_WRITE: dict[str, str] = {}
 def is_in_write_queue(file_path: str) -> bool:
 	return file_path.replace("\\", "/") in FILES_TO_WRITE
 
+def sort_override_model(json_content: dict) -> None:
+	for key, value in json_content.items():
+		if key == "overrides" \
+			and isinstance(value, list) and len(value) > 1 \
+			and all(isinstance(x, dict) \
+				and x.get("predicate") \
+				and isinstance(x["predicate"], dict) \
+				and x["predicate"].get("custom_model_data") is not None \
+				and isinstance(x["predicate"]["custom_model_data"], int) \
+				for x in value
+			):
+				json_content["overrides"] = sorted(value, key=lambda x: x["predicate"]["custom_model_data"])
+
 def write_to_file(file_path: str, content: str, overwrite: bool = False):
 
 	# Clean path
 	file_path = file_path.replace("\\", "/")
 
 	# If file doesn't exists or overwrite is true, made it empty
 	if file_path not in FILES_TO_WRITE or overwrite:
 		FILES_TO_WRITE[file_path] = ""
 	
 	# If the file already exists as JSON and the content is a dict, merge both dict
 	if not overwrite and file_path in FILES_TO_WRITE and file_path.endswith(".json") and FILES_TO_WRITE[file_path] != "":
 		dict_content = json.loads(content)
 		old_content = json.loads(FILES_TO_WRITE[file_path])
-		FILES_TO_WRITE[file_path] = super_json_dump(super_merge_dict(old_content, dict_content))
+		merged = super_merge_dict(old_content, dict_content)
+		sort_override_model(merged)
+		FILES_TO_WRITE[file_path] = super_json_dump(merged)
 		return
 	
 	# Add the content to the file
 	FILES_TO_WRITE[file_path] += str(content)
 
 def write_all_files(contains: str = ""):
 	contains = contains.replace("\\", "/")
```

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.2.3/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/print.py` & `python_datapack-0.2.3/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/src/python_datapack/utils/weld.py` & `python_datapack-0.2.3/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/LICENSE` & `python_datapack-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.2/pyproject.toml` & `python_datapack-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.2.2/PKG-INFO` & `python_datapack-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

