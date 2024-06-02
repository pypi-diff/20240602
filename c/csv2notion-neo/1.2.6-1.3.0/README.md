# Comparing `tmp/csv2notion_neo-1.2.6.tar.gz` & `tmp/csv2notion_neo-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2notion_neo-1.2.6.tar", max compression
+gzip compressed data, was "csv2notion_neo-1.3.0.tar", max compression
```

## Comparing `csv2notion_neo-1.2.6.tar` & `csv2notion_neo-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     3070 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/CHANGELOG.md
--rw-r--r--   0        0        0     1068 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/LICENSE
--rw-r--r--   0        0        0    27897 2024-05-19 01:26:54.960995 csv2notion_neo-1.2.6/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:26:55.401000 csv2notion_neo-1.2.6/csv2notion_neo/__init__.py
--rw-r--r--   0        0        0      119 2024-05-19 01:26:55.401000 csv2notion_neo-1.2.6/csv2notion_neo/__main__.py
--rw-r--r--   0        0        0     3139 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli.py
--rw-r--r--   0        0        0    11825 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli_args.py
--rw-r--r--   0        0        0     2353 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/cli_steps.py
--rw-r--r--   0        0        0     5533 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/local_data.py
--rw-r--r--   0        0        0        0 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/__init__.py
--rw-r--r--   0        0        0    24846 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/block.py
--rw-r--r--   0        0        0    16051 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/client.py
--rw-r--r--   0        0        0    27147 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/collection.py
--rw-r--r--   0        0        0     1107 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/logger.py
--rw-r--r--   0        0        0     3725 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/maps.py
--rw-r--r--   0        0        0     9350 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/markdown.py
--rw-r--r--   0        0        0     8200 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/monitor.py
--rw-r--r--   0        0        0     1021 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/operations.py
--rw-r--r--   0        0        0     4898 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/records.py
--rw-r--r--   0        0        0      671 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/settings.py
--rw-r--r--   0        0        0     9398 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/smoke_test.py
--rw-r--r--   0        0        0     1636 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/space.py
--rw-r--r--   0        0        0    14842 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/store.py
--rw-r--r--   0        0        0      546 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/user.py
--rw-r--r--   0        0        0     2851 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/utils.py
--rw-r--r--   0        0        0     2279 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion/utils_ssl.py
--rw-r--r--   0        0        0    12666 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_convert.py
--rw-r--r--   0        0        0     1922 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_convert_map.py
--rw-r--r--   0        0        0     6697 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db.py
--rw-r--r--   0        0        0     2072 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db_client.py
--rw-r--r--   0        0        0     5092 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_db_collection.py
--rw-r--r--   0        0        0     9697 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_preparator.py
--rw-r--r--   0        0        0     9799 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row.py
--rw-r--r--   0        0        0     4151 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row_image_block.py
--rw-r--r--   0        0        0     2908 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_row_upload_file.py
--rw-r--r--   0        0        0     1126 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_type_guess.py
--rw-r--r--   0        0        0     1759 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/notion_uploader.py
--rw-r--r--   0        0        0     1503 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_ai.py
--rw-r--r--   0        0        0     1276 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_db.py
--rw-r--r--   0        0        0      305 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_exceptions.py
--rw-r--r--   0        0        0      331 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_file.py
--rw-r--r--   0        0        0      679 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_rand_id.py
--rw-r--r--   0        0        0     1792 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_static.py
--rw-r--r--   0        0        0      249 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_str.py
--rw-r--r--   0        0        0     1387 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/utils_threading.py
--rw-r--r--   0        0        0       22 2024-05-19 01:26:55.405000 csv2notion_neo-1.2.6/csv2notion_neo/version.py
--rw-r--r--   0        0        0     5334 2024-05-19 01:26:55.409000 csv2notion_neo-1.2.6/pyproject.toml
--rw-r--r--   0        0        0    29861 1970-01-01 00:00:00.000000 csv2notion_neo-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     3573 2024-06-02 21:49:46.917973 csv2notion_neo-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2024-06-02 21:49:46.917973 csv2notion_neo-1.3.0/LICENSE
+-rw-r--r--   0        0        0    32647 2024-06-02 21:49:46.917973 csv2notion_neo-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/__main__.py
+-rw-r--r--   0        0        0     3151 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/cli.py
+-rw-r--r--   0        0        0    12566 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/cli_args.py
+-rw-r--r--   0        0        0     2353 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/cli_steps.py
+-rw-r--r--   0        0        0     7015 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/local_data.py
+-rw-r--r--   0        0        0        0 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/__init__.py
+-rw-r--r--   0        0        0    24846 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/block.py
+-rw-r--r--   0        0        0    16051 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/client.py
+-rw-r--r--   0        0        0    27147 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/collection.py
+-rw-r--r--   0        0        0     1107 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/logger.py
+-rw-r--r--   0        0        0     3725 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/maps.py
+-rw-r--r--   0        0        0     9350 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/markdown.py
+-rw-r--r--   0        0        0     8200 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/monitor.py
+-rw-r--r--   0        0        0     1021 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/operations.py
+-rw-r--r--   0        0        0     4898 2024-06-02 21:49:47.437981 csv2notion_neo-1.3.0/csv2notion_neo/notion/records.py
+-rw-r--r--   0        0        0      671 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/settings.py
+-rw-r--r--   0        0        0     9398 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/smoke_test.py
+-rw-r--r--   0        0        0     1636 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/space.py
+-rw-r--r--   0        0        0    14842 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/store.py
+-rw-r--r--   0        0        0      546 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/user.py
+-rw-r--r--   0        0        0     2851 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/utils.py
+-rw-r--r--   0        0        0     2279 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion/utils_ssl.py
+-rw-r--r--   0        0        0    13243 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_convert.py
+-rw-r--r--   0        0        0     1922 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_convert_map.py
+-rw-r--r--   0        0        0     6697 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_db.py
+-rw-r--r--   0        0        0     2072 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_db_client.py
+-rw-r--r--   0        0        0     5092 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_db_collection.py
+-rw-r--r--   0        0        0     9697 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_preparator.py
+-rw-r--r--   0        0        0     9817 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_row.py
+-rw-r--r--   0        0        0     4151 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_row_image_block.py
+-rw-r--r--   0        0        0     2926 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_row_upload_file.py
+-rw-r--r--   0        0        0     1126 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_type_guess.py
+-rw-r--r--   0        0        0     1989 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/notion_uploader.py
+-rw-r--r--   0        0        0     2284 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_ai.py
+-rw-r--r--   0        0        0     1276 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_db.py
+-rw-r--r--   0        0        0      305 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_exceptions.py
+-rw-r--r--   0        0        0      331 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_file.py
+-rw-r--r--   0        0        0      679 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_rand_id.py
+-rw-r--r--   0        0        0     1887 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_static.py
+-rw-r--r--   0        0        0      249 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_str.py
+-rw-r--r--   0        0        0     1423 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/utils_threading.py
+-rw-r--r--   0        0        0       22 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/csv2notion_neo/version.py
+-rw-r--r--   0        0        0     5334 2024-06-02 21:49:47.441980 csv2notion_neo-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    34611 1970-01-01 00:00:00.000000 csv2notion_neo-1.3.0/PKG-INFO
```

### Comparing `csv2notion_neo-1.2.6/CHANGELOG.md` & `csv2notion_neo-1.3.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+### 1.3.0
+
+**🎉 Released:**
+- 3rd June 2024
+
+**🔨 Improvements:**
+- Automatically analyse and generate captions for images using Hugging Face's open-source AI/ML models (#25)
+- Added `--hugging-face-token`: Hugging Face token to use image captioning model online
+- Added `--hf-model `: Provide the model used for generating caption <`vit-gpt2` | `blip-image` | `git-large`> (defaults: `vit-gpt2`)
+- Added `--caption-column`: Provide both image column and column where caption would be written
+
+---
+
 ### 1.2.6
 
 **🎉 Released:**
 - 19th May 2024
 
 **🔨 Improvements:**
 - Improved log output for `--rename-notion-key-column` (#35)
```

### Comparing `csv2notion_neo-1.2.6/LICENSE` & `csv2notion_neo-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/README.md` & `csv2notion_neo-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 - Choose column types manually instead of letting Notion detecting them automatically
 - Link or create new entries in relation columns based on their values automatically
 - Easily upload files into the designated "Files & Media" column
 - Assign a icon for each row for quick identification
 - Set a cover or embed an image for each row to enhance visual representation
 - Upload image files for covers or icons
 - Apply validation options for input data to ensure accuracy
+- Automatically analyse and generate captions for images using Hugging Face's open-source AI/ML models
 
 ### Disadvantages over native import
  
 - Importing each row separately might lead to slower speed
   - To address this, utilise multithreaded upload
 
 ## Table of contents
@@ -53,14 +54,15 @@
   - [Missing Columns](#missing-columns)
   - [Column Types](#column-types)
   - [Mergin](#merging)
   - [Relation Columns](#relation-columns)
   - [Cover Image & Embedded Image](#cover-image--embedded-image)
   - [Icons](#icons)
   - [Mandatory Columns](#mandatory-columns)
+  - [AI/ML Options (Hugging Face)](#aiml-options-hugging-face)
 - [Examples](#examples)
 - [Credits](#credits)
 - [License](#license)
 - [Reporting Bugs](#reporting-bugs)
 
 ## Background
 
@@ -121,14 +123,19 @@
   --url URL                          Notion database URL; if none is provided, will create a new database
   --max-threads                      upload threads (default: 5)
   --log FILE                         file to store program log
   --verbose                          output debug information
   --version                          show program's version number and exit
   -h, --help                         show this help message and exit
 
+machine learning options:
+  --hugging-face-token              Hugging Face token to use image captioning model online
+  --hf-model                        Provide the model used for generating caption <vit-gpt2 | blip-image| git-large> (defaults: vit-gpt2)
+  --caption-column                  Provide both image column and column where caption would be written
+
 column options:
   --column-types                     comma-separated list of column types to use for non-key columns;
                                      if none is provided, types will be guessed from CSV values
                                      (can also be used with --add-missing-columns flag)
   --add-missing-columns              if columns are present in CSV but not in Notion DB, add them to Notion DB
   --rename-notion-key-column         rename the key column in the file to a different key column in Airtable
   --randomize-select-colors          randomize colors for added options in select and multi select columns
@@ -352,14 +359,74 @@
 
 If you want to set the same icon for each row, use the `--default-icon` option. If both `--icon-column` and `--default-icon` are present, the default icon is used if the row doesn't have anything in the icon column.
 
 ### Mandatory Columns
 
 If you want to ensure that specific columns always have value and are not allowed to be empty, then use the `--mandatory-column` option. The program execution will stop if validation fails.
 
+### AI/ML Options (Hugging Face)
+
+Hugging Face is a prominent AI company known for its contributions to natural language processing (NLP) through its comprehensive open-source platform. It offers an extensive library called Transformers, which provides pre-trained models for a wide range of NLP tasks, including text generation, sentiment analysis, translation, and more. These models are based on state-of-the-art architectures like BERT, GPT, and T5.
+
+The platform fosters a vibrant open-source community where developers and researchers can share and collaborate on models. Users can access, fine-tune, and deploy a vast array of community-contributed models via the Hugging Face Model Hub. This collaborative environment accelerates innovation and democratizes access to advanced machine learning tools.
+
+<details><summary>Obtaining Hugging Face Token</summary>
+<p>
+
+Steps to Obtain a Hugging Face Token with Write Mode
+
+1. **Create a Hugging Face Account (if you don't have one already):**
+   - Go to the [Hugging Face website](https://huggingface.co/).
+   - Click on "Sign Up" in the top right corner.
+   - Fill in your details (username, email, password) and complete the registration process.
+
+2. **Log In to Your Account:**
+   - If you already have an account, simply log in by clicking "Log In" and entering your credentials.
+
+3. **Navigate to Your Profile Settings:**
+   - Once logged in, click on your profile icon in the top right corner of the page.
+   - From the dropdown menu, select "Settings."
+
+4. **Access the API Tokens Section:**
+   - In the settings menu on the left side of the screen, find and click on "Access Tokens."
+
+5. **Create a New API Token:**
+   - In the "Access Tokens" section, you will see an option to create a new token.
+   - Click on "New token."
+
+6. **Set Permissions to Write Mode:**
+   - Provide a name for your token (e.g., "MyWriteToken").
+   - Set the permissions type to "Write" type by selecting the "Write" from the dropdown. This will grant the token write access, allowing you to perform actions that modify data on Hugging Face.
+
+7. **Generate and Copy Your Token:**
+   - Click on the "Generate token" button.
+   - Your new token will be displayed. Copy it and store it in a secure place, as you will need it to access Hugging Face's API services.
+
+**Note:** Keep your token secure and do not share it publicly, as it grants access to your Hugging Face account and its resources.
+
+</p>
+</details>
+
+<details><summary>Avaliable Model Information</summary>
+<p>
+
+| Models      | Information                                                          | Accuracy |
+| ---------- | -------------------------------------------------------------------- | -------- |
+| vit-gpt2   | [Link](https://huggingface.co/nlpconnect/vit-gpt2-image-captioning)  | Low - Medium   |
+| blip-image | [Link](https://huggingface.co/Salesforce/blip-image-captioning-base) | Low - Medium   |
+| git-large  | [Link](https://huggingface.co/microsoft/git-large)                   | Low - Medium   |
+
+**Note:** Additional models will be integrated in the future from Hugging Face as better models are identified.
+
+</p>
+</details>
+
+> [!WARNING]  
+> Please be aware that this feature is currently in an experimental phase. We strongly advise against uploading sensitive images or those of a personal and private nature. Images will be uploaded to Hugging Face’s servers for analysis. We recommend using commercial images, such as movie stills or stock photos, for AI captioning.
+
 ## Examples
 
 <details><summary>Importing CSV into New Database</summary>
 <p>
 
 ```shell
 csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE test.csv
@@ -369,70 +436,81 @@
 </p>
 </details>
 
 <details><summary>Using Custom Column Types</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --column-types "number,multi_select" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --column-types "number,multi_select" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_02.png?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing CSV into Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_03.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Merging CSV with Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --merge test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --merge test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_04.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Merging CSV with Select Columns in Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_ TOKEN_HERE --url NOTION URL --merge --merge-only-column "Column 2" --merge-onLy-column "Column 3" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_ TOKEN_HERE \
+  --url NOTION URL \
+  --merge \
+  --merge-only-column "Column 2" \
+  --merge-onLy-column "Column 3" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_05.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing Rows with Images</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --image-column "Image Column" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+--image-column "Image Column" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_06.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing Rows with Images (Multiple Image Column)</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --image-column "Colour Image" "Black & White Image" "Map" --image-column-keep --mandatory-column "Cat ID" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --image-column "Colour Image" "Black & White Image" "Map" \
+  --image-column-keep --mandatory-column "Cat ID" test.csv
 ```
 
 Example CSV
 
 ```text
 Cat ID,Animal Name,Location,Colour Image,Black & White Image,Map
 1,Lion,Namibia,Colour/lion.jpg,Black & White/lion.jpg,Map/Namibia.jpg
@@ -480,56 +558,88 @@
 </p>
 </details>
 
 <details><summary>Importing Rows with Emoji Icons</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --icon-column "Icon Column" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE  \
+  --icon-column "Icon Column" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_07.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Updating Emoji Icon Only for All Rows</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --default-icon 👍 --merge --merge-only-column "Key" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --default-icon 👍 \
+  --merge \
+  --merge-only-column "Key" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_08.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing JSON into Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-column "Cat ID" --merge JSON-Demo.json
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --mandatory-column "Cat ID" \
+  --payload-key-column "Cat ID" \
+  --merge JSON-Demo.json
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_09.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing JSON into Existing Database with a Different Key Column</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-Demo.json
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --mandatory-column "Cat ID" \
+  --payload-key-column "Cat ID" \
+  --rename-notion-key-column "Cat ID" "Anything ID" \
+  --merge JSON-Demo.json
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
+<details><summary>Utilising Hugging Face's AI/ML Model to Automatically Analyse and Generate Captions from Images</summary>
+<p>
+
+```shell
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --hugging-face-token YOUR_HUGGING_FACE_TOKEN_HERE \
+  --hf-model blip-image \
+  --caption-column "Image Filename" "Frame Description" \
+  --image-column "Image Filename" \
+  --image-column-keep \
+  --mandatory-column "Cat ID" \
+  --merge big_cats.csv
+```
+
+<p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_12.gif?raw=true"> </p>
+
+</p>
+</details>
+
 ## Utilised By
 
 ### Marker Data
 
 <details><summary>Marker Data's Notion Panel</summary>
 <p>
```

#### html2text {}

```diff
@@ -7,56 +7,63 @@
 JSON with the existing database, using the first column as a key to combine
 existing rows - Choose column types manually instead of letting Notion
 detecting them automatically - Link or create new entries in relation columns
 based on their values automatically - Easily upload files into the designated
 "Files & Media" column - Assign a icon for each row for quick identification -
 Set a cover or embed an image for each row to enhance visual representation -
 Upload image files for covers or icons - Apply validation options for input
-data to ensure accuracy ### Disadvantages over native import - Importing each
-row separately might lead to slower speed - To address this, utilise
-multithreaded upload ## Table of contents - [Background](#background) -
-[Installation](#installation) - [Pre-compiled Binary (Recommended)](#pre-
-compiled-binary-recommended) - [From Source](#from-source) - [Guide](#guide) -
-[macOS Release](#macos-release) - [Prerequisite](#prerequisite) - [Upload
-Speed](#upload-speed) - [Duplicate CSV Columns](#duplicate-csv-columns) -
-[Missing Columns](#missing-columns) - [Column Types](#column-types) - [Mergin]
-(#merging) - [Relation Columns](#relation-columns) - [Cover Image & Embedded
-Image](#cover-image--embedded-image) - [Icons](#icons) - [Mandatory Columns]
-(#mandatory-columns) - [Examples](#examples) - [Credits](#credits) - [License]
-(#license) - [Reporting Bugs](#reporting-bugs) ## Background Originally, we
-developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the
-lack of advanced importing support for `*.csv` files in [Notion](https://
-notion.so). We took inspiration from [Airtable](https://www.airtable.com)âs
-[CSV import extension](https://support.airtable.com/docs/csv-import-extension).
-**CSV2Notion Neo** was created as a spin-off project to address inactivity in
-the original repository and maintain compatibility with Notion. As Notion
-changes or updates its backend API periodically, we aim to fix, update and add
-new features to the tool in a timely manner. Any dependent tools or project
-that relied on [csv2notion](https://github.com/vzhd1701/csv2notion), can use
-our **CSV2Notion Neo** tool interchangeably requiring additional augments. ##
-Installation ### Pre-compiled Binary (Recommended) Download the latest release
-of the latest binary release [here](https://github.com/TheAcharya/csv2notion-
-neo/releases). ### With [Homebrew](https://brew.sh/) (Recommended for macOS)
-```bash $ brew install TheAcharya/homebrew-tap/csv2notion-neo ``` ```bash $
-brew uninstall --cask csv2notion-neo ``` ### With PIP ```bash $ pip install --
-user csv2notion_neo ``` **Python 3.7 or later required.** ### From source This
-project uses [poetry](https://python-poetry.org/) for dependency management and
-packaging. You will have to install it first. See [poetry official
-documentation](https://python-poetry.org/docs/) for instructions. ```shell $
-git clone https://github.com/TheAcharya/csv2notion-neo.git $ cd csv2notion_neo/
-$ poetry install --no-dev $ poetry run csv2notion_neo ``` ## Guide ```plain $
-csv2notion_neo --help usage: csv2notion_neo [-h] --token TOKEN [--url URL]
-[OPTION]... FILE https://github.com/TheAcharya/csv2notion-neo Upload & Merge
-CSV or JSON Data with Images to Notion Database positional arguments: FILE CSV
-or JSON file to upload general options: --workspace active Notion workspace
-name --token Notion token, stored in token_v2 cookie for notion.so --url URL
-Notion database URL; if none is provided, will create a new database --max-
-threads upload threads (default: 5) --log FILE file to store program log --
-verbose output debug information --version show program's version number and
-exit -h, --help show this help message and exit column options: --column-types
+data to ensure accuracy - Automatically analyse and generate captions for
+images using Hugging Face's open-source AI/ML models ### Disadvantages over
+native import - Importing each row separately might lead to slower speed - To
+address this, utilise multithreaded upload ## Table of contents - [Background]
+(#background) - [Installation](#installation) - [Pre-compiled Binary
+(Recommended)](#pre-compiled-binary-recommended) - [From Source](#from-source)
+- [Guide](#guide) - [macOS Release](#macos-release) - [Prerequisite]
+(#prerequisite) - [Upload Speed](#upload-speed) - [Duplicate CSV Columns]
+(#duplicate-csv-columns) - [Missing Columns](#missing-columns) - [Column Types]
+(#column-types) - [Mergin](#merging) - [Relation Columns](#relation-columns) -
+[Cover Image & Embedded Image](#cover-image--embedded-image) - [Icons](#icons)
+- [Mandatory Columns](#mandatory-columns) - [AI/ML Options (Hugging Face)]
+(#aiml-options-hugging-face) - [Examples](#examples) - [Credits](#credits) -
+[License](#license) - [Reporting Bugs](#reporting-bugs) ## Background
+Originally, we developed [csv2notion](https://github.com/vzhd1701/csv2notion)
+to address the lack of advanced importing support for `*.csv` files in [Notion]
+(https://notion.so). We took inspiration from [Airtable](https://
+www.airtable.com)âs [CSV import extension](https://support.airtable.com/docs/
+csv-import-extension). **CSV2Notion Neo** was created as a spin-off project to
+address inactivity in the original repository and maintain compatibility with
+Notion. As Notion changes or updates its backend API periodically, we aim to
+fix, update and add new features to the tool in a timely manner. Any dependent
+tools or project that relied on [csv2notion](https://github.com/vzhd1701/
+csv2notion), can use our **CSV2Notion Neo** tool interchangeably requiring
+additional augments. ## Installation ### Pre-compiled Binary (Recommended)
+Download the latest release of the latest binary release [here](https://
+github.com/TheAcharya/csv2notion-neo/releases). ### With [Homebrew](https://
+brew.sh/) (Recommended for macOS) ```bash $ brew install TheAcharya/homebrew-
+tap/csv2notion-neo ``` ```bash $ brew uninstall --cask csv2notion-neo ``` ###
+With PIP ```bash $ pip install --user csv2notion_neo ``` **Python 3.7 or later
+required.** ### From source This project uses [poetry](https://python-
+poetry.org/) for dependency management and packaging. You will have to install
+it first. See [poetry official documentation](https://python-poetry.org/docs/
+) for instructions. ```shell $ git clone https://github.com/TheAcharya/
+csv2notion-neo.git $ cd csv2notion_neo/ $ poetry install --no-dev $ poetry run
+csv2notion_neo ``` ## Guide ```plain $ csv2notion_neo --help usage:
+csv2notion_neo [-h] --token TOKEN [--url URL] [OPTION]... FILE https://
+github.com/TheAcharya/csv2notion-neo Upload & Merge CSV or JSON Data with
+Images to Notion Database positional arguments: FILE CSV or JSON file to upload
+general options: --workspace active Notion workspace name --token Notion token,
+stored in token_v2 cookie for notion.so --url URL Notion database URL; if none
+is provided, will create a new database --max-threads upload threads (default:
+5) --log FILE file to store program log --verbose output debug information --
+version show program's version number and exit -h, --help show this help
+message and exit machine learning options: --hugging-face-token Hugging Face
+token to use image captioning model online --hf-model Provide the model used
+for generating caption
+blip-image| git-large> (defaults: vit-gpt2) --caption-column Provide both image
+column and column where caption would be written column options: --column-types
 comma-separated list of column types to use for non-key columns; if none is
 provided, types will be guessed from CSV values (can also be used with --add-
 missing-columns flag) --add-missing-columns if columns are present in CSV but
 not in Notion DB, add them to Notion DB --rename-notion-key-column rename the
 key column in the file to a different key column in Airtable --randomize-
 select-colors randomize colors for added options in select and multi select
 columns merge options: --merge merge CSV or JSON with existing Notion DB rows,
@@ -229,49 +236,94 @@
 or single emoji. To also treat `--icon-column` as a regular column, use `--
 icon-column-keep` flag, similar to `--image-column-keep`. If you want to set
 the same icon for each row, use the `--default-icon` option. If both `--icon-
 column` and `--default-icon` are present, the default icon is used if the row
 doesn't have anything in the icon column. ### Mandatory Columns If you want to
 ensure that specific columns always have value and are not allowed to be empty,
 then use the `--mandatory-column` option. The program execution will stop if
-validation fails. ## Examples Importing CSV into New Database
+validation fails. ### AI/ML Options (Hugging Face) Hugging Face is a prominent
+AI company known for its contributions to natural language processing (NLP)
+through its comprehensive open-source platform. It offers an extensive library
+called Transformers, which provides pre-trained models for a wide range of NLP
+tasks, including text generation, sentiment analysis, translation, and more.
+These models are based on state-of-the-art architectures like BERT, GPT, and
+T5. The platform fosters a vibrant open-source community where developers and
+researchers can share and collaborate on models. Users can access, fine-tune,
+and deploy a vast array of community-contributed models via the Hugging Face
+Model Hub. This collaborative environment accelerates innovation and
+democratizes access to advanced machine learning tools. Obtaining Hugging Face
+Token
+Steps to Obtain a Hugging Face Token with Write Mode 1. **Create a Hugging Face
+Account (if you don't have one already):** - Go to the [Hugging Face website]
+(https://huggingface.co/). - Click on "Sign Up" in the top right corner. - Fill
+in your details (username, email, password) and complete the registration
+process. 2. **Log In to Your Account:** - If you already have an account,
+simply log in by clicking "Log In" and entering your credentials. 3. **Navigate
+to Your Profile Settings:** - Once logged in, click on your profile icon in the
+top right corner of the page. - From the dropdown menu, select "Settings." 4.
+**Access the API Tokens Section:** - In the settings menu on the left side of
+the screen, find and click on "Access Tokens." 5. **Create a New API Token:** -
+In the "Access Tokens" section, you will see an option to create a new token. -
+Click on "New token." 6. **Set Permissions to Write Mode:** - Provide a name
+for your token (e.g., "MyWriteToken"). - Set the permissions type to "Write"
+type by selecting the "Write" from the dropdown. This will grant the token
+write access, allowing you to perform actions that modify data on Hugging Face.
+7. **Generate and Copy Your Token:** - Click on the "Generate token" button. -
+Your new token will be displayed. Copy it and store it in a secure place, as
+you will need it to access Hugging Face's API services. **Note:** Keep your
+token secure and do not share it publicly, as it grants access to your Hugging
+Face account and its resources.
+Avaliable Model Information
+| Models | Information | Accuracy | | ---------- | ----------------------------
+---------------------------------------- | -------- | | vit-gpt2 | [Link]
+(https://huggingface.co/nlpconnect/vit-gpt2-image-captioning) | Low - Medium |
+| blip-image | [Link](https://huggingface.co/Salesforce/blip-image-captioning-
+base) | Low - Medium | | git-large | [Link](https://huggingface.co/microsoft/
+git-large) | Low - Medium | **Note:** Additional models will be integrated in
+the future from Hugging Face as better models are identified.
+> [!WARNING] > Please be aware that this feature is currently in an
+experimental phase. We strongly advise against uploading sensitive images or
+those of a personal and private nature. Images will be uploaded to Hugging
+Faceâs servers for analysis. We recommend using commercial images, such as
+movie stills or stock photos, for AI captioning. ## Examples Importing CSV into
+New Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_01.png?raw=true]
 Using Custom Column Types
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --column-types "number,multi_select" test.csv ```
+YOUR_TOKEN_HERE \ --column-types "number,multi_select" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_02.png?raw=true]
 Importing CSV into Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_03.gif?raw=true]
 Merging CSV with Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --merge test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --merge test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_04.gif?raw=true]
 Merging CSV with Select Columns in Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_
-TOKEN_HERE --url NOTION URL --merge --merge-only-column "Column 2" --merge-
-onLy-column "Column 3" test.csv ```
+TOKEN_HERE \ --url NOTION URL \ --merge \ --merge-only-column "Column 2" \ --
+merge-onLy-column "Column 3" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_05.gif?raw=true]
 Importing Rows with Images
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --image-column "Image Column" test.csv ```
+YOUR_TOKEN_HERE \ --image-column "Image Column" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_06.gif?raw=true]
 Importing Rows with Images (Multiple Image Column)
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --image-column "Colour Image" "Black & White Image" "Map" --
-image-column-keep --mandatory-column "Cat ID" test.csv ``` Example CSV ```text
+YOUR_TOKEN_HERE \ --image-column "Colour Image" "Black & White Image" "Map" \ -
+-image-column-keep --mandatory-column "Cat ID" test.csv ``` Example CSV ```text
 Cat ID,Animal Name,Location,Colour Image,Black & White Image,Map
 1,Lion,Namibia,Colour/lion.jpg,Black & White/lion.jpg,Map/Namibia.jpg
 2,Tiger,India,Colour/tiger.jpg,Black & White/tiger.jpg,Map/India.jpg
 3,Panther,India,Colour/panther.jpg,Black & White/panther.jpg,Map/India.jpg
 4,Snow Leopard,Nepal,Colour/snow_leopard.jpg,Black & White/
 snow_leopard.jpg,Map/Nepal.jpg 5,Cheetah,South Africa,Colour/cheetah.jpg,Black
 & White/cheetah.jpg,Map/South Africa.jpg 6,Puma,South America,Colour/
@@ -286,36 +338,45 @@
 ââ Map/ â â ââ Brazil.jpg â â ââ India.jpg â â ââ
 Namibia.jpg â â ââ Nepal.jpg â â ââ South Africa.jpg â â
 ââ South America.jpg â â ââ tiger.jpg ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_11.gif?raw=true]
 Importing Rows with Emoji Icons
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --icon-column "Icon Column" test.csv ```
+YOUR_TOKEN_HERE \ --icon-column "Icon Column" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_07.gif?raw=true]
 Updating Emoji Icon Only for All Rows
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --default-icon ð --merge --merge-only-
-column "Key" test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --default-icon ð \ --merge \ --merge-
+only-column "Key" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_08.gif?raw=true]
 Importing JSON into Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
-column "Cat ID" --merge JSON-Demo.json ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --mandatory-column "Cat ID" \ --payload-
+key-column "Cat ID" \ --merge JSON-Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_09.gif?raw=true]
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
-column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
-Demo.json ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --mandatory-column "Cat ID" \ --payload-
+key-column "Cat ID" \ --rename-notion-key-column "Cat ID" "Anything ID" \ --
+merge JSON-Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
+Utilising Hugging Face's AI/ML Model to Automatically Analyse and Generate
+Captions from Images
+```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
+YOUR_TOKEN_HERE --url NOTION_URL --hugging-face-token
+YOUR_HUGGING_FACE_TOKEN_HERE \ --hf-model blip-image \ --caption-column "Image
+Filename" "Frame Description" \ --image-column "Image Filename" \ --image-
+column-keep \ --mandatory-column "Cat ID" \ --merge big_cats.csv ```
+       [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
+                           example_12.gif?raw=true]
 ## Utilised By ### Marker Data Marker Data's Notion Panel
   [https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-
                       database-settings_01.png?raw=true]
 ### [CommandPost](https://commandpost.io) CommandPost's Notion Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/cli.py` & `csv2notion_neo-1.3.0/csv2notion_neo/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 from csv2notion_neo.utils_exceptions import CriticalError, NotionError
 
 logger = logging.getLogger(__name__)
 
 
 def cli(*argv: str) -> None:
     try:
-        ic.disable()
+        ic.enable()
         args = parse_args(argv)
-        
+            
         setup_logging(is_verbose=args.verbose, log_file=args.log)
         logger.info(f"CSV2Notion Neo version {__version__}")
 
         path = Path(args.csv_file).suffix
 
         if "json" in path:
             if not args.payload_key_column:
                 raise CriticalError("Json file found, please enter the key column!")
             
         logger.info(f"Validating {path[1::]} & csv2notion_neo.notion DB schema")
 
         csv_data = LocalData(
-            args.csv_file, args.column_types, args.fail_on_duplicate_csv_columns, args.payload_key_column,
+            args.csv_file, args.column_types, args.fail_on_duplicate_csv_columns, args.payload_key_column,args=args
         )
 
         if not csv_data:
             raise CriticalError(f"{path} file is empty")
 
         client = get_notion_client(
             args.token,
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/cli_args.py` & `csv2notion_neo-1.3.0/csv2notion_neo/cli_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,35 @@
                 "version": f"%(prog)s {__version__}",
             },
             ("-h", "--help"): {
                 "action": "help",
                 "help": "show this help message and exit",
             },
         },
+        "machine learning options":{
+            "--hugging-face-token":{
+                "help": (
+                    "Hugging Face token to use image captioning model online"
+                ),
+                "metavar": "AI",
+            },
+            "--hf-model":{
+                "help": (
+                    "Provide the model used for generating caption <vit-gpt2 | blip-image | git-large> (defaults: vit-gpt2)"
+                ),
+                "metavar": "AI",
+            },
+            "--caption-column":{
+                "help":(
+                    "Provide both image column and column where caption would be written"
+                ),
+                "metavar":"AI",
+                "nargs":2,
+            }
+        },
         "column options": {
             "--column-types": {
                 "help": (
                     "comma-separated list of column types to use for non-key columns;"
                     "\nif none is provided, types will be guessed from CSV values"
                     "\n(can also be used with --add-missing-columns flag)"
                 ),
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/cli_steps.py` & `csv2notion_neo-1.3.0/csv2notion_neo/cli_steps.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/block.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/block.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/client.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/client.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/collection.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/collection.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/logger.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/logger.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/maps.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/maps.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/markdown.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/markdown.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/monitor.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/monitor.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/operations.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/operations.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/records.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/records.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/settings.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/settings.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/smoke_test.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/smoke_test.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/space.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/space.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/store.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/store.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/user.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/user.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/utils.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/utils.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion/utils_ssl.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion/utils_ssl.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_convert.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.rules = conversion_rules
         self._current_row = 0
 
     def convert_to_notion_rows(self, csv_data: LocalData) -> List[NotionUploadRow]:
         notion_rows = []
         # starting with 2nd row, because first is header
         self._current_row = 2
+        self.csv_data = csv_data
 
         for row in csv_data:
 
             if self.rules.rename_notion_key_column:
                 if self.rules.rename_notion_key_column[1] == self.rules.rename_notion_key_column[0]:
                     raise CriticalError(f"Please do not provide same column name in rename-payload-key-column")
                 new_id = self.rules.rename_notion_key_column[1]
@@ -74,14 +75,26 @@
         if self.rules.payload_key_column:
             if self.rules.rename_notion_key_column:
                 new_id = self.rules.rename_notion_key_column[1]
                 properties["payload_key_column"] = new_id
             else:
                 properties["payload_key_column"] = self.rules.payload_key_column
 
+        #ai features
+        if self.rules.hugging_face_token:
+            if self.rules.caption_column:
+                properties['AI'] = {"caption":{
+                    "hftoken":self.rules.hugging_face_token,
+                    "image_path": self.rules.csv_file.parent / Path(row[self.rules.caption_column[0]]),
+                    "caption_column":self.rules.caption_column[1],
+                    "model_url":self.csv_data.model_url
+                }}
+
+        
+
         if self.rules.image_column_mode == "block":
             properties["cover_block"] = self._map_image(row)
             properties["cover_block_caption"] = self._map_image_caption(row)
         else:
             properties["cover"] = self._map_image(row)
 
         properties["icon"] = self._map_icon(row)
@@ -178,17 +191,18 @@
 
             if self.rules.image_column:
         
                 for image_column in self.rules.image_column:
                     image = row.get(image_column, "").strip()
                     if image:
                         image = map_url_or_file(image)
+                        
                         if isinstance(image, Path):
                             image = self._relative_path(image)
-
+                        #ic(image)
                     self._raise_if_mandatory_empty(image_column, image)
 
                     images.append(image)
                     if not self.rules.image_column_keep:
                         row.pop(image_column, None)
             
             return images
@@ -275,14 +289,15 @@
                 f" to upload on csv2notion_neo.notion."
             )
             return None
 
         return ensured_path
 
     def _relative_path(self, path: Path) -> Optional[Path]:
+        #PATH
         search_path = self.rules.files_search_path
 
         if not path.is_absolute():
             path = search_path / path
 
         if not path.exists():
             self._error(f"File {path.name} does not exist.")
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_convert_map.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_convert_map.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_db.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_db_client.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_db_client.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_db_collection.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_db_collection.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_preparator.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_preparator.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_row.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,22 +66,24 @@
             cover_meta = None
         else:
 
             new_image, cover_meta = upload_filetype(self, new_image)
 
         self.cover_meta = cover_meta
         CollectionRowBlock.cover.fset(self, new_image)
+        
 
     @property
     def cover_block(self) -> Optional[str]:
         return self.image_block.url  # type: ignore
 
     @cover_block.setter
     def cover_block(self, image: FileType) -> None:
         
+        
         new_images = []
         if image:
             cover_img = image.pop(0)
         else:
             cover_img = None
         if self._client.in_transaction():
             raise RuntimeError("Cannot set cover_block during atomic transaction")
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_row_image_block.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_row_image_block.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_row_upload_file.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_row_upload_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from icecream import ic
 
 Meta = Dict[str, str]
 
 
 def upload_filetype(parent: Block, filetype: FileType) -> Tuple[str, Meta]:
 
+    #ic(filetype)
     if isinstance(filetype, Path):
         url, meta = upload_file(parent, filetype)
     else:
         url = filetype
         meta = {"type": "url", "url": filetype}
 
     return url, meta
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_type_guess.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_type_guess.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/notion_uploader.py` & `csv2notion_neo-1.3.0/csv2notion_neo/notion_uploader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from dataclasses import dataclass
 from typing import Any, Dict
 
 from csv2notion_neo.notion_db import NotionDB
 from csv2notion_neo.notion_row import CollectionRowBlockExtended
 from icecream import ic
-
+from csv2notion_neo.utils_ai import AI
 
 @dataclass
 class NotionUploadRow(object):
     columns: Dict[str, Any]
     properties: Dict[str, Any]
 
     def key(self) -> str:
         if "payload_key_column" in self.properties:
             if self.properties["payload_key_column"]:
                 return str(self.columns[self.properties["payload_key_column"]])
         return str(list(self.columns.values())[0])
 
-
 class NotionRowUploader(object):
     def __init__(self, db: NotionDB):
         self.db = db
 
     def upload_row(self, row: NotionUploadRow, is_merge: bool) -> None:
 
+        #CHECK
+        if 'AI' in row.properties:
+            ai_client = AI(row.properties['AI'])
+            row.columns = ai_client.out(row.columns)
+        #row.columns['ai caption'] = '2'
         post_properties = _extract_post_properties(row.properties)
 
         db_row = self._get_db_row(row, is_merge)
 
         # these need to be updated after
         # because they can't be updated in atomic transaction
         for prop, prop_val in post_properties.items():
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/utils_ai.py` & `csv2notion_neo-1.3.0/csv2notion_neo/utils_ai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,72 @@
 import shutil, os
 import logging
 from tqdm import tqdm
 from icecream import ic
 import requests
+import time
 
 logger = logging.getLogger(__name__)
 
 class AI:
 
     def __init__(self,ai_data:dict) -> None:
         self.ai_data = ai_data
     
     def out(self,row) -> str:
         
         if 'caption' in self.ai_data:
             data = self.ai_data['caption']
             try:
-                row[data['caption_column']] = self._img2caption(data['hftoken'],str(data['image_path']))
+                row[data['caption_column']] = self._img2caption(data['hftoken'],str(data['image_path']),data['model_url'])
                 return row
             except Exception as e:
                 logger.error(f"Error during AI process : {e}")
 
 
-    def _img2caption(self,token,image_url:str) -> str:
+    def _img2caption(self,token:str,image_url:str,model_url:str) -> str:
         try:
-            sess = requests.session()
             file = open(image_url,'rb')
             filename = os.path.basename(image_url)
             tqdm.write(f"AI generating caption for image {filename}")
 
-            caption = sess.post(
-            'https://api-inference.huggingface.co/models/Salesforce/blip-image-captioning-large',
-            json='None',
-            data=file,
-            headers={'authorization': f'Bearer {token}'},
-            cookies=None,
-            timeout=None,
-            stream=False
-            )
+            retries = 0
+            while True:
+
+                if retries == 15:
+                    tqdm.write(f"Error generating caption for {filename} \n The model size is huge and could have problem loading! try again after some time")
+                    #logger.error(caption.json())
+                    break
+
+                sess = requests.session()
+                caption = sess.post(
+                model_url,
+                json='None',
+                data=file,
+                headers={'authorization': f'Bearer {token}'},
+                cookies=None,
+                timeout=None,
+                stream=False
+                )
+
+                retries += 1
+                if 'error' in caption.json():
+                    if 'estimated_time' in caption.json():
+                        time.sleep(3)
+                    elif 'Error in `parameters`: field required' in caption.json()['error']:
+                        time.sleep(3)
+                    else:
+                        break
+                else:
+                    break
 
             tqdm.write(f"Caption generated for image {filename} : {caption.json()[0]['generated_text']}")
             return caption.json()[0]['generated_text']
         except Exception as e:
             tqdm.write(f"Error generating caption for {filename}")
             logger.error(e,exc_info=1)
+            logger.error(caption.json())
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/utils_db.py` & `csv2notion_neo-1.3.0/csv2notion_neo/utils_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/utils_rand_id.py` & `csv2notion_neo-1.3.0/csv2notion_neo/utils_rand_id.py`

 * *Files identical despite different names*

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/utils_static.py` & `csv2notion_neo-1.3.0/csv2notion_neo/utils_static.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,17 +58,20 @@
     fail_on_conversion_error: bool
     fail_on_inaccessible_relations: bool
     fail_on_missing_columns: bool
     fail_on_unsettable_columns: bool
     fail_on_wrong_status_values: bool
 
     rename_notion_key_column: List[str]
-
     payload_key_column: Optional[str]
 
+    hugging_face_token: Optional[str]
+    caption_column: List[str]
+    hf_model:Optional[str]
+
     @property
     def files_search_path(self) -> Path:
         return self.csv_file.parent
 
     @classmethod
     def from_args(cls, args: Namespace) -> "ConversionRules":
         args_map = {
```

### Comparing `csv2notion_neo-1.2.6/csv2notion_neo/utils_threading.py` & `csv2notion_neo-1.3.0/csv2notion_neo/utils_threading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import threading
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from typing import Any, Callable, Iterable, Iterator
 
 from csv2notion_neo.notion_db import NotionDB
 from csv2notion_neo.notion_db_client import NotionClientExtended
 from csv2notion_neo.notion_uploader import NotionRowUploader
-
+from icecream import ic
 
 class ThreadRowUploader(object):
     def __init__(self, client: NotionClientExtended, collection_id: str) -> None:
         self.thread_data = threading.local()
 
         self.client = client
         self.collection_id = collection_id
 
     def worker(self, *args: Any, **kwargs: Any) -> None:
         try:
             notion_uploader = self.thread_data.uploader
         except AttributeError:
             client = NotionClientExtended(old_client=self.client)
             notion_db = NotionDB(client, self.collection_id)
+            
             notion_uploader = NotionRowUploader(notion_db)
             self.thread_data.uploader = notion_uploader
 
         notion_uploader.upload_row(*args, **kwargs)
 
 
 def process_iter(
```

### Comparing `csv2notion_neo-1.2.6/pyproject.toml` & `csv2notion_neo-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "csv2notion_neo"
-version = "1.2.6"
+version = "1.3.0"
 description = "Upload & Merge CSV Data with Images to Notion Database"
 authors = ["vzhd1701 <vzhd1701@gmail.com>", "Arjun <arjunprakash027@gmail.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 license = "MIT"
 homepage = "https://github.com/TheAcharya/csv2notion-neo"
 repository = "https://github.com/TheAcharya/csv2notion-neo"
```

### Comparing `csv2notion_neo-1.2.6/PKG-INFO` & `csv2notion_neo-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2notion-neo
-Version: 1.2.6
+Version: 1.3.0
 Summary: Upload & Merge CSV Data with Images to Notion Database
 Home-page: https://github.com/TheAcharya/csv2notion-neo
 License: MIT
 Keywords: csv,notion,import,merge
 Author: vzhd1701
 Author-email: vzhd1701@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -76,14 +76,15 @@
 - Choose column types manually instead of letting Notion detecting them automatically
 - Link or create new entries in relation columns based on their values automatically
 - Easily upload files into the designated "Files & Media" column
 - Assign a icon for each row for quick identification
 - Set a cover or embed an image for each row to enhance visual representation
 - Upload image files for covers or icons
 - Apply validation options for input data to ensure accuracy
+- Automatically analyse and generate captions for images using Hugging Face's open-source AI/ML models
 
 ### Disadvantages over native import
  
 - Importing each row separately might lead to slower speed
   - To address this, utilise multithreaded upload
 
 ## Table of contents
@@ -100,14 +101,15 @@
   - [Missing Columns](#missing-columns)
   - [Column Types](#column-types)
   - [Mergin](#merging)
   - [Relation Columns](#relation-columns)
   - [Cover Image & Embedded Image](#cover-image--embedded-image)
   - [Icons](#icons)
   - [Mandatory Columns](#mandatory-columns)
+  - [AI/ML Options (Hugging Face)](#aiml-options-hugging-face)
 - [Examples](#examples)
 - [Credits](#credits)
 - [License](#license)
 - [Reporting Bugs](#reporting-bugs)
 
 ## Background
 
@@ -168,14 +170,19 @@
   --url URL                          Notion database URL; if none is provided, will create a new database
   --max-threads                      upload threads (default: 5)
   --log FILE                         file to store program log
   --verbose                          output debug information
   --version                          show program's version number and exit
   -h, --help                         show this help message and exit
 
+machine learning options:
+  --hugging-face-token              Hugging Face token to use image captioning model online
+  --hf-model                        Provide the model used for generating caption <vit-gpt2 | blip-image| git-large> (defaults: vit-gpt2)
+  --caption-column                  Provide both image column and column where caption would be written
+
 column options:
   --column-types                     comma-separated list of column types to use for non-key columns;
                                      if none is provided, types will be guessed from CSV values
                                      (can also be used with --add-missing-columns flag)
   --add-missing-columns              if columns are present in CSV but not in Notion DB, add them to Notion DB
   --rename-notion-key-column         rename the key column in the file to a different key column in Airtable
   --randomize-select-colors          randomize colors for added options in select and multi select columns
@@ -399,14 +406,74 @@
 
 If you want to set the same icon for each row, use the `--default-icon` option. If both `--icon-column` and `--default-icon` are present, the default icon is used if the row doesn't have anything in the icon column.
 
 ### Mandatory Columns
 
 If you want to ensure that specific columns always have value and are not allowed to be empty, then use the `--mandatory-column` option. The program execution will stop if validation fails.
 
+### AI/ML Options (Hugging Face)
+
+Hugging Face is a prominent AI company known for its contributions to natural language processing (NLP) through its comprehensive open-source platform. It offers an extensive library called Transformers, which provides pre-trained models for a wide range of NLP tasks, including text generation, sentiment analysis, translation, and more. These models are based on state-of-the-art architectures like BERT, GPT, and T5.
+
+The platform fosters a vibrant open-source community where developers and researchers can share and collaborate on models. Users can access, fine-tune, and deploy a vast array of community-contributed models via the Hugging Face Model Hub. This collaborative environment accelerates innovation and democratizes access to advanced machine learning tools.
+
+<details><summary>Obtaining Hugging Face Token</summary>
+<p>
+
+Steps to Obtain a Hugging Face Token with Write Mode
+
+1. **Create a Hugging Face Account (if you don't have one already):**
+   - Go to the [Hugging Face website](https://huggingface.co/).
+   - Click on "Sign Up" in the top right corner.
+   - Fill in your details (username, email, password) and complete the registration process.
+
+2. **Log In to Your Account:**
+   - If you already have an account, simply log in by clicking "Log In" and entering your credentials.
+
+3. **Navigate to Your Profile Settings:**
+   - Once logged in, click on your profile icon in the top right corner of the page.
+   - From the dropdown menu, select "Settings."
+
+4. **Access the API Tokens Section:**
+   - In the settings menu on the left side of the screen, find and click on "Access Tokens."
+
+5. **Create a New API Token:**
+   - In the "Access Tokens" section, you will see an option to create a new token.
+   - Click on "New token."
+
+6. **Set Permissions to Write Mode:**
+   - Provide a name for your token (e.g., "MyWriteToken").
+   - Set the permissions type to "Write" type by selecting the "Write" from the dropdown. This will grant the token write access, allowing you to perform actions that modify data on Hugging Face.
+
+7. **Generate and Copy Your Token:**
+   - Click on the "Generate token" button.
+   - Your new token will be displayed. Copy it and store it in a secure place, as you will need it to access Hugging Face's API services.
+
+**Note:** Keep your token secure and do not share it publicly, as it grants access to your Hugging Face account and its resources.
+
+</p>
+</details>
+
+<details><summary>Avaliable Model Information</summary>
+<p>
+
+| Models      | Information                                                          | Accuracy |
+| ---------- | -------------------------------------------------------------------- | -------- |
+| vit-gpt2   | [Link](https://huggingface.co/nlpconnect/vit-gpt2-image-captioning)  | Low - Medium   |
+| blip-image | [Link](https://huggingface.co/Salesforce/blip-image-captioning-base) | Low - Medium   |
+| git-large  | [Link](https://huggingface.co/microsoft/git-large)                   | Low - Medium   |
+
+**Note:** Additional models will be integrated in the future from Hugging Face as better models are identified.
+
+</p>
+</details>
+
+> [!WARNING]  
+> Please be aware that this feature is currently in an experimental phase. We strongly advise against uploading sensitive images or those of a personal and private nature. Images will be uploaded to Hugging Face’s servers for analysis. We recommend using commercial images, such as movie stills or stock photos, for AI captioning.
+
 ## Examples
 
 <details><summary>Importing CSV into New Database</summary>
 <p>
 
 ```shell
 csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE test.csv
@@ -416,70 +483,81 @@
 </p>
 </details>
 
 <details><summary>Using Custom Column Types</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --column-types "number,multi_select" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --column-types "number,multi_select" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_02.png?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing CSV into Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_03.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Merging CSV with Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --merge test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --merge test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_04.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Merging CSV with Select Columns in Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_ TOKEN_HERE --url NOTION URL --merge --merge-only-column "Column 2" --merge-onLy-column "Column 3" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_ TOKEN_HERE \
+  --url NOTION URL \
+  --merge \
+  --merge-only-column "Column 2" \
+  --merge-onLy-column "Column 3" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_05.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing Rows with Images</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --image-column "Image Column" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+--image-column "Image Column" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_06.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing Rows with Images (Multiple Image Column)</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --image-column "Colour Image" "Black & White Image" "Map" --image-column-keep --mandatory-column "Cat ID" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --image-column "Colour Image" "Black & White Image" "Map" \
+  --image-column-keep --mandatory-column "Cat ID" test.csv
 ```
 
 Example CSV
 
 ```text
 Cat ID,Animal Name,Location,Colour Image,Black & White Image,Map
 1,Lion,Namibia,Colour/lion.jpg,Black & White/lion.jpg,Map/Namibia.jpg
@@ -527,56 +605,88 @@
 </p>
 </details>
 
 <details><summary>Importing Rows with Emoji Icons</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --icon-column "Icon Column" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE  \
+  --icon-column "Icon Column" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_07.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Updating Emoji Icon Only for All Rows</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --default-icon 👍 --merge --merge-only-column "Key" test.csv
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --default-icon 👍 \
+  --merge \
+  --merge-only-column "Key" test.csv
 ```
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_08.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing JSON into Existing Database</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-column "Cat ID" --merge JSON-Demo.json
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --mandatory-column "Cat ID" \
+  --payload-key-column "Cat ID" \
+  --merge JSON-Demo.json
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_09.gif?raw=true"> </p>
 
 </p>
 </details>
 
 <details><summary>Importing JSON into Existing Database with a Different Key Column</summary>
 <p>
 
 ```shell
-csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-Demo.json
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE \
+  --url NOTION_URL \
+  --mandatory-column "Cat ID" \
+  --payload-key-column "Cat ID" \
+  --rename-notion-key-column "Cat ID" "Anything ID" \
+  --merge JSON-Demo.json
 ```
 
 <p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_10.gif?raw=true"> </p>
 
 </p>
 </details>
 
+<details><summary>Utilising Hugging Face's AI/ML Model to Automatically Analyse and Generate Captions from Images</summary>
+<p>
+
+```shell
+csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_TOKEN_HERE --url NOTION_URL --hugging-face-token YOUR_HUGGING_FACE_TOKEN_HERE \
+  --hf-model blip-image \
+  --caption-column "Image Filename" "Frame Description" \
+  --image-column "Image Filename" \
+  --image-column-keep \
+  --mandatory-column "Cat ID" \
+  --merge big_cats.csv
+```
+
+<p align="center"> <img src="https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/example_12.gif?raw=true"> </p>
+
+</p>
+</details>
+
 ## Utilised By
 
 ### Marker Data
 
 <details><summary>Marker Data's Notion Panel</summary>
 <p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.2.6 Summary: Upload &
+Metadata-Version: 2.1 Name: csv2notion-neo Version: 1.3.0 Summary: Upload &
 Merge CSV Data with Images to Notion Database Home-page: https://github.com/
 TheAcharya/csv2notion-neo License: MIT Keywords: csv,notion,import,merge
 Author: vzhd1701 Author-email: vzhd1701@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Operating System :: MacOS Classifier: Operating System :: Microsoft Classifier:
@@ -33,56 +33,63 @@
 JSON with the existing database, using the first column as a key to combine
 existing rows - Choose column types manually instead of letting Notion
 detecting them automatically - Link or create new entries in relation columns
 based on their values automatically - Easily upload files into the designated
 "Files & Media" column - Assign a icon for each row for quick identification -
 Set a cover or embed an image for each row to enhance visual representation -
 Upload image files for covers or icons - Apply validation options for input
-data to ensure accuracy ### Disadvantages over native import - Importing each
-row separately might lead to slower speed - To address this, utilise
-multithreaded upload ## Table of contents - [Background](#background) -
-[Installation](#installation) - [Pre-compiled Binary (Recommended)](#pre-
-compiled-binary-recommended) - [From Source](#from-source) - [Guide](#guide) -
-[macOS Release](#macos-release) - [Prerequisite](#prerequisite) - [Upload
-Speed](#upload-speed) - [Duplicate CSV Columns](#duplicate-csv-columns) -
-[Missing Columns](#missing-columns) - [Column Types](#column-types) - [Mergin]
-(#merging) - [Relation Columns](#relation-columns) - [Cover Image & Embedded
-Image](#cover-image--embedded-image) - [Icons](#icons) - [Mandatory Columns]
-(#mandatory-columns) - [Examples](#examples) - [Credits](#credits) - [License]
-(#license) - [Reporting Bugs](#reporting-bugs) ## Background Originally, we
-developed [csv2notion](https://github.com/vzhd1701/csv2notion) to address the
-lack of advanced importing support for `*.csv` files in [Notion](https://
-notion.so). We took inspiration from [Airtable](https://www.airtable.com)âs
-[CSV import extension](https://support.airtable.com/docs/csv-import-extension).
-**CSV2Notion Neo** was created as a spin-off project to address inactivity in
-the original repository and maintain compatibility with Notion. As Notion
-changes or updates its backend API periodically, we aim to fix, update and add
-new features to the tool in a timely manner. Any dependent tools or project
-that relied on [csv2notion](https://github.com/vzhd1701/csv2notion), can use
-our **CSV2Notion Neo** tool interchangeably requiring additional augments. ##
-Installation ### Pre-compiled Binary (Recommended) Download the latest release
-of the latest binary release [here](https://github.com/TheAcharya/csv2notion-
-neo/releases). ### With [Homebrew](https://brew.sh/) (Recommended for macOS)
-```bash $ brew install TheAcharya/homebrew-tap/csv2notion-neo ``` ```bash $
-brew uninstall --cask csv2notion-neo ``` ### With PIP ```bash $ pip install --
-user csv2notion_neo ``` **Python 3.7 or later required.** ### From source This
-project uses [poetry](https://python-poetry.org/) for dependency management and
-packaging. You will have to install it first. See [poetry official
-documentation](https://python-poetry.org/docs/) for instructions. ```shell $
-git clone https://github.com/TheAcharya/csv2notion-neo.git $ cd csv2notion_neo/
-$ poetry install --no-dev $ poetry run csv2notion_neo ``` ## Guide ```plain $
-csv2notion_neo --help usage: csv2notion_neo [-h] --token TOKEN [--url URL]
-[OPTION]... FILE https://github.com/TheAcharya/csv2notion-neo Upload & Merge
-CSV or JSON Data with Images to Notion Database positional arguments: FILE CSV
-or JSON file to upload general options: --workspace active Notion workspace
-name --token Notion token, stored in token_v2 cookie for notion.so --url URL
-Notion database URL; if none is provided, will create a new database --max-
-threads upload threads (default: 5) --log FILE file to store program log --
-verbose output debug information --version show program's version number and
-exit -h, --help show this help message and exit column options: --column-types
+data to ensure accuracy - Automatically analyse and generate captions for
+images using Hugging Face's open-source AI/ML models ### Disadvantages over
+native import - Importing each row separately might lead to slower speed - To
+address this, utilise multithreaded upload ## Table of contents - [Background]
+(#background) - [Installation](#installation) - [Pre-compiled Binary
+(Recommended)](#pre-compiled-binary-recommended) - [From Source](#from-source)
+- [Guide](#guide) - [macOS Release](#macos-release) - [Prerequisite]
+(#prerequisite) - [Upload Speed](#upload-speed) - [Duplicate CSV Columns]
+(#duplicate-csv-columns) - [Missing Columns](#missing-columns) - [Column Types]
+(#column-types) - [Mergin](#merging) - [Relation Columns](#relation-columns) -
+[Cover Image & Embedded Image](#cover-image--embedded-image) - [Icons](#icons)
+- [Mandatory Columns](#mandatory-columns) - [AI/ML Options (Hugging Face)]
+(#aiml-options-hugging-face) - [Examples](#examples) - [Credits](#credits) -
+[License](#license) - [Reporting Bugs](#reporting-bugs) ## Background
+Originally, we developed [csv2notion](https://github.com/vzhd1701/csv2notion)
+to address the lack of advanced importing support for `*.csv` files in [Notion]
+(https://notion.so). We took inspiration from [Airtable](https://
+www.airtable.com)âs [CSV import extension](https://support.airtable.com/docs/
+csv-import-extension). **CSV2Notion Neo** was created as a spin-off project to
+address inactivity in the original repository and maintain compatibility with
+Notion. As Notion changes or updates its backend API periodically, we aim to
+fix, update and add new features to the tool in a timely manner. Any dependent
+tools or project that relied on [csv2notion](https://github.com/vzhd1701/
+csv2notion), can use our **CSV2Notion Neo** tool interchangeably requiring
+additional augments. ## Installation ### Pre-compiled Binary (Recommended)
+Download the latest release of the latest binary release [here](https://
+github.com/TheAcharya/csv2notion-neo/releases). ### With [Homebrew](https://
+brew.sh/) (Recommended for macOS) ```bash $ brew install TheAcharya/homebrew-
+tap/csv2notion-neo ``` ```bash $ brew uninstall --cask csv2notion-neo ``` ###
+With PIP ```bash $ pip install --user csv2notion_neo ``` **Python 3.7 or later
+required.** ### From source This project uses [poetry](https://python-
+poetry.org/) for dependency management and packaging. You will have to install
+it first. See [poetry official documentation](https://python-poetry.org/docs/
+) for instructions. ```shell $ git clone https://github.com/TheAcharya/
+csv2notion-neo.git $ cd csv2notion_neo/ $ poetry install --no-dev $ poetry run
+csv2notion_neo ``` ## Guide ```plain $ csv2notion_neo --help usage:
+csv2notion_neo [-h] --token TOKEN [--url URL] [OPTION]... FILE https://
+github.com/TheAcharya/csv2notion-neo Upload & Merge CSV or JSON Data with
+Images to Notion Database positional arguments: FILE CSV or JSON file to upload
+general options: --workspace active Notion workspace name --token Notion token,
+stored in token_v2 cookie for notion.so --url URL Notion database URL; if none
+is provided, will create a new database --max-threads upload threads (default:
+5) --log FILE file to store program log --verbose output debug information --
+version show program's version number and exit -h, --help show this help
+message and exit machine learning options: --hugging-face-token Hugging Face
+token to use image captioning model online --hf-model Provide the model used
+for generating caption
+blip-image| git-large> (defaults: vit-gpt2) --caption-column Provide both image
+column and column where caption would be written column options: --column-types
 comma-separated list of column types to use for non-key columns; if none is
 provided, types will be guessed from CSV values (can also be used with --add-
 missing-columns flag) --add-missing-columns if columns are present in CSV but
 not in Notion DB, add them to Notion DB --rename-notion-key-column rename the
 key column in the file to a different key column in Airtable --randomize-
 select-colors randomize colors for added options in select and multi select
 columns merge options: --merge merge CSV or JSON with existing Notion DB rows,
@@ -255,49 +262,94 @@
 or single emoji. To also treat `--icon-column` as a regular column, use `--
 icon-column-keep` flag, similar to `--image-column-keep`. If you want to set
 the same icon for each row, use the `--default-icon` option. If both `--icon-
 column` and `--default-icon` are present, the default icon is used if the row
 doesn't have anything in the icon column. ### Mandatory Columns If you want to
 ensure that specific columns always have value and are not allowed to be empty,
 then use the `--mandatory-column` option. The program execution will stop if
-validation fails. ## Examples Importing CSV into New Database
+validation fails. ### AI/ML Options (Hugging Face) Hugging Face is a prominent
+AI company known for its contributions to natural language processing (NLP)
+through its comprehensive open-source platform. It offers an extensive library
+called Transformers, which provides pre-trained models for a wide range of NLP
+tasks, including text generation, sentiment analysis, translation, and more.
+These models are based on state-of-the-art architectures like BERT, GPT, and
+T5. The platform fosters a vibrant open-source community where developers and
+researchers can share and collaborate on models. Users can access, fine-tune,
+and deploy a vast array of community-contributed models via the Hugging Face
+Model Hub. This collaborative environment accelerates innovation and
+democratizes access to advanced machine learning tools. Obtaining Hugging Face
+Token
+Steps to Obtain a Hugging Face Token with Write Mode 1. **Create a Hugging Face
+Account (if you don't have one already):** - Go to the [Hugging Face website]
+(https://huggingface.co/). - Click on "Sign Up" in the top right corner. - Fill
+in your details (username, email, password) and complete the registration
+process. 2. **Log In to Your Account:** - If you already have an account,
+simply log in by clicking "Log In" and entering your credentials. 3. **Navigate
+to Your Profile Settings:** - Once logged in, click on your profile icon in the
+top right corner of the page. - From the dropdown menu, select "Settings." 4.
+**Access the API Tokens Section:** - In the settings menu on the left side of
+the screen, find and click on "Access Tokens." 5. **Create a New API Token:** -
+In the "Access Tokens" section, you will see an option to create a new token. -
+Click on "New token." 6. **Set Permissions to Write Mode:** - Provide a name
+for your token (e.g., "MyWriteToken"). - Set the permissions type to "Write"
+type by selecting the "Write" from the dropdown. This will grant the token
+write access, allowing you to perform actions that modify data on Hugging Face.
+7. **Generate and Copy Your Token:** - Click on the "Generate token" button. -
+Your new token will be displayed. Copy it and store it in a secure place, as
+you will need it to access Hugging Face's API services. **Note:** Keep your
+token secure and do not share it publicly, as it grants access to your Hugging
+Face account and its resources.
+Avaliable Model Information
+| Models | Information | Accuracy | | ---------- | ----------------------------
+---------------------------------------- | -------- | | vit-gpt2 | [Link]
+(https://huggingface.co/nlpconnect/vit-gpt2-image-captioning) | Low - Medium |
+| blip-image | [Link](https://huggingface.co/Salesforce/blip-image-captioning-
+base) | Low - Medium | | git-large | [Link](https://huggingface.co/microsoft/
+git-large) | Low - Medium | **Note:** Additional models will be integrated in
+the future from Hugging Face as better models are identified.
+> [!WARNING] > Please be aware that this feature is currently in an
+experimental phase. We strongly advise against uploading sensitive images or
+those of a personal and private nature. Images will be uploaded to Hugging
+Faceâs servers for analysis. We recommend using commercial images, such as
+movie stills or stock photos, for AI captioning. ## Examples Importing CSV into
+New Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
 YOUR_TOKEN_HERE test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_01.png?raw=true]
 Using Custom Column Types
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --column-types "number,multi_select" test.csv ```
+YOUR_TOKEN_HERE \ --column-types "number,multi_select" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_02.png?raw=true]
 Importing CSV into Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_03.gif?raw=true]
 Merging CSV with Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --merge test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --merge test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_04.gif?raw=true]
 Merging CSV with Select Columns in Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token YOUR_
-TOKEN_HERE --url NOTION URL --merge --merge-only-column "Column 2" --merge-
-onLy-column "Column 3" test.csv ```
+TOKEN_HERE \ --url NOTION URL \ --merge \ --merge-only-column "Column 2" \ --
+merge-onLy-column "Column 3" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_05.gif?raw=true]
 Importing Rows with Images
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --image-column "Image Column" test.csv ```
+YOUR_TOKEN_HERE \ --image-column "Image Column" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_06.gif?raw=true]
 Importing Rows with Images (Multiple Image Column)
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --image-column "Colour Image" "Black & White Image" "Map" --
-image-column-keep --mandatory-column "Cat ID" test.csv ``` Example CSV ```text
+YOUR_TOKEN_HERE \ --image-column "Colour Image" "Black & White Image" "Map" \ -
+-image-column-keep --mandatory-column "Cat ID" test.csv ``` Example CSV ```text
 Cat ID,Animal Name,Location,Colour Image,Black & White Image,Map
 1,Lion,Namibia,Colour/lion.jpg,Black & White/lion.jpg,Map/Namibia.jpg
 2,Tiger,India,Colour/tiger.jpg,Black & White/tiger.jpg,Map/India.jpg
 3,Panther,India,Colour/panther.jpg,Black & White/panther.jpg,Map/India.jpg
 4,Snow Leopard,Nepal,Colour/snow_leopard.jpg,Black & White/
 snow_leopard.jpg,Map/Nepal.jpg 5,Cheetah,South Africa,Colour/cheetah.jpg,Black
 & White/cheetah.jpg,Map/South Africa.jpg 6,Puma,South America,Colour/
@@ -312,36 +364,45 @@
 ââ Map/ â â ââ Brazil.jpg â â ââ India.jpg â â ââ
 Namibia.jpg â â ââ Nepal.jpg â â ââ South Africa.jpg â â
 ââ South America.jpg â â ââ tiger.jpg ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_11.gif?raw=true]
 Importing Rows with Emoji Icons
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --icon-column "Icon Column" test.csv ```
+YOUR_TOKEN_HERE \ --icon-column "Icon Column" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_07.gif?raw=true]
 Updating Emoji Icon Only for All Rows
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --default-icon ð --merge --merge-only-
-column "Key" test.csv ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --default-icon ð \ --merge \ --merge-
+only-column "Key" test.csv ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_08.gif?raw=true]
 Importing JSON into Existing Database
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
-column "Cat ID" --merge JSON-Demo.json ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --mandatory-column "Cat ID" \ --payload-
+key-column "Cat ID" \ --merge JSON-Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_09.gif?raw=true]
 Importing JSON into Existing Database with a Different Key Column
 ```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
-YOUR_TOKEN_HERE --url NOTION_URL --mandatory-column "Cat ID" --payload-key-
-column "Cat ID" --rename-notion-key-column "Cat ID" "Anything ID" --merge JSON-
-Demo.json ```
+YOUR_TOKEN_HERE \ --url NOTION_URL \ --mandatory-column "Cat ID" \ --payload-
+key-column "Cat ID" \ --rename-notion-key-column "Cat ID" "Anything ID" \ --
+merge JSON-Demo.json ```
        [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
                            example_10.gif?raw=true]
+Utilising Hugging Face's AI/ML Model to Automatically Analyse and Generate
+Captions from Images
+```shell csv2notion_neo --workspace YOUR_WORKSPACE_NAME_HERE --token
+YOUR_TOKEN_HERE --url NOTION_URL --hugging-face-token
+YOUR_HUGGING_FACE_TOKEN_HERE \ --hf-model blip-image \ --caption-column "Image
+Filename" "Frame Description" \ --image-column "Image Filename" \ --image-
+column-keep \ --mandatory-column "Cat ID" \ --merge big_cats.csv ```
+       [https://github.com/TheAcharya/csv2notion-neo/blob/master/assets/
+                           example_12.gif?raw=true]
 ## Utilised By ### Marker Data Marker Data's Notion Panel
   [https://github.com/TheAcharya/MarkerData-Website/blob/main/docs/assets/md-
                       database-settings_01.png?raw=true]
 ### [CommandPost](https://commandpost.io) CommandPost's Notion Toolbox
   [https://github.com/CommandPost/CommandPost-Website/blob/main/docs/static/
                          toolbox-notion.png?raw=true]
 ## Credits Original Idea and Workflow Architecture by [Vigneswaran Rajkumar]
```

