# Comparing `tmp/python_datapack-0.2.1.tar.gz` & `tmp/python_datapack-0.2.2.tar.gz`

## Comparing `python_datapack-0.2.1.tar` & `python_datapack-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.1/1_upgrades.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.1/2_build.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.1/3_upload.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.1/build_all_in_one.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.1/copy_in_local.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/constants.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/enhance_config.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/finalyze.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/initialize.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/verify_database.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/basic_structure.py
--rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/custom_blocks.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/headers.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/lang.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/loading.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/loot_tables.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/main.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/datapack/recipes.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/book_optimizer.py
--rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/main.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/shared_import.py
--rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/utils.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/furnace.png
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item.png
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item_release.png
--rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/minecraft_font.ttf
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/none.png
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/none_release.png
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_2x2.png
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_3x3.png
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/simple_case_no_border.png
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_information.png
--rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
--rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_result_of_craft.png
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/check_unused_textures.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/item_models.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/main.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/sounds.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/resource_pack/vanilla_models.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/cache.py
--rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/database_helper.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/ingredients.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/io.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/multiprocessing.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/print.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.1/src/python_datapack/utils/weld.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.1/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.1/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.2/1_upgrades.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 python_datapack-0.2.2/2_build.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 python_datapack-0.2.2/3_upload.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 python_datapack-0.2.2/build_all_in_one.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 python_datapack-0.2.2/copy_in_local.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/constants.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/enhance_config.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/finalyze.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/initialize.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/verify_database.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/basic_structure.py
+-rw-r--r--   0        0        0    15298 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/custom_blocks.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/headers.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/lang.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/loading.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/loot_tables.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/main.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/datapack/recipes.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/book_optimizer.py
+-rw-r--r--   0        0        0    23803 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/main.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/shared_import.py
+-rw-r--r--   0        0        0    30296 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/utils.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/furnace.png
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item.png
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item_release.png
+-rw-r--r--   0        0        0    42432 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/minecraft_font.ttf
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/none.png
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/none_release.png
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_2x2.png
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_3x3.png
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/simple_case_no_border.png
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_information.png
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png
+-rw-r--r--   0        0        0    16198 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_result_of_craft.png
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/check_unused_textures.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/item_models.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/main.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/sounds.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/resource_pack/vanilla_models.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/cache.py
+-rw-r--r--   0        0        0    28462 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/database_helper.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/ingredients.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/io.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/multiprocessing.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/print.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 python_datapack-0.2.2/src/python_datapack/utils/weld.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 python_datapack-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 python_datapack-0.2.2/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 python_datapack-0.2.2/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 python_datapack-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 python_datapack-0.2.2/PKG-INFO
```

### Comparing `python_datapack-0.2.1/src/python_datapack/__init__.py` & `python_datapack-0.2.2/src/python_datapack/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/constants.py` & `python_datapack-0.2.2/src/python_datapack/constants.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/enhance_config.py` & `python_datapack-0.2.2/src/python_datapack/enhance_config.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/finalyze.py` & `python_datapack-0.2.2/src/python_datapack/finalyze.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/initialize.py` & `python_datapack-0.2.2/src/python_datapack/initialize.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/verify_database.py` & `python_datapack-0.2.2/src/python_datapack/verify_database.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/basic_structure.py` & `python_datapack-0.2.2/src/python_datapack/datapack/basic_structure.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/custom_blocks.py` & `python_datapack-0.2.2/src/python_datapack/datapack/custom_blocks.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/headers.py` & `python_datapack-0.2.2/src/python_datapack/datapack/headers.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,33 +20,51 @@
 			to_be_called = f"{config['namespace']}:" + splitted[1].replace(".mcfunction","")
 			
 			# Add to mcfunctions dictionary
 			mcfunctions[to_be_called] = {"path": file_path, "within": []}
 
 	# For each json file, get the functions that it calls
 	functions_tags_folder = "/tags/function/"
+	advancements_folder = "/advancement/"
 	for file_path in FILES_TO_WRITE:
-		if functions_tags_folder in file_path and file_path.endswith(".json"):
+		if file_path.endswith(".json"):
+			if functions_tags_folder in file_path:
 
-			# Get namespace of the file
-			splitted = file_path.split(functions_tags_folder)
-			namespace = splitted[0].split("/")[-1]
+				# Get namespace of the file
+				splitted = file_path.split(functions_tags_folder)
+				namespace = splitted[0].split("/")[-1]
 
-			# Get string that is used for calling the function (ex: "#namespace:my_function")
-			to_be_called = f"#{namespace}:" + splitted[1].replace(".json","")
+				# Get string that is used for calling the function (ex: "#namespace:my_function")
+				to_be_called = f"#{namespace}:" + splitted[1].replace(".json","")
 
-			# Read the json file and loop its values
-			data = json.loads(FILES_TO_WRITE[file_path])
-			if data.get("values"):
-				for value in data["values"]:
+				# Read the json file and loop its values
+				data = json.loads(FILES_TO_WRITE[file_path])
+				if data.get("values"):
+					for value in data["values"]:
 
-					# Get the function that is called, either "function" or {"id": "function", ...}
-					calling = value if type(value) == str else value["id"]
+						# Get the function that is called, either "function" or {"id": "function", ...}
+						calling = value if type(value) == str else value["id"]
 
