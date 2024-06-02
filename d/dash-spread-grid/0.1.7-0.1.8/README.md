# Comparing `tmp/dash_spread_grid-0.1.7.tar.gz` & `tmp/dash_spread_grid-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_spread_grid-0.1.7.tar", last modified: Sun Jun  2 06:05:02 2024, max compression
+gzip compressed data, was "dash_spread_grid-0.1.8.tar", last modified: Sun Jun  2 06:35:37 2024, max compression
```

## Comparing `dash_spread_grid-0.1.7.tar` & `dash_spread_grid-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:05:02.942674 dash_spread_grid-0.1.7/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.7/LICENSE
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.7/MANIFEST.in
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-06-02 06:05:02.942674 dash_spread_grid-0.1.7/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.7/README.md
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:05:02.942674 dash_spread_grid-0.1.7/dash_spread_grid/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3490 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid/DashSpreadGrid.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.7/dash_spread_grid/__init__.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid/_imports_.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    58258 2024-06-02 06:05:01.000000 dash_spread_grid-0.1.7/dash_spread_grid/dash_spread_grid.min.js
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   227440 2024-06-02 06:05:01.000000 dash_spread_grid-0.1.7/dash_spread_grid/dash_spread_grid.min.js.map
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6509 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid/metadata.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid/package-info.json
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:05:02.942674 dash_spread_grid-0.1.7/dash_spread_grid.egg-info/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid.egg-info/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-06-02 06:05:02.000000 dash_spread_grid-0.1.7/dash_spread_grid.egg-info/top_level.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-06-02 06:04:48.000000 dash_spread_grid-0.1.7/package.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-06-02 06:05:02.942674 dash_spread_grid-0.1.7/setup.cfg
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.7/setup.py
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:35:37.652670 dash_spread_grid-0.1.8/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.8/LICENSE
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.8/MANIFEST.in
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-06-02 06:35:37.652670 dash_spread_grid-0.1.8/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.8/README.md
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:35:37.652670 dash_spread_grid-0.1.8/dash_spread_grid/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3490 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid/DashSpreadGrid.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.8/dash_spread_grid/__init__.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid/_imports_.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    58258 2024-06-02 06:35:36.000000 dash_spread_grid-0.1.8/dash_spread_grid/dash_spread_grid.min.js
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   227440 2024-06-02 06:35:36.000000 dash_spread_grid-0.1.8/dash_spread_grid/dash_spread_grid.min.js.map
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6509 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid/metadata.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid/package-info.json
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-06-02 06:35:37.652670 dash_spread_grid-0.1.8/dash_spread_grid.egg-info/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-06-02 06:35:37.000000 dash_spread_grid-0.1.8/dash_spread_grid.egg-info/top_level.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-06-02 06:35:22.000000 dash_spread_grid-0.1.8/package.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-06-02 06:35:37.652670 dash_spread_grid-0.1.8/setup.cfg
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.8/setup.py
```

### Comparing `dash_spread_grid-0.1.7/README.md` & `dash_spread_grid-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/DashSpreadGrid.py` & `dash_spread_grid-0.1.8/dash_spread_grid/DashSpreadGrid.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/__init__.py` & `dash_spread_grid-0.1.8/dash_spread_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/dash_spread_grid.min.js` & `dash_spread_grid-0.1.8/dash_spread_grid/dash_spread_grid.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2674,15 +2674,15 @@
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
                 o = isLocalScript(t),
                 n = __jsonpScriptSrc__(e);
             if (!o) return n;
             var r = n.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_1_7m1717308301"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_1_8m1717310136"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     var __webpack_exports__ = {};
     (() => {
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
             DashSpreadGrid: () => e.Z
         });
```

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/dash_spread_grid.min.js.map` & `dash_spread_grid-0.1.8/dash_spread_grid/dash_spread_grid.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982578397212544%*

 * *Differences: {"'sourcesContent'": "{insert: [(80, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc […]*

```diff
@@ -960,11 +960,11 @@
         "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.key === stringifyId(columnId) && row.key === stringifyId(rowId);\n    }\n\n    function isConflictingWithCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.type === 'HEADER' && column.key === stringifyId(columnId)\n            || row.type === 'HEADER' && row.key === stringifyId(rowId);\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld\n        ? sortBy.filter(rule => !isCurrentRule(rule))\n        : sortBy.filter(rule => !isConflictingWithCurrentRule(rule));\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport Selection from \"../types/Selection.js\";\n\nexport default function getClipboardData(selectedCells, columns, rows, formatResolver) {\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const selectedCellKeys = selectedCells.map(cell => ({\n        columnKey: stringifyId(cell.columnId),\n        rowKey: stringifyId(cell.rowId)\n    })).filter(cell => columnLookup.has(cell.columnKey) && rowLookup.has(cell.rowKey));\n    const selectedColumns = new Set(selectedCellKeys.map(cell => cell.columnKey));\n    const selectedRows = new Set(selectedCellKeys.map(cell => cell.rowKey));\n\n    if (selectedCellKeys.length === 0)\n        return '';\n\n    const selection = new Selection(selectedCells);\n    const minColumnIndex = Math.min(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const maxColumnIndex = Math.max(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const minRowIndex = Math.min(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n    const maxRowIndex = Math.max(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n\n    const stringBuilder = [];\n\n    for (let rowIndex = minRowIndex; rowIndex <= maxRowIndex; rowIndex++) {\n        const row = rows[rowIndex];\n        const rowKey = row.key;\n\n        if (!selectedRows.has(rowKey))\n            continue;\n\n        for (let columnIndex = minColumnIndex; columnIndex <= maxColumnIndex; columnIndex++) {\n            const column = columns[columnIndex];\n            const columnKey = column.key;\n\n            if (!selectedColumns.has(columnKey))\n                continue;\n\n            if (selection.isKeySelected(rowKey, columnKey)) {\n                const cellData = formatResolver.resolve(row, column).text;\n                stringBuilder.push(cellData);\n            }\n\n            if (columnIndex < maxColumnIndex)\n                stringBuilder.push('\\t');\n        }\n\n        if (rowIndex < maxRowIndex)\n            stringBuilder.push('\\n');\n    }\n\n    return stringBuilder.join('');\n}",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_7m1717308301\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_8m1717310136\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
     ],
     "version": 3
 }
```

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/metadata.json` & `dash_spread_grid-0.1.8/dash_spread_grid/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.1.7/dash_spread_grid/package-info.json` & `dash_spread_grid-0.1.8/dash_spread_grid/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.7",
+    "version": "0.1.8",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

### Comparing `dash_spread_grid-0.1.7/package.json` & `dash_spread_grid-0.1.8/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -53,15 +53,15 @@
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.1.7",
+    "version": "0.1.8",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

