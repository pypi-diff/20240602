# Comparing `tmp/basketball_reference_webscrapper-0.4.0.tar.gz` & `tmp/basketball_reference_webscrapper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basketball_reference_webscrapper-0.4.0.tar", max compression
+gzip compressed data, was "basketball_reference_webscrapper-0.4.1.tar", max compression
```

## Comparing `basketball_reference_webscrapper-0.4.0.tar` & `basketball_reference_webscrapper-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2967 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/__init__.py
--rw-r--r--   0        0        0     1223 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/team_city_refdata.csv
--rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/data_models/__init_.py
--rw-r--r--   0        0        0      213 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/data_models/feature_model.py
--rw-r--r--   0        0        0     2153 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/params.yaml
--rw-r--r--   0        0        0        0 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/__init__.py
--rw-r--r--   0        0        0     1075 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/logs.py
--rw-r--r--   0        0        0     8575 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py
--rw-r--r--   0        0        0      958 2024-06-01 07:28:50.621763 basketball_reference_webscrapper-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2558 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/constants/__init__.py
+-rw-r--r--   0        0        0     1223 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/constants/team_city_refdata.csv
+-rw-r--r--   0        0        0        0 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/data_models/__init_.py
+-rw-r--r--   0        0        0      213 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/data_models/feature_model.py
+-rw-r--r--   0        0        0     2153 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/params.yaml
+-rw-r--r--   0        0        0        0 2024-06-02 16:26:13.347033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/utils/__init__.py
+-rw-r--r--   0        0        0     1075 2024-06-02 16:26:13.351033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/utils/logs.py
+-rw-r--r--   0        0        0     8575 2024-06-02 16:26:13.351033 basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/webscrapping_basketball_reference.py
+-rw-r--r--   0        0        0      958 2024-06-02 16:26:13.351033 basketball_reference_webscrapper-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 basketball_reference_webscrapper-0.4.1/PKG-INFO
```

### Comparing `basketball_reference_webscrapper-0.4.0/README.md` & `basketball_reference_webscrapper-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# WebScrapBasketballReference
+# basketball-reference-webscrapper
 
-WebScrapBasketballReference is a Python package designed to scrape NBA games data from the Basketball Reference website. By providing a URL and a season, the package returns all games' team stats for that season.
+basketball-reference-webscrapper is a Python package designed to web scrape NBA games data from the Basketball Reference website.
 
 ## Features
 
-- Scrapes NBA gamelogs, schedules, and player attributes.
+- Web scrapes NBA gamelogs, schedules, and player attributes.
 - Validates user inputs to ensure data accuracy.
 - Handles team-specific data filtering.
 - Collects and processes data into a pandas DataFrame.
 
 ## Installation
 
-To install WebScrapBasketballReference, clone the repository and install the required dependencies:
+To install  basketball-reference-webscrapper, clone the repository and install the required dependencies:
 
 ```bash
-git clone https://github.com/yourusername/WebScrapBasketballReference.git
-cd WebScrapBasketballReference
-pip install -r requirements.txt
+pip install basketball-reference-webscrapper
 ```
 
 ## Usage
 
 ### Importing the Package
 
 ```python
@@ -53,19 +51,15 @@
 
 - **Data Type Validation:** Ensures `data_type` is one of `'gamelog'`, `'schedule'`, or `'player_attributes'`.
 - **Season Validation:** Ensures `season` is an integer between 2000 and the current NBA season.
 - **Team List Validation:** Ensures `team` is either `'all'` or a list of valid NBA team abbreviations.
 
 ## Configuration
 
-The package uses a `params.yaml` file to store URL patterns and other configurations. Ensure this file is correctly set up in the `basketball_reference_webscrapper` directory.
-
-## Logging
-
-Logging is configured to provide information about the scraping execution. Logs can be viewed to monitor the process and debug if necessary.
+The package uses a `params.yaml` file to store URL patterns and other configurations.
 
 ## Example
 
 ```python
 from basketball_reference_webscrapper.data_models.feature_model import FeatureIn
 from basketball_reference_webscrapper.webscrap_basketball_reference import WebScrapBasketballReference
 
@@ -80,19 +74,17 @@
 # Create the scraper instance
 scraper = WebScrapBasketballReference(feature_object)
 
 # Scrape the data
 data = scraper.webscrappe_nba_games_data()
 
 # Display the data