-					# If the called function is registered, append the name of this file
+						# If the called function is registered, append the name of this file
+						if calling in mcfunctions.keys() and to_be_called not in mcfunctions[calling]["within"]:
+							mcfunctions[calling]["within"].append(to_be_called)
+
+			elif advancements_folder in file_path:
+
+				# Get namespace of the file
+				splitted = file_path.split(advancements_folder)
+				namespace = splitted[0].split("/")[-1]
+
+				# Get string that is used for calling the function (ex: "advancement namespace:my_function")
+				to_be_called = f"advancement {namespace}:" + splitted[1].replace(".json","")
+
+				# Read the json file and loop its values
+				data: dict = json.loads(FILES_TO_WRITE[file_path])
+				if data.get("rewards", {}) and data["rewards"].get("function"):
+					calling = data["rewards"]["function"]
 					if calling in mcfunctions.keys() and to_be_called not in mcfunctions[calling]["within"]:
 						mcfunctions[calling]["within"].append(to_be_called)
 
 
 	# For each mcfunction file, look at each lines
 	for file, data in mcfunctions.items():
 		for line in FILES_TO_WRITE[data["path"]].split("\n"):
```

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/lang.py` & `python_datapack-0.2.2/src/python_datapack/datapack/lang.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/loading.py` & `python_datapack-0.2.2/src/python_datapack/datapack/loading.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/loot_tables.py` & `python_datapack-0.2.2/src/python_datapack/datapack/loot_tables.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/main.py` & `python_datapack-0.2.2/src/python_datapack/datapack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/datapack/recipes.py` & `python_datapack-0.2.2/src/python_datapack/datapack/recipes.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/book_optimizer.py` & `python_datapack-0.2.2/src/python_datapack/manual/book_optimizer.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/main.py` & `python_datapack-0.2.2/src/python_datapack/manual/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 	super_copy(f"{TEMPLATES_PATH}/wiki_ingredient_of_craft.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/wiki_ingredient_of_craft.png")
 	if config['manual_high_resolution']:
 		super_copy(f"{TEMPLATES_PATH}/furnace.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/furnace.png")
 		super_copy(f"{TEMPLATES_PATH}/shaped_2x2.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_2x2.png")
 		super_copy(f"{TEMPLATES_PATH}/shaped_3x3.png", f"{config['build_resource_pack']}/assets/{config['namespace']}/textures/font/shaped_3x3.png")
 
 	# If the manual cache is enabled and we have a cache file, load it
-	if config['cache_manual_pages'] and os.path.exists(config['manual_debug']):
+	if config['cache_manual_pages'] and os.path.exists(config['manual_debug']) and os.path.exists(f"{config['manual_path']}/font/manual.json"):
 		with super_open(config['manual_debug'], "r") as f:
 			book_content = json.load(f)
 
 	# Else, generate all
 	else:
 
 		# Generate categories list
```

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/shared_import.py` & `python_datapack-0.2.2/src/python_datapack/manual/shared_import.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/utils.py` & `python_datapack-0.2.2/src/python_datapack/manual/utils.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/furnace.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/invisible_item_release.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/invisible_item_release.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/minecraft_font.ttf` & `python_datapack-0.2.2/src/python_datapack/manual/assets/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_2x2.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_2x2.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/shaped_3x3.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/shaped_3x3.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/simple_case_no_border.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/simple_case_no_border.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_information.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_information.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_ingredient_of_craft_template.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/manual/assets/wiki_result_of_craft.png` & `python_datapack-0.2.2/src/python_datapack/manual/assets/wiki_result_of_craft.png`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/resource_pack/check_unused_textures.py` & `python_datapack-0.2.2/src/python_datapack/resource_pack/check_unused_textures.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/resource_pack/item_models.py` & `python_datapack-0.2.2/src/python_datapack/resource_pack/item_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/resource_pack/main.py` & `python_datapack-0.2.2/src/python_datapack/resource_pack/main.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/resource_pack/sounds.py` & `python_datapack-0.2.2/src/python_datapack/resource_pack/sounds.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/resource_pack/vanilla_models.py` & `python_datapack-0.2.2/src/python_datapack/resource_pack/vanilla_models.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/database_helper.py` & `python_datapack-0.2.2/src/python_datapack/utils/database_helper.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/ingredients.py` & `python_datapack-0.2.2/src/python_datapack/utils/ingredients.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/io.py` & `python_datapack-0.2.2/src/python_datapack/utils/io.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/multiprocessing.py` & `python_datapack-0.2.2/src/python_datapack/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/print.py` & `python_datapack-0.2.2/src/python_datapack/utils/print.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/src/python_datapack/utils/weld.py` & `python_datapack-0.2.2/src/python_datapack/utils/weld.py`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/LICENSE` & `python_datapack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datapack-0.2.1/pyproject.toml` & `python_datapack-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling", "pillow", "smithed", "model_resolver"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_datapack"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
 	{ name="Stoupy51", email="stoupy51@gmail.com" },
 ]
 description = "Python package to help generating advanced Minecraft datapack contents"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `python_datapack-0.2.1/PKG-INFO` & `python_datapack-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_datapack
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package to help generating advanced Minecraft datapack contents
 Project-URL: Homepage, https://github.com/Stoupy51/python_datapack
 Project-URL: Issues, https://github.com/Stoupy51/python_datapack/issues
 Author-email: Stoupy51 <stoupy51@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

