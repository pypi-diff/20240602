# Comparing `tmp/niaaml_gui-0.3.0.tar.gz` & `tmp/niaaml_gui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niaaml_gui-0.3.0.tar", max compression
+gzip compressed data, was "niaaml_gui-0.3.1.tar", max compression
```

## Comparing `niaaml_gui-0.3.0.tar` & `niaaml_gui-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/LICENSE
--rw-r--r--   0        0        0     7131 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/README.md
--rw-r--r--   0        0        0      322 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/niaaml_gui/__init__.py
--rw-r--r--   0        0        0     2199 2024-04-30 18:39:11.971898 niaaml_gui-0.3.0/niaaml_gui/main.py
--rw-r--r--   0        0        0     1215 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/process_window_data.py
--rw-r--r--   0        0        0      291 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/progress_bar.py
--rw-r--r--   0        0        0      971 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/styles.qss
--rw-r--r--   0        0        0      281 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/__init__.py
--rw-r--r--   0        0        0     1499 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/base_main_widget.py
--rw-r--r--   0        0        0      770 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/list_widget_custom.py
--rw-r--r--   0        0        0    15746 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/optimization_widget.py
--rw-r--r--   0        0        0     3489 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/widgets/use_pipeline_widget.py
--rw-r--r--   0        0        0      223 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/__init__.py
--rw-r--r--   0        0        0     3544 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/csv_editor_window.py
--rw-r--r--   0        0        0     3427 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/process_window.py
--rw-r--r--   0        0        0      173 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/__init__.py
--rw-r--r--   0        0        0     1999 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/optimize_thread.py
--rw-r--r--   0        0        0      593 2024-04-30 18:39:11.972898 niaaml_gui-0.3.0/niaaml_gui/windows/threads/run_thread.py
--rw-r--r--   0        0        0      862 2024-04-30 18:39:11.973898 niaaml_gui-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8048 1970-01-01 00:00:00.000000 niaaml_gui-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7194 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/README.md
+-rw-r--r--   0        0        0      322 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/__init__.py
+-rw-r--r--   0        0        0     2199 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/main.py
+-rw-r--r--   0        0        0     1215 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/process_window_data.py
+-rw-r--r--   0        0        0      291 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/progress_bar.py
+-rw-r--r--   0        0        0     1060 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/styles.qss
+-rw-r--r--   0        0        0      281 2024-06-02 10:04:15.883849 niaaml_gui-0.3.1/niaaml_gui/widgets/__init__.py
+-rw-r--r--   0        0        0     1499 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/widgets/base_main_widget.py
+-rw-r--r--   0        0        0      770 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/widgets/list_widget_custom.py
+-rw-r--r--   0        0        0    15746 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/widgets/optimization_widget.py
+-rw-r--r--   0        0        0     3489 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/widgets/use_pipeline_widget.py
+-rw-r--r--   0        0        0      223 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/windows/__init__.py
+-rw-r--r--   0        0        0     3544 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/windows/csv_editor_window.py
+-rw-r--r--   0        0        0     3427 2024-06-02 10:04:15.884849 niaaml_gui-0.3.1/niaaml_gui/windows/process_window.py
+-rw-r--r--   0        0        0      173 2024-06-02 10:04:15.885849 niaaml_gui-0.3.1/niaaml_gui/windows/threads/__init__.py
+-rw-r--r--   0        0        0     1999 2024-06-02 10:04:15.885849 niaaml_gui-0.3.1/niaaml_gui/windows/threads/optimize_thread.py
+-rw-r--r--   0        0        0      593 2024-06-02 10:04:15.885849 niaaml_gui-0.3.1/niaaml_gui/windows/threads/run_thread.py
+-rw-r--r--   0        0        0      862 2024-06-02 10:04:15.887849 niaaml_gui-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8162 1970-01-01 00:00:00.000000 niaaml_gui-0.3.1/PKG-INFO
```

### Comparing `niaaml_gui-0.3.0/LICENSE` & `niaaml_gui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/README.md` & `niaaml_gui-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/lukapecnik/NiaAML-GUI.svg)
 [![Fedora package](https://img.shields.io/fedora/v/NiaAML-GUI?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/NiaAML-GUI)
 [![Packaging status](https://repology.org/badge/tiny-repos/niaaml-gui.svg)](https://repology.org/project/niaaml-gui/versions)
 
 ---
 
-This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/lukapecnik/NiaAML) Python package.
+This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/firefly-cpp/NiaAML) Python package.
 
-* **Python versions:** 3.9.x, 3.10.x, 3.11.x
+* **Python versions:** 3.9.x, 3.10.x, 3.11.x, 3.12.x
 
 ## Installation
 
 Install NiaAML-GUI with pip:
 
 ```sh
 pip install niaaml_gui
@@ -47,15 +47,15 @@
 
 ```sh
 $ apk add niaaml-gui
 ```
 
 ## Usage
 
-NiaAML GUI application allows you to use main features of the [NiaAML](https://github.com/lukapecnik/NiaAML) framework. There are two views in the application. In the first one, you can prepare an environment for a pipeline optimization process. The purpose of the second one is to allow you to use an existing pipeline from a file. **The application currently supports data input in a form of CSV files.**
+NiaAML GUI application allows you to use main features of the [NiaAML](https://github.com/firefly-cpp/NiaAML) framework. There are two views in the application. In the first one, you can prepare an environment for a pipeline optimization process. The purpose of the second one is to allow you to use an existing pipeline from a file. **The application currently supports data input in a form of CSV files.**
 
 ### Optimization View
 
 Below is a screenshot of the first view with labeled components and you can find a description for each component under the screenshot.
 
 <p align="center"><img src=".github/gui1.png" alt="NiaAML GUI First View" title="NiaAML GUI First View"/></p>
 
@@ -170,8 +170,8 @@
 
 ## References
 
 <a id="1">[1]</a> Dua, D. and Graff, C. (2019). [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml). Irvine, CA: University of California, School of Information and Computer Science.
 
 ## Cite us
 
-L. Pečnik, I. Fister Jr. "NiaAML: AutoML framework based on stochastic population-based nature-inspired algorithms." Journal of Open Source Software 6.61 (2021): 2949.
+L. Pečnik, I. Fister Jr. "[NiaAML: AutoML framework based on stochastic population-based nature-inspired algorithms](https://joss.theoj.org/papers/10.21105/joss.02949)." Journal of Open Source Software 6.61 (2021): 2949.
```

### Comparing `niaaml_gui-0.3.0/niaaml_gui/main.py` & `niaaml_gui-0.3.1/niaaml_gui/main.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/process_window_data.py` & `niaaml_gui-0.3.1/niaaml_gui/process_window_data.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/styles.qss` & `niaaml_gui-0.3.1/niaaml_gui/styles.qss`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     padding: 2;
     font-weight: 600;
 }
 
 QLabel {
     width: fit-content;
     font-weight: 700;
-    /* color: #547500; */
 }
 
 QPushButton#editCSVButton{
     background-color:#547500;
 }
 
 QLineEdit {
@@ -52,8 +51,17 @@
 
 
 QListWidget::item:selected {
     background-color: #547500;
     color: white;
     border: 2px solid #547500;
     border-top: 0;
-}
+}
+
+QProgressBar {
+    color: black;
+    font-weight: 600;
+}
+
+QProgressBar::chunk {
+    background-color: #547500;
+}
```

### Comparing `niaaml_gui-0.3.0/niaaml_gui/widgets/base_main_widget.py` & `niaaml_gui-0.3.1/niaaml_gui/widgets/base_main_widget.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/widgets/list_widget_custom.py` & `niaaml_gui-0.3.1/niaaml_gui/widgets/list_widget_custom.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/widgets/optimization_widget.py` & `niaaml_gui-0.3.1/niaaml_gui/widgets/optimization_widget.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/widgets/use_pipeline_widget.py` & `niaaml_gui-0.3.1/niaaml_gui/widgets/use_pipeline_widget.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/windows/csv_editor_window.py` & `niaaml_gui-0.3.1/niaaml_gui/windows/csv_editor_window.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/windows/process_window.py` & `niaaml_gui-0.3.1/niaaml_gui/windows/process_window.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/windows/threads/optimize_thread.py` & `niaaml_gui-0.3.1/niaaml_gui/windows/threads/optimize_thread.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/niaaml_gui/windows/threads/run_thread.py` & `niaaml_gui-0.3.1/niaaml_gui/windows/threads/run_thread.py`

 * *Files identical despite different names*

### Comparing `niaaml_gui-0.3.0/pyproject.toml` & `niaaml_gui-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NiaAML-GUI"
-version = "0.3.0"
+version = "0.3.1"
 description = "GUI for NiaAML Python package"
 license = "MIT"
 authors = ["Luka Pečnik <lukapecnik96@gmail.com>"]
 keywords = ['classification', 'NiaPy', 'NiaAML', 'scikit-learn', 'nature-inspired algorithms', 'feature selection', 'preprocessing']
 homepage = "https://github.com/firefly-cpp/NiaAML-GUI"
 repository = "https://github.com/firefly-cpp/NiaAML-GUI"
 readme = "README.md"