-print(data)
+print(data.head())
 ```
 
 ## Contributing
 
 Contributions are welcome! Please submit a pull request or create an issue to report bugs or request features.
 
-## License
-
 ## Contact
 
 For any questions or feedback, please contact [yannick.flores1992@gmail.com].
```

### Comparing `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/constants/team_city_refdata.csv` & `basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/constants/team_city_refdata.csv`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/params.yaml` & `basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/params.yaml`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/utils/logs.py` & `basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.4.0/basketball_reference_webscrapper/webscrapping_basketball_reference.py` & `basketball_reference_webscrapper-0.4.1/basketball_reference_webscrapper/webscrapping_basketball_reference.py`

 * *Files identical despite different names*

### Comparing `basketball_reference_webscrapper-0.4.0/pyproject.toml` & `basketball_reference_webscrapper-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basketball-reference-webscrapper"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python package for Basketball Reference that gathers data by scraping the website"
 authors = ["Yannick Flores <yannick.flores1992@gmail.com>"]
 readme = "README.md"
 exclude = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `basketball_reference_webscrapper-0.4.0/PKG-INFO` & `basketball_reference_webscrapper-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basketball-reference-webscrapper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package for Basketball Reference that gathers data by scraping the website
 Author: Yannick Flores
 Author-email: yannick.flores1992@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,33 +13,31 @@
 Requires-Dist: pandas (==2.*)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: pylint (>=2.15.10,<3.0.0)
 Requires-Dist: pytest
 Requires-Dist: requests (==2.32.*)
 Description-Content-Type: text/markdown
 
-# WebScrapBasketballReference
+# basketball-reference-webscrapper
 
-WebScrapBasketballReference is a Python package designed to scrape NBA games data from the Basketball Reference website. By providing a URL and a season, the package returns all games' team stats for that season.
+basketball-reference-webscrapper is a Python package designed to web scrape NBA games data from the Basketball Reference website.
 
 ## Features
 
-- Scrapes NBA gamelogs, schedules, and player attributes.
+- Web scrapes NBA gamelogs, schedules, and player attributes.
 - Validates user inputs to ensure data accuracy.
 - Handles team-specific data filtering.
 - Collects and processes data into a pandas DataFrame.
 
 ## Installation
 
-To install WebScrapBasketballReference, clone the repository and install the required dependencies:
+To install  basketball-reference-webscrapper, clone the repository and install the required dependencies:
 
 ```bash
-git clone https://github.com/yourusername/WebScrapBasketballReference.git
-cd WebScrapBasketballReference
-pip install -r requirements.txt
+pip install basketball-reference-webscrapper
 ```
 
 ## Usage
 
 ### Importing the Package
 
 ```python
@@ -72,19 +70,15 @@
 
 - **Data Type Validation:** Ensures `data_type` is one of `'gamelog'`, `'schedule'`, or `'player_attributes'`.
 - **Season Validation:** Ensures `season` is an integer between 2000 and the current NBA season.
 - **Team List Validation:** Ensures `team` is either `'all'` or a list of valid NBA team abbreviations.
 
 ## Configuration
 
-The package uses a `params.yaml` file to store URL patterns and other configurations. Ensure this file is correctly set up in the `basketball_reference_webscrapper` directory.
-
-## Logging
-
-Logging is configured to provide information about the scraping execution. Logs can be viewed to monitor the process and debug if necessary.
+The package uses a `params.yaml` file to store URL patterns and other configurations.
 
 ## Example
 
 ```python
 from basketball_reference_webscrapper.data_models.feature_model import FeatureIn
 from basketball_reference_webscrapper.webscrap_basketball_reference import WebScrapBasketballReference
 
@@ -99,20 +93,18 @@
 # Create the scraper instance
 scraper = WebScrapBasketballReference(feature_object)
 
 # Scrape the data
 data = scraper.webscrappe_nba_games_data()
 
 # Display the data
-print(data)
+print(data.head())
 ```
 
 ## Contributing
 
 Contributions are welcome! Please submit a pull request or create an issue to report bugs or request features.
 
-## License
-
 ## Contact
 
 For any questions or feedback, please contact [yannick.flores1992@gmail.com].
```

