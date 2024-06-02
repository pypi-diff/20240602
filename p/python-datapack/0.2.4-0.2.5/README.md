# Comparing `tmp/python_datapack-0.2.4.tar.gz` & `tmp/python_datapack-0.2.5.tar.gz`

## Comparing `python_datapack-0.2.4.tar` & `python_datapack-0.2.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.4/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.4/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.4/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.4/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.4/copy_in_local.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/invisible_item.png
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/invisible_item_release.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/custom_block_ticks.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.4/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.4/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.4/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.4/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.5/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.5/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.5/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.5/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.5/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/custom_block_ticks.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/invisible_item.png
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/invisible_item_release.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.5/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.5/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.5/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.5/PKG-INFO
```

### Comparing `python_datapack-0.2.4/src/python_datapack/__init__.py` & `python_datapack-0.2.5/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/constants.py` & `python_datapack-0.2.5/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/enhance_config.py` & `python_datapack-0.2.5/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/finalyze.py` & `python_datapack-0.2.5/src/python_datapack/finalyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 # Imports
 from .utils.io import *
 from .utils.print import *
 from .utils.weld import weld_datapack, weld_resource_pack
 from .datapack.lang import main as lang_main
 from .datapack.headers import main as headers_main
+from .datapack.custom_block_ticks import custom_blocks_ticks_and_second_functions
 from .resource_pack.check_unused_textures import main as check_unused_textures_main
 import shutil
 
 def main(config: dict, user_code: callable):
 
 	# For every file in the merge folder, copy it to the build folder (with append content)
 	print()
@@ -43,14 +44,17 @@
 				else:
 					super_copy(merge_path, build_path)
 	info(f"All content in the '{config['merge_folder']}' folder copied to '{config['build_folder']}'")
 
 	# Run user code
 	if user_code:
 		user_code(config)
+	
+	# Second and tick functions for custom blocks
+	custom_blocks_ticks_and_second_functions(config)
 
 	# Generate lang file
 	if config['enable_translations']:
 		lang_main(config)
 
 	# Add a small header for each .mcfunction file
 	headers_main(config)
```

### Comparing `python_datapack-0.2.4/src/python_datapack/initialize.py` & `python_datapack-0.2.5/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/verify_database.py` & `python_datapack-0.2.5/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.2.5/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.2.5/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/headers.py` & `python_datapack-0.2.5/src/python_datapack/datapack/headers.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/lang.py` & `python_datapack-0.2.5/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/loading.py` & `python_datapack-0.2.5/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.2.5/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/main.py` & `python_datapack-0.2.5/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/datapack/recipes.py` & `python_datapack-0.2.5/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.2.5/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/main.py` & `python_datapack-0.2.5/src/python_datapack/manual/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/shared_import.py` & `python_datapack-0.2.5/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/utils.py` & `python_datapack-0.2.5/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/invisible_item.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/invisible_item.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/invisible_item_release.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/invisible_item_release.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.2.5/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.2.5/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.2.5/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.2.5/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/resource_pack/main.py` & `python_datapack-0.2.5/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.2.5/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.2.5/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/custom_block_ticks.py` & `python_datapack-0.2.5/src/python_datapack/datapack/custom_block_ticks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 
 # Imports
-from .print import *
-from .io import *
+from ..utils.print import *
+from ..utils.io import *
 
 # Setup custom blocks ticks and second functions calls
 def custom_blocks_ticks_and_second_functions(config: dict) -> None:
 	""" Setup custom blocks ticks and second functions calls\n
 	It will seek for "second.mcfunction" and "tick.mcfunction" files in the custom_blocks folder\n
 	Then it will generate all functions to lead to the execution of these files by adding tags\n
 	Args:
 		config (dict): The config dictionary\n
 	"""
-	database: dict[str, dict] = config['database']
 	namespace: str = config['namespace']
 	build_datapack: str = config['build_datapack']
 	custom_blocks = f"{build_datapack}/data/{namespace}/function/custom_blocks/"
 	
 	# Get second and ticks functions
 	custom_blocks_second = []
 	custom_blocks_tick = []
@@ -35,17 +34,17 @@
 	for custom_block in custom_blocks_second:
 		write_to_file(f"{custom_blocks}{custom_block}/place_secondary.mcfunction", f"\n# Add tag for loop every second\ntag @s add {namespace}.second")
 	for custom_block in custom_blocks_tick:
 		write_to_file(f"{custom_blocks}{custom_block}/place_secondary.mcfunction", f"\n# Add tag for loop every tick\ntag @s add {namespace}.tick")
 	
 	# Write second functions
 	if custom_blocks_second:
-		write_to_file(f"{build_datapack}/data/{namespace}/function/second.mcfunction", f"\n# Custom blocks second functions\nexecute as @e[tag={namespace}.second] run function {namespace}:custom_blocks/second")
+		write_to_file(f"{build_datapack}/data/{namespace}/function/second.mcfunction", f"\n# Custom blocks second functions\nexecute as @e[tag={namespace}.second] at @s run function {namespace}:custom_blocks/second")
 		content = "\n".join(f"execute if entity @s[tag={namespace}.{custom_block}] run function {namespace}:custom_blocks/{custom_block}/second" for custom_block in custom_blocks_second)
 		write_to_file(f"{build_datapack}/data/{namespace}/function/custom_blocks/second.mcfunction", content)
 	
 	# Write tick functions
 	if custom_blocks_tick:
-		write_to_file(f"{build_datapack}/data/{namespace}/function/tick.mcfunction", f"\n# Custom blocks tick functions\nexecute as @e[tag={namespace}.tick] run function {namespace}:custom_blocks/tick")
+		write_to_file(f"{build_datapack}/data/{namespace}/function/tick.mcfunction", f"\n# Custom blocks tick functions\nexecute as @e[tag={namespace}.tick] at @s run function {namespace}:custom_blocks/tick")
 		content = "\n".join(f"execute if entity @s[tag={namespace}.{custom_block}] run function {namespace}:custom_blocks/{custom_block}/tick" for custom_block in custom_blocks_tick)
 		write_to_file(f"{build_datapack}/data/{namespace}/function/custom_blocks/tick.mcfunction", content)
```

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/database_helper.py` & `python_datapack-0.2.5/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/ingredients.py` & `python_datapack-0.2.5/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/io.py` & `python_datapack-0.2.5/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.2.5/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/print.py` & `python_datapack-0.2.5/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/src/python_datapack/utils/weld.py` & `python_datapack-0.2.5/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/LICENSE` & `python_datapack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.4/pyproject.toml` & `python_datapack-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.2.4/PKG-INFO` & `python_datapack-0.2.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