```

### Comparing `niaaml_gui-0.3.0/PKG-INFO` & `niaaml_gui-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: niaaml-gui
-Version: 0.3.0
+Name: NiaAML-GUI
+Version: 0.3.1
 Summary: GUI for NiaAML Python package
 Home-page: https://github.com/firefly-cpp/NiaAML-GUI
 License: MIT
 Keywords: classification,NiaPy,NiaAML,scikit-learn,nature-inspired algorithms,feature selection,preprocessing
 Author: Luka Pečnik
 Author-email: lukapecnik96@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: QtAwesome (>=1.2.3,<2.0.0)
 Requires-Dist: niaaml (>=1.2.0,<2.0.0)
 Requires-Dist: niapy (>=2.0.5,<3.0.0)
 Requires-Dist: pyqt6 (>=6.6.0,<7.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
 Project-URL: Repository, https://github.com/firefly-cpp/NiaAML-GUI
 Description-Content-Type: text/markdown
@@ -34,17 +35,17 @@
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/lukapecnik/NiaAML-GUI.svg)](http://isitmaintained.com/project/lukapecnik/NiaAML-GUI "Percentage of issues still open")
 ![GitHub contributors](https://img.shields.io/github/contributors/lukapecnik/NiaAML-GUI.svg)
 [![Fedora package](https://img.shields.io/fedora/v/NiaAML-GUI?color=blue&label=Fedora%20Linux&logo=fedora)](https://src.fedoraproject.org/rpms/NiaAML-GUI)
 [![Packaging status](https://repology.org/badge/tiny-repos/niaaml-gui.svg)](https://repology.org/project/niaaml-gui/versions)
 
 ---
 
-This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/lukapecnik/NiaAML) Python package.
+This is a basic graphical user interface intended for users of the [NiaAML](https://github.com/firefly-cpp/NiaAML) Python package.
 
-* **Python versions:** 3.9.x, 3.10.x, 3.11.x
+* **Python versions:** 3.9.x, 3.10.x, 3.11.x, 3.12.x
 
 ## Installation
 
 Install NiaAML-GUI with pip:
 
 ```sh
 pip install niaaml_gui
@@ -70,15 +71,15 @@
 
 ```sh
 $ apk add niaaml-gui
 ```
 
 ## Usage
 
-NiaAML GUI application allows you to use main features of the [NiaAML](https://github.com/lukapecnik/NiaAML) framework. There are two views in the application. In the first one, you can prepare an environment for a pipeline optimization process. The purpose of the second one is to allow you to use an existing pipeline from a file. **The application currently supports data input in a form of CSV files.**
+NiaAML GUI application allows you to use main features of the [NiaAML](https://github.com/firefly-cpp/NiaAML) framework. There are two views in the application. In the first one, you can prepare an environment for a pipeline optimization process. The purpose of the second one is to allow you to use an existing pipeline from a file. **The application currently supports data input in a form of CSV files.**
 
 ### Optimization View
 
 Below is a screenshot of the first view with labeled components and you can find a description for each component under the screenshot.
 
 <p align="center"><img src=".github/gui1.png" alt="NiaAML GUI First View" title="NiaAML GUI First View"/></p>
 
@@ -193,9 +194,9 @@
 
 ## References
 
 <a id="1">[1]</a> Dua, D. and Graff, C. (2019). [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml). Irvine, CA: University of California, School of Information and Computer Science.
 
 ## Cite us
 
-L. Pečnik, I. Fister Jr. "NiaAML: AutoML framework based on stochastic population-based nature-inspired algorithms." Journal of Open Source Software 6.61 (2021): 2949.
+L. Pečnik, I. Fister Jr. "[NiaAML: AutoML framework based on stochastic population-based nature-inspired algorithms](https://joss.theoj.org/papers/10.21105/joss.02949)." Journal of Open Source Software 6.61 (2021): 2949.
```

