# Comparing `tmp/pynboard-0.0.1.tar.gz` & `tmp/pynboard-0.0.2.tar.gz`

## Comparing `pynboard-0.0.1.tar` & `pynboard-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/pynboard.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynboard-0.0.1/src/pynboard/__init__.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pynboard-0.0.1/src/pynboard/actions.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.1/src/pynboard/core.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pynboard-0.0.1/src/pynboard/html_buffer.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.1/src/pynboard/utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.1/README.md
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pynboard-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pynboard-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pynboard-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/pynboard.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pynboard-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/__init__.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/actions.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/core.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/html_buffer.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pynboard-0.0.2/src/pynboard/utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pynboard-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pynboard-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pynboard-0.0.2/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pynboard-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pynboard-0.0.2/PKG-INFO
```

### Comparing `pynboard-0.0.1/.idea/workspace.xml` & `pynboard-0.0.2/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `pynboard-0.0.1/.idea/workspace.xml` & `pynboard-0.0.2/.idea/workspace.xml`

```diff
@@ -1,11 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
+  <component name="AutoImportSettings">
+    <option name="autoReloadType" value="SELECTIVE"/>
+  </component>
   <component name="ChangeListManager">
-    <list default="true" id="8e3ec5eb-ecea-4929-9532-604c6ae2131c" name="Changes" comment=""/>
+    <list default="true" id="8e3ec5eb-ecea-4929-9532-604c6ae2131c" name="Changes" comment="pyproject.toml">
+      <change afterPath="$PROJECT_DIR$/requirements.txt" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
@@ -24,14 +29,18 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "git-widget-placeholder": "main",
     "last_opened_file_path": "C:/Users/Lukas/mambaforge/condabin/conda.bat",
+    "node.js.detected.package.eslint": "true",
+    "node.js.detected.package.tslint": "true",
+    "node.js.selected.package.eslint": "(autodetect)",
+    "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "settings.editor.selected.configurable": "pyconsole",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="PyConsoleOptionsProvider">
     <option name="myShowVariablesByDefault" value="false"/>
@@ -48,15 +57,37 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="8e3ec5eb-ecea-4929-9532-604c6ae2131c" name="Changes" comment=""/>
       <created>1717348824739</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1717348824739</updated>
-      <workItem from="1717348826484" duration="32000"/>
+      <workItem from="1717348826484" duration="3287000"/>
+    </task>
+    <task id="LOCAL-00001" summary="pynboard">
+      <option name="closed" value="true"/>
+      <created>1717348938104</created>
+      <option name="number" value="00001"/>
+      <option name="presentableId" value="LOCAL-00001"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1717348938104</updated>
     </task>
+    <task id="LOCAL-00002" summary="pyproject.toml">
+      <option name="closed" value="true"/>
+      <created>1717350483007</created>
+      <option name="number" value="00002"/>
+      <option name="presentableId" value="LOCAL-00002"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1717350483007</updated>
+    </task>
+    <option name="localTasksCounter" value="3"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
+  <component name="VcsManagerConfiguration">
+    <MESSAGE value="pynboard"/>
+    <MESSAGE value="pyproject.toml"/>
+    <option name="LAST_COMMIT_MESSAGE" value="pyproject.toml"/>
+  </component>
 </project>
```

### Comparing `pynboard-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `pynboard-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.1/src/pynboard/__init__.py` & `pynboard-0.0.2/src/pynboard/__init__.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.1/src/pynboard/actions.py` & `pynboard-0.0.2/src/pynboard/actions.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.1/src/pynboard/core.py` & `pynboard-0.0.2/src/pynboard/core.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.1/src/pynboard/html_buffer.py` & `pynboard-0.0.2/src/pynboard/html_buffer.py`

 * *Files identical despite different names*

### Comparing `pynboard-0.0.1/LICENSE` & `pynboard-0.0.2/LICENSE`

 * *Files identical despite different names*

