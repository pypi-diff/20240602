# Comparing `tmp/kaizen_cloudcode-0.1.9.tar.gz` & `tmp/kaizen_cloudcode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.9.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.2.0.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.9.tar` & `kaizen_cloudcode-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/LICENSE
--rw-r--r--   0        0        0     4089 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/README.md
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.008617 kaizen_cloudcode-0.1.9/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1463 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3594 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7039 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     2526 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     4195 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1528 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     2248 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-22 23:32:11.012616 kaizen_cloudcode-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-06-02 00:41:00.356246 kaizen_cloudcode-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4639 2024-06-02 00:41:00.356246 kaizen_cloudcode-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3768 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     2980 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7612 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     5550 2024-06-02 00:41:00.360246 kaizen_cloudcode-0.2.0/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     6285 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     2079 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-06-02 00:41:00.364246 kaizen_cloudcode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5870 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.2.0/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.9/LICENSE` & `kaizen_cloudcode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.9/README.md` & `kaizen_cloudcode-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,99 @@
 <p align="center">
   <a href="https://github.com/Cloud-Code-AI/">
     <img src="https://img.shields.io/github/stars/Cloud-Code-AI/cloudcode" alt="Github Stars">
   </a>
   <a href="https://github.com/Cloud-Code-AI/cloudcode/pulse">
     <img src="https://img.shields.io/github/commit-activity/w/Cloud-Code-AI/cloudcode" alt="Commits-per-week">
   </a>
+    <a href="https://discord.gg/W33Hh5yWpj">
+    <img src="https://img.shields.io/discord/1156434217966764033.svg?style=social&logo=discord" alt="Discord">
+    </a>
   <a href="https://opensource.org/license/agpl-v3">
     <img src="https://img.shields.io/badge/License-AGPL%20v3-blue.svg" alt="License: AGPL-3.0">
   </a>
 </p>
 
 # Kaizen
 
-Kaizen is an open-source project that helps teams ensure quality in their software delivery by providing a suite of tools for code review, test generation, and end-to-end testing. It integrates with your existing code repositories and workflows, allowing you to streamline your software development process.
+Kaizen is an open-source project that helps teams ensure quality in their software delivery by providing an AI-powered suite of tools for code review, test generation, and end-to-end testing. It seamlessly integrates with your existing code repositories and workflows, allowing you to streamline your software development process and catch bugs early.
+
+[![Book a Demo](https://img.shields.io/badge/Book%20a%20Demo-Book%20Now-brightgreen)](https://www.cloudcode.ai/book-a-demo.html) [![Join the Waitlist](https://img.shields.io/badge/Join%20the%20Waitlist-Sign%20Up-blue)](https://cloudcode.ai/#cta)
+
 
 ## Features
 
 ### End-to-End Testing
 
-Kaizen generates comprehensive end-to-end tests based on your application's code and documentation. These tests ensure that your application functions correctly from start to finish, catching regressions and edge cases that may have been overlooked during development.
+Kaizen leverages advanced AI techniques to generate comprehensive end-to-end tests based on your application's code and documentation. These tests ensure that your application functions correctly from start to finish, catching regressions and edge cases that may have been overlooked during development.
 
 ### UI Testing and Review
 
-Kaizen can provide teams with helpful reviews for their UI and generate necessary tests to ensure that their website works as expected.
+Kaizen provides teams with insightful reviews for their UI components and automatically generates necessary tests to ensure that their website works as expected, reducing the risk of visual and functional regressions.
 
 ### Code Review
 
-Kaizen automatically reviews pull requests, summarizes code changes and provides insightful feedback on potential issues or areas of improvement. It leverages advanced natural language processing techniques to understand the context and implications of the code changes.
-
+Kaizen automatically reviews pull requests, summarizes code changes, and provides insightful feedback on potential issues or areas of improvement. It leverages advanced natural language processing techniques to understand the context and implications of the code changes, helping developers write better, more maintainable code.
 
 ## File Structure
 
 - `github_app`: Contains the API server used by the GitHub app to process and respond to incoming requests.
 - `kaizen`: Contains the main logic for interaction with LLMs and data processing.
-  - `actors`: Contains classes used to process various different actions like Code Review and Test execution.
+  - `actors`: Contains classes used to process various actions like Code Review and Test execution.
   - `generators`: Contains the main logic for generative use cases like test case generation, description generation, etc.
   - `llms`: Contains LLM integrations.
 - `docs`: Contains Nextra-powered documentation for the project.
 - `examples`: Contains sample code for various use cases.
 
 ## Getting Started
 
 To get started with Kaizen, follow these steps:
 
-1. Install Kaizen package:
-
-    ```bash
-      pip install kaizen-cloudcode
-    ```
+1. Install the Kaizen package:
 
-2. Copy the example code from `examples/basic`
+```
+pip install kaizen-cloudcode
+```
 
+2. Copy the example code from `examples/basic`.
 3. Generate tests for your website:
+   First, you need to update the URL in the `examples/basic/generate.py`.
+
+```
+PYTHONPATH=. poetry run python examples/basic/generate.py
+```
 
-    First, you need to update the URL in the `examples/basic/generate.py`
-    ```bash
-      PYTHONPATH=. poetry run python examples/basic/generate.py
-    ```
-  
-    Kaizen will generate all the tests and store them inside `.kaizen/tests/`
+Kaizen will generate all the tests and store them inside `.kaizen/tests/`.
 
 4. Execute tests:
+   Once you have generated all the necessary tests, you can run all the tests in two of the following ways:
+
+```
+PYTHONPATH=. poetry run python examples/basic/execute.py
+```
 
-    Once you have generated all the necessary tests, you can run all the tests in two ways:
-    ```bash
-      PYTHONPATH=. poetry run python examples/basic/execute.py
-    ```
-
-    Or using the default pytest module:
-   ```
-     pytest -v .kaizen/tests/
-   ```
-  
-    Kaizen will generate all the tests and store them inside `.kaizen/tests/`
+Or using the default pytest module:
 
+```
+pytest -v .kaizen/ui-tests/
+```
 
-### Running API Server for GitHub App
+Kaizen will execute the generated tests and provide detailed reports.
 
-Kaizen utilizes a GitHub app to perform actions like PR review and description updates. Here is a quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md)
+## Running API Server for GitHub App
+
+Kaizen utilizes a GitHub app to perform actions like PR review and description updates. Here's a quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md)
 
 Deploy the API using Docker Compose:
+
 ```
 docker-compose up
 ```
 
-You can also configure features by tweaking the config.json file.
+You can also configure features by tweaking the `config.json` file.
 
 **NOTE:** You need to create a `.env` file by copying `.env.example` and also store the PEM file for the GitHub app as `GITHUB_APP_KEY.pem`.
 
 ## Contributing
 
 We welcome contributions from the community! If you'd like to contribute to Kaizen, please follow these steps:
 
@@ -96,12 +101,12 @@
 2. Create a new branch (`git checkout -b feature/my-feature`)
 3. Commit your changes (`git commit -m 'Add some feature'`)
 4. Push to the branch (`git push origin feature/my-feature`)
 5. Open a Pull Request
 
 ## License
 
-Kaizen is released under the [AGPL License](LICENSE).
+Kaizen is released under the AGPL License.
 
 ## Contact
 
 If you have any questions or need further assistance, please feel free to contact us at support@cloudcode.ai.
```

#### html2text {}

```diff
@@ -1,47 +1,53 @@
-              _[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _A_G_P_L_-_3_._0_]
+         _[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_D_i_s_c_o_r_d_]_[_L_i_c_e_n_s_e_:_ _A_G_P_L_-_3_._0_]
 # Kaizen Kaizen is an open-source project that helps teams ensure quality in
-their software delivery by providing a suite of tools for code review, test
-generation, and end-to-end testing. It integrates with your existing code
-repositories and workflows, allowing you to streamline your software
-development process. ## Features ### End-to-End Testing Kaizen generates
-comprehensive end-to-end tests based on your application's code and
-documentation. These tests ensure that your application functions correctly
-from start to finish, catching regressions and edge cases that may have been
-overlooked during development. ### UI Testing and Review Kaizen can provide
-teams with helpful reviews for their UI and generate necessary tests to ensure
-that their website works as expected. ### Code Review Kaizen automatically
-reviews pull requests, summarizes code changes and provides insightful feedback
-on potential issues or areas of improvement. It leverages advanced natural
-language processing techniques to understand the context and implications of
-the code changes. ## File Structure - `github_app`: Contains the API server
-used by the GitHub app to process and respond to incoming requests. - `kaizen`:
-Contains the main logic for interaction with LLMs and data processing. -
-`actors`: Contains classes used to process various different actions like Code
-Review and Test execution. - `generators`: Contains the main logic for
+their software delivery by providing an AI-powered suite of tools for code
+review, test generation, and end-to-end testing. It seamlessly integrates with
+your existing code repositories and workflows, allowing you to streamline your
+software development process and catch bugs early. [![Book a Demo](https://
+img.shields.io/badge/Book%20a%20Demo-Book%20Now-brightgreen)](https://
+www.cloudcode.ai/book-a-demo.html) [![Join the Waitlist](https://
+img.shields.io/badge/Join%20the%20Waitlist-Sign%20Up-blue)](https://
+cloudcode.ai/#cta) ## Features ### End-to-End Testing Kaizen leverages advanced
+AI techniques to generate comprehensive end-to-end tests based on your
+application's code and documentation. These tests ensure that your application
+functions correctly from start to finish, catching regressions and edge cases
+that may have been overlooked during development. ### UI Testing and Review
+Kaizen provides teams with insightful reviews for their UI components and
+automatically generates necessary tests to ensure that their website works as
+expected, reducing the risk of visual and functional regressions. ### Code
+Review Kaizen automatically reviews pull requests, summarizes code changes, and
+provides insightful feedback on potential issues or areas of improvement. It
+leverages advanced natural language processing techniques to understand the
+context and implications of the code changes, helping developers write better,
+more maintainable code. ## File Structure - `github_app`: Contains the API
+server used by the GitHub app to process and respond to incoming requests. -
+`kaizen`: Contains the main logic for interaction with LLMs and data
+processing. - `actors`: Contains classes used to process various actions like
+Code Review and Test execution. - `generators`: Contains the main logic for
 generative use cases like test case generation, description generation, etc. -
 `llms`: Contains LLM integrations. - `docs`: Contains Nextra-powered
 documentation for the project. - `examples`: Contains sample code for various
 use cases. ## Getting Started To get started with Kaizen, follow these steps:
-1. Install Kaizen package: ```bash pip install kaizen-cloudcode ``` 2. Copy the
-example code from `examples/basic` 3. Generate tests for your website: First,
-you need to update the URL in the `examples/basic/generate.py` ```bash
+1. Install the Kaizen package: ``` pip install kaizen-cloudcode ``` 2. Copy the
+example code from `examples/basic`. 3. Generate tests for your website: First,
+you need to update the URL in the `examples/basic/generate.py`. ```
 PYTHONPATH=. poetry run python examples/basic/generate.py ``` Kaizen will
-generate all the tests and store them inside `.kaizen/tests/` 4. Execute tests:
-Once you have generated all the necessary tests, you can run all the tests in
-two ways: ```bash PYTHONPATH=. poetry run python examples/basic/execute.py ```
-Or using the default pytest module: ``` pytest -v .kaizen/tests/ ``` Kaizen
-will generate all the tests and store them inside `.kaizen/tests/` ### Running
-API Server for GitHub App Kaizen utilizes a GitHub app to perform actions like
-PR review and description updates. Here is a quick link to set up your own
-GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md) Deploy the API
-using Docker Compose: ``` docker-compose up ``` You can also configure features
-by tweaking the config.json file. **NOTE:** You need to create a `.env` file by
-copying `.env.example` and also store the PEM file for the GitHub app as
-`GITHUB_APP_KEY.pem`. ## Contributing We welcome contributions from the
-community! If you'd like to contribute to Kaizen, please follow these steps: 1.
-Fork the repository 2. Create a new branch (`git checkout -b feature/my-
-feature`) 3. Commit your changes (`git commit -m 'Add some feature'`) 4. Push
-to the branch (`git push origin feature/my-feature`) 5. Open a Pull Request ##
-License Kaizen is released under the [AGPL License](LICENSE). ## Contact If you
-have any questions or need further assistance, please feel free to contact us
-at support@cloudcode.ai.
+generate all the tests and store them inside `.kaizen/tests/`. 4. Execute
+tests: Once you have generated all the necessary tests, you can run all the
+tests in two of the following ways: ``` PYTHONPATH=. poetry run python
+examples/basic/execute.py ``` Or using the default pytest module: ``` pytest -
+v .kaizen/ui-tests/ ``` Kaizen will execute the generated tests and provide
+detailed reports. ## Running API Server for GitHub App Kaizen utilizes a GitHub
+app to perform actions like PR review and description updates. Here's a quick
+link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/
+github_app.md) Deploy the API using Docker Compose: ``` docker-compose up ```
+You can also configure features by tweaking the `config.json` file. **NOTE:**
+You need to create a `.env` file by copying `.env.example` and also store the
+PEM file for the GitHub app as `GITHUB_APP_KEY.pem`. ## Contributing We welcome
+contributions from the community! If you'd like to contribute to Kaizen, please
+follow these steps: 1. Fork the repository 2. Create a new branch (`git
+checkout -b feature/my-feature`) 3. Commit your changes (`git commit -m 'Add
+some feature'`) 4. Push to the branch (`git push origin feature/my-feature`) 5.
+Open a Pull Request ## License Kaizen is released under the AGPL License. ##
+Contact If you have any questions or need further assistance, please feel free
+to contact us at support@cloudcode.ai.
```

### Comparing `kaizen_cloudcode-0.1.9/kaizen/generator/ui.py` & `kaizen_cloudcode-0.2.0/kaizen/generator/ui.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 )
 
 
 class UITestGenerator:
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self.provider = LLMProvider(system_prompt=UI_TESTS_SYSTEM_PROMPT)
+        self.custom_model = None
+        if self.provider.models and "best" in self.provider.models:
+            self.custom_model = self.provider.models["best"]
+            if "type" in self.custom_model:
+                del self.custom_model["type"]
 
     def generate_ui_tests(
         self,
         web_url: str,
         folder_path: Optional[str] = "",
     ):
         """
@@ -41,15 +46,15 @@
         return html
 
     def identify_modules(self, web_content: str, user: Optional[str] = None):
         """
         This method identifies the different UI modules from a webpage.
         """
         prompt = UI_MODULES_PROMPT.format(WEB_CONTENT=web_content)
-        resp, usage = self.provider.chat_completion(prompt, user=user)
+        resp, usage = self.provider.chat_completion(prompt, user=user, custom_model=self.custom_model)
         modules = parser.extract_multi_json(resp)
         return {"modules": modules, "usage": usage}
 
     def generate_playwright_code(
         self,
         web_content: str,
         test_description: str,
@@ -59,15 +64,15 @@
         """
         This method generates playwright code for a particular UI test.
         """
         prompt = PLAYWRIGHT_CODE_PROMPT.format(
             WEB_CONTENT=web_content, TEST_DESCRIPTION=test_description, URL=web_url
         )
 
-        resp, usage = self.provider.chat_completion(prompt, user=user)
+        resp, usage = self.provider.chat_completion(prompt, user=user, custom_model=self.custom_model)
 
         return {"code": resp, "usage": usage}
 
     def generate_module_tests(self, web_content: str, test_modules: dict, web_url: str):
         """
         This method generates UI testing points for all modules.
         """
@@ -88,15 +93,15 @@
         return ui_tests, total_usage
 
     def store_tests_files(self, json_tests: list, folder_path: str = ""):
 
         if not folder_path:
             folder_path = output.get_parent_folder()
 
-        folder_path = os.path.join(folder_path, ".kaizen/tests")
+        folder_path = os.path.join(folder_path, ".kaizen/ui-tests")
         output.create_folder(folder_path)
         output.create_test_files(json_tests, folder_path)
 
     def run_tests(self, ui_tests: dict):
         """
         This method runs playwright tests and updates logs and status accordingly.
         """
```

### Comparing `kaizen_cloudcode-0.1.9/kaizen/helpers/general.py` & `kaizen_cloudcode-0.2.0/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.9/kaizen/helpers/output.py` & `kaizen_cloudcode-0.2.0/kaizen/helpers/output.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,52 +9,31 @@
 from kaizen.helpers import general
 
 logger = logging.getLogger(__name__)
 
 
 PR_COLLAPSIBLE_TEMPLATE = """
 <details>
-<summary>[{confidence}] -> {reasoning}</summary>
-</details>
+<summary><strong>[{confidence}]<strong> -> {comment}</summary> \n
+</strong> Potential Solution:</strong> \n\n{solution}
+\n
+<blockquote>  
+    <p><code>{file_name} | {start_line} - {end_line}</code></p>  
+  </blockquote>  
+</details> \n
+
 """
 
 DESC_COLLAPSIBLE_TEMPLATE = """
 <details>
 <summary>Original Description</summary>
 {desc}
 </details>
-"""
-
 
-def merge_topics(reviews):
-    topics = {}
-    for review in reviews:
-        if review["topic"] in topics:
-            topics[review["topic"]].append(review)
-        else:
-            topics[review["topic"]] = [review]
-    return topics
-
-
-def create_pr_review_from_json(reviews):
-    markdown_output = "## Code Review Feedback\n\n"
-
-    topics = merge_topics(reviews)
-
-    for topic, reviews in topics.items():
-        markdown_output += f"### {topic}\n\n"
-        for review in reviews:
-            ct = PR_COLLAPSIBLE_TEMPLATE.format(
-                comment=review.get("comment", "NA"),
-                reasoning=review.get("reasoning", "NA"),
-                confidence=review.get("confidence", "NA"),
-            )
-            markdown_output += ct + "\n"
-
-    return markdown_output
+"""
 
 
 def create_pr_description(data, original_desc):
     markdown_output = data["desc"]
     markdown_output += "\n\n> ✨ Generated with love by Kaizen ❤️"
     markdown_output += "\n\n" + DESC_COLLAPSIBLE_TEMPLATE.format(desc=original_desc)
     return markdown_output
```

### Comparing `kaizen_cloudcode-0.1.9/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.2.0/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.9/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.2.0/kaizen/llms/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,121 +4,127 @@
 Provide constructive feedback and suggestions for improvements, considering best practices, error handling, performance, readability, and maintainability. 
 Be thorough, objective, and respectful in your reviews, focusing on helping developers improve their skills and code quality. 
 Ask clarifying questions if needed.
 """
 
 CODE_REVIEW_PROMPT = """
 You are an experienced software engineer tasked with reviewing a pull request.
-Your goal is to provide a comprehensive code review that evaluates the code changes, identifies potential issues,
-and provides constructive feedback to the developer.
+Your goal is to provide a concise and actionable code review that evaluates the code changes, identifies potential issues, and provides constructive feedback to the developer.
 
-Using the provided information, generate a detailed code review with feedback organized as a JSON object. Only include sections with relevant feedback, omitting sections without feedback. Follow this structure:
+Using the provided information, generate a code review with feedback organized as a JSON object. Only include sections with relevant feedback, omitting sections without feedback. Follow this structure:
 {{
   "review": [
     {{
       "topic": "<SECTION_TOPIC>",
-      "comment": "<CONCISE_FEEDBACK>",
-      "confidence": <CONFIDENCE_LEVEL>,
-      "reasoning": "<BRIEF_EXPLANATION>"
+      "comment": "<CONCISE_ACTIONABLE_FEEDBACK>",
+      "confidence": "<CONFIDENCE_LEVEL>",
+      "solution": "<SOLUTION_TO_THE_COMMENT>",
+      "start_line": "<CODE_START_LINE_INTEGER>",
+      "end_line": "<CODE_END_LINE_INTEGER>",
+      "file_name": "<CODE_FILE_NAME>",
     }},
     ...
   ]
 }}
 
-Here are the Confidence Levels:
+Here are the Confidence Levels based on severity of the issue:
 [
   "critical",
   "important",
   "moderate",
   "low",
   "trivial"
 ]
 
 Potential section topics:
 - "Code Quality"
 - "Performance" 
 - "Potential Issues"
 - "Improvements"
 
-Generate all possible feedbacks.
-For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed. Use markdown code blocks to quote relevant snippets of code when necessary.
-Keep comments short but make sure it has actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
+Generate all relevant and actionable feedback. Avoid duplicate feedbacks for same line, try to merge them.
+For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed for each comment. Use markdown code blocks to quote relevant snippets of code when necessary.
+Keep comments concise but make sure they have actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
+
+If there is no feedback, return an empty JSON object: {{"review": []}}
+
 
 INFORMATION:
 Pull Request Title: {PULL_REQUEST_TITLE}
 Pull Request Description: {PULL_REQUEST_DESC}
 
 Code Diff:
 ```{CODE_DIFF}```
 """
 
 FILE_CODE_REVIEW_PROMPT = """
 You are an experienced software engineer tasked with reviewing a pull request.
-Your goal is to provide a comprehensive code review that evaluates the code changes, identifies potential issues or areas for improvement,
-and provides constructive feedback to the developer.
+Your goal is to provide a concise and actionable code review that evaluates the code changes, identifies potential issues, and provides constructive feedback to the developer.
 
-Using the provided information, generate a detailed code review with feedback organized as a JSON object. Only include sections with relevant feedback, omitting sections without feedback. Follow this structure:
+Using the provided information, generate a code review with feedback organized as a JSON object. Only include sections with relevant feedback, omitting sections without feedback. Follow this structure:
 {{
   "review": [
     {{
       "topic": "<SECTION_TOPIC>",
-      "comment": "<CONCISE_FEEDBACK>",
-      "confidence": <CONFIDENCE_LEVEL>,
-      "reasoning": "<BRIEF_EXPLANATION>"
+      "comment": "<CONCISE_ACTIONABLE_FEEDBACK>",
+      "confidence": "<CONFIDENCE_LEVEL>",
+      "solution": "<SOLUTION_TO_THE_COMMENT>",
+      "start_line": "<CODE_START_LINE_INTEGER>",
+      "end_line": "<CODE_END_LINE_INTEGER>",
+      "file_name": "<CODE_FILE_NAME>",
     }},
     ...
   ]
 }}
 
-Here are the Confidence Levels:
+Here are the Confidence Levels based on severity of the issue:
 [
   "critical",
   "important",
   "moderate",
   "low",
   "trivial"
 ]
 
 Potential section topics:
 - "Code Quality"
 - "Performance" 
 - "Potential Issues"
 - "Improvements"
 
-Generate all possible feedbacks.
-For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed. Use markdown code blocks to quote relevant snippets of code when necessary.
-Keep comments short but make sure it has actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
+Generate all relevant and actionable feedback. Avoid duplicate feedbacks for same line, try to merge them.
+For each piece of feedback, clearly reference the specific file(s) and line number(s) of code being addressed for each comment. Use markdown code blocks to quote relevant snippets of code when necessary.
+Keep comments concise but make sure they have actionable points pointing to the code or line having the issue. Avoid duplicate feedback, merge when necessary.
+
+If there is no feedback, return an empty JSON object: {{"review": []}}
+
 
 INFORMATION:
 Pull Request Title: {PULL_REQUEST_TITLE}
 Pull Request Description: {PULL_REQUEST_DESC}
 
 File PATCH:
 ```{FILE_PATCH}```
 """
 
 PR_DESCRIPTION_PROMPT = """
 You are a skilled developer reviewing a pull request.
+Using the provided information, generate a concise description for this pull request, covering:
 
-Using the provided information, generate a comprehensive description for this pull request. Cover the following points:
-
-1. Summarize the main purpose and scope of the changes.
-2. Highlight any significant modifications, refactoring, or new features introduced.
+Main purpose and scope of changes
+Significant modifications, refactoring, or new features
 
-Provide output in following format:
+Provide output in the format:
 {{"desc": "<PR_DESCRIPTION_IN_MARKDOWN>"}}
-
-Your description should be clear, concise, and tailored to help reviewers understand the pull request's impact and make an informed decision.
-
+Keep the description clear and tailored to help reviewers understand the pull request's impact, but avoid unnecessary details.
 INFORMATION:
 Pull Request Title: {PULL_REQUEST_TITLE}
 Pull Request Description: {PULL_REQUEST_DESC}
-
 Code Diff:
-```{CODE_DIFF}```
+{CODE_DIFF}
 
 """
 # TODO: Rephrase prompt to make it more clear and accurate.
 UI_MODULES_PROMPT = """
 Assign yourself as a quality assurance engineer. Read this code and design comprehensive tests to test the UI
 of this html. Break it down into 5-10 separate modules and return the output as JSON with the following keys:
 id - serial number to identify
```

### Comparing `kaizen_cloudcode-0.1.9/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.2.0/kaizen/reviewer/work_summarizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,26 +15,37 @@
     def generate_work_summaries(
         self,
         diff_file_data: List[Dict],
         user: Optional[str] = None,
     ):
         available_tokens = self.provider.available_tokens(WORK_SUMMARY_PROMPT)
         summaries = []
+        # Try to merge the files untill LLM can process the response
         combined_diff_data = ""
         total_usage = None
         for file_dict in diff_file_data:
             temp_prompt = combined_diff_data
             temp_prompt += f"""\n---->\nFile Name: {file_dict["file"]}\nPatch: {file_dict["patch"]}\n Status: {file_dict["status"]}"""
+
+            # If available tokens is greated than the new prompt size, process it.
             if available_tokens - self.provider.get_token_count(temp_prompt) > 0:
                 combined_diff_data = temp_prompt
                 continue
 
             # Process the prompt
             prompt = WORK_SUMMARY_PROMPT.format(PATCH_DATA=combined_diff_data)
             response, usage = self.provider.chat_completion(prompt, user=user)
+            total_usage = self.provider.update_usage(total_usage, usage)
+            summaries.append(response)
+            combined_diff_data = ""
+
+        if combined_diff_data != "":
+            # process the remaining file diff pending
+            prompt = WORK_SUMMARY_PROMPT.format(PATCH_DATA=combined_diff_data)
+            response, usage = self.provider.chat_completion(prompt, user=user)
             summaries.append(response)
             combined_diff_data = ""
             total_usage = self.provider.update_usage(total_usage, usage)
 
         if len(summaries) > 1:
             # TODO Merge summaries
             pass
```

### Comparing `kaizen_cloudcode-0.1.9/kaizen/utils/config.py` & `kaizen_cloudcode-0.2.0/kaizen/utils/config.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.9/pyproject.toml` & `kaizen_cloudcode-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.9"
+version = "0.2.0"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.9/PKG-INFO` & `kaizen_cloudcode-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.9
+Version: 0.2.0
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -30,94 +30,99 @@
 <p align="center">
   <a href="https://github.com/Cloud-Code-AI/">
     <img src="https://img.shields.io/github/stars/Cloud-Code-AI/cloudcode" alt="Github Stars">
   </a>
   <a href="https://github.com/Cloud-Code-AI/cloudcode/pulse">
     <img src="https://img.shields.io/github/commit-activity/w/Cloud-Code-AI/cloudcode" alt="Commits-per-week">
   </a>
+    <a href="https://discord.gg/W33Hh5yWpj">
+    <img src="https://img.shields.io/discord/1156434217966764033.svg?style=social&logo=discord" alt="Discord">
+    </a>
   <a href="https://opensource.org/license/agpl-v3">
     <img src="https://img.shields.io/badge/License-AGPL%20v3-blue.svg" alt="License: AGPL-3.0">
   </a>
 </p>
 
 # Kaizen
 
-Kaizen is an open-source project that helps teams ensure quality in their software delivery by providing a suite of tools for code review, test generation, and end-to-end testing. It integrates with your existing code repositories and workflows, allowing you to streamline your software development process.
+Kaizen is an open-source project that helps teams ensure quality in their software delivery by providing an AI-powered suite of tools for code review, test generation, and end-to-end testing. It seamlessly integrates with your existing code repositories and workflows, allowing you to streamline your software development process and catch bugs early.
+
+[![Book a Demo](https://img.shields.io/badge/Book%20a%20Demo-Book%20Now-brightgreen)](https://www.cloudcode.ai/book-a-demo.html) [![Join the Waitlist](https://img.shields.io/badge/Join%20the%20Waitlist-Sign%20Up-blue)](https://cloudcode.ai/#cta)
+
 
 ## Features
 
 ### End-to-End Testing
 
-Kaizen generates comprehensive end-to-end tests based on your application's code and documentation. These tests ensure that your application functions correctly from start to finish, catching regressions and edge cases that may have been overlooked during development.
+Kaizen leverages advanced AI techniques to generate comprehensive end-to-end tests based on your application's code and documentation. These tests ensure that your application functions correctly from start to finish, catching regressions and edge cases that may have been overlooked during development.
 
 ### UI Testing and Review
 
-Kaizen can provide teams with helpful reviews for their UI and generate necessary tests to ensure that their website works as expected.
+Kaizen provides teams with insightful reviews for their UI components and automatically generates necessary tests to ensure that their website works as expected, reducing the risk of visual and functional regressions.
 
 ### Code Review
 
-Kaizen automatically reviews pull requests, summarizes code changes and provides insightful feedback on potential issues or areas of improvement. It leverages advanced natural language processing techniques to understand the context and implications of the code changes.
-
+Kaizen automatically reviews pull requests, summarizes code changes, and provides insightful feedback on potential issues or areas of improvement. It leverages advanced natural language processing techniques to understand the context and implications of the code changes, helping developers write better, more maintainable code.
 
 ## File Structure
 
 - `github_app`: Contains the API server used by the GitHub app to process and respond to incoming requests.
 - `kaizen`: Contains the main logic for interaction with LLMs and data processing.
-  - `actors`: Contains classes used to process various different actions like Code Review and Test execution.
+  - `actors`: Contains classes used to process various actions like Code Review and Test execution.
   - `generators`: Contains the main logic for generative use cases like test case generation, description generation, etc.
   - `llms`: Contains LLM integrations.
 - `docs`: Contains Nextra-powered documentation for the project.
 - `examples`: Contains sample code for various use cases.
 
 ## Getting Started
 
 To get started with Kaizen, follow these steps:
 
-1. Install Kaizen package:
-
-    ```bash
-      pip install kaizen-cloudcode
-    ```
+1. Install the Kaizen package:
 
-2. Copy the example code from `examples/basic`
+```
+pip install kaizen-cloudcode
+```
 
+2. Copy the example code from `examples/basic`.
 3. Generate tests for your website:
+   First, you need to update the URL in the `examples/basic/generate.py`.
+
+```
+PYTHONPATH=. poetry run python examples/basic/generate.py
+```
 
-    First, you need to update the URL in the `examples/basic/generate.py`
-    ```bash
-      PYTHONPATH=. poetry run python examples/basic/generate.py
-    ```
-  
-    Kaizen will generate all the tests and store them inside `.kaizen/tests/`
+Kaizen will generate all the tests and store them inside `.kaizen/tests/`.
 
 4. Execute tests:
+   Once you have generated all the necessary tests, you can run all the tests in two of the following ways:
+
+```
+PYTHONPATH=. poetry run python examples/basic/execute.py
+```
 
-    Once you have generated all the necessary tests, you can run all the tests in two ways:
-    ```bash
-      PYTHONPATH=. poetry run python examples/basic/execute.py
-    ```
-
-    Or using the default pytest module:
-   ```
-     pytest -v .kaizen/tests/
-   ```
-  
-    Kaizen will generate all the tests and store them inside `.kaizen/tests/`
+Or using the default pytest module:
 
+```
+pytest -v .kaizen/ui-tests/
+```
 
-### Running API Server for GitHub App
+Kaizen will execute the generated tests and provide detailed reports.
 
-Kaizen utilizes a GitHub app to perform actions like PR review and description updates. Here is a quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md)
+## Running API Server for GitHub App
+
+Kaizen utilizes a GitHub app to perform actions like PR review and description updates. Here's a quick link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md)
 
 Deploy the API using Docker Compose:
+
 ```
 docker-compose up
 ```
 
-You can also configure features by tweaking the config.json file.
+You can also configure features by tweaking the `config.json` file.
 
 **NOTE:** You need to create a `.env` file by copying `.env.example` and also store the PEM file for the GitHub app as `GITHUB_APP_KEY.pem`.
 
 ## Contributing
 
 We welcome contributions from the community! If you'd like to contribute to Kaizen, please follow these steps:
 
@@ -125,13 +130,13 @@
 2. Create a new branch (`git checkout -b feature/my-feature`)
 3. Commit your changes (`git commit -m 'Add some feature'`)
 4. Push to the branch (`git push origin feature/my-feature`)
 5. Open a Pull Request
 
 ## License
 
-Kaizen is released under the [AGPL License](LICENSE).
+Kaizen is released under the AGPL License.
 
 ## Contact
 
 If you have any questions or need further assistance, please feel free to contact us at support@cloudcode.ai.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.9 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.2.0 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -11,54 +11,60 @@
 cryptography (>=42.0.5,<43.0.0) Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: flake8 (>=7.0.0,<8.0.0) Requires-Dist: fuzzywuzzy
 (>=0.18.0,<0.19.0) Requires-Dist: litellm (>=1.34.42,<2.0.0) Requires-Dist:
 nest-asyncio (>=1.6.0,<2.0.0) Requires-Dist: pip (>=24.0,<25.0) Requires-Dist:
 pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pytest-playwright (>=0.4.4,<0.5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn
 (>=0.29.0,<0.30.0) Description-Content-Type: text/markdown
-              _[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_L_i_c_e_n_s_e_:_ _A_G_P_L_-_3_._0_]
+         _[_G_i_t_h_u_b_ _S_t_a_r_s_]_[_C_o_m_m_i_t_s_-_p_e_r_-_w_e_e_k_]_[_D_i_s_c_o_r_d_]_[_L_i_c_e_n_s_e_:_ _A_G_P_L_-_3_._0_]
 # Kaizen Kaizen is an open-source project that helps teams ensure quality in
-their software delivery by providing a suite of tools for code review, test
-generation, and end-to-end testing. It integrates with your existing code
-repositories and workflows, allowing you to streamline your software
-development process. ## Features ### End-to-End Testing Kaizen generates
-comprehensive end-to-end tests based on your application's code and
-documentation. These tests ensure that your application functions correctly
-from start to finish, catching regressions and edge cases that may have been
-overlooked during development. ### UI Testing and Review Kaizen can provide
-teams with helpful reviews for their UI and generate necessary tests to ensure
-that their website works as expected. ### Code Review Kaizen automatically
-reviews pull requests, summarizes code changes and provides insightful feedback
-on potential issues or areas of improvement. It leverages advanced natural
-language processing techniques to understand the context and implications of
-the code changes. ## File Structure - `github_app`: Contains the API server
-used by the GitHub app to process and respond to incoming requests. - `kaizen`:
-Contains the main logic for interaction with LLMs and data processing. -
-`actors`: Contains classes used to process various different actions like Code
-Review and Test execution. - `generators`: Contains the main logic for
+their software delivery by providing an AI-powered suite of tools for code
+review, test generation, and end-to-end testing. It seamlessly integrates with
+your existing code repositories and workflows, allowing you to streamline your
+software development process and catch bugs early. [![Book a Demo](https://
+img.shields.io/badge/Book%20a%20Demo-Book%20Now-brightgreen)](https://
+www.cloudcode.ai/book-a-demo.html) [![Join the Waitlist](https://
+img.shields.io/badge/Join%20the%20Waitlist-Sign%20Up-blue)](https://
+cloudcode.ai/#cta) ## Features ### End-to-End Testing Kaizen leverages advanced
+AI techniques to generate comprehensive end-to-end tests based on your
+application's code and documentation. These tests ensure that your application
+functions correctly from start to finish, catching regressions and edge cases
+that may have been overlooked during development. ### UI Testing and Review
+Kaizen provides teams with insightful reviews for their UI components and
+automatically generates necessary tests to ensure that their website works as
+expected, reducing the risk of visual and functional regressions. ### Code
+Review Kaizen automatically reviews pull requests, summarizes code changes, and
+provides insightful feedback on potential issues or areas of improvement. It
+leverages advanced natural language processing techniques to understand the
+context and implications of the code changes, helping developers write better,
+more maintainable code. ## File Structure - `github_app`: Contains the API
+server used by the GitHub app to process and respond to incoming requests. -
+`kaizen`: Contains the main logic for interaction with LLMs and data
+processing. - `actors`: Contains classes used to process various actions like
+Code Review and Test execution. - `generators`: Contains the main logic for
 generative use cases like test case generation, description generation, etc. -
 `llms`: Contains LLM integrations. - `docs`: Contains Nextra-powered
 documentation for the project. - `examples`: Contains sample code for various
 use cases. ## Getting Started To get started with Kaizen, follow these steps:
-1. Install Kaizen package: ```bash pip install kaizen-cloudcode ``` 2. Copy the
-example code from `examples/basic` 3. Generate tests for your website: First,
-you need to update the URL in the `examples/basic/generate.py` ```bash
+1. Install the Kaizen package: ``` pip install kaizen-cloudcode ``` 2. Copy the
+example code from `examples/basic`. 3. Generate tests for your website: First,
+you need to update the URL in the `examples/basic/generate.py`. ```
 PYTHONPATH=. poetry run python examples/basic/generate.py ``` Kaizen will
-generate all the tests and store them inside `.kaizen/tests/` 4. Execute tests:
-Once you have generated all the necessary tests, you can run all the tests in
-two ways: ```bash PYTHONPATH=. poetry run python examples/basic/execute.py ```
-Or using the default pytest module: ``` pytest -v .kaizen/tests/ ``` Kaizen
-will generate all the tests and store them inside `.kaizen/tests/` ### Running
-API Server for GitHub App Kaizen utilizes a GitHub app to perform actions like
-PR review and description updates. Here is a quick link to set up your own
-GitHub App: [docs/pages/github_app.md](docs/pages/github_app.md) Deploy the API
-using Docker Compose: ``` docker-compose up ``` You can also configure features
-by tweaking the config.json file. **NOTE:** You need to create a `.env` file by
-copying `.env.example` and also store the PEM file for the GitHub app as
-`GITHUB_APP_KEY.pem`. ## Contributing We welcome contributions from the
-community! If you'd like to contribute to Kaizen, please follow these steps: 1.
-Fork the repository 2. Create a new branch (`git checkout -b feature/my-
-feature`) 3. Commit your changes (`git commit -m 'Add some feature'`) 4. Push
-to the branch (`git push origin feature/my-feature`) 5. Open a Pull Request ##
-License Kaizen is released under the [AGPL License](LICENSE). ## Contact If you
-have any questions or need further assistance, please feel free to contact us
-at support@cloudcode.ai.
+generate all the tests and store them inside `.kaizen/tests/`. 4. Execute
+tests: Once you have generated all the necessary tests, you can run all the
+tests in two of the following ways: ``` PYTHONPATH=. poetry run python
+examples/basic/execute.py ``` Or using the default pytest module: ``` pytest -
+v .kaizen/ui-tests/ ``` Kaizen will execute the generated tests and provide
+detailed reports. ## Running API Server for GitHub App Kaizen utilizes a GitHub
+app to perform actions like PR review and description updates. Here's a quick
+link to set up your own GitHub App: [docs/pages/github_app.md](docs/pages/
+github_app.md) Deploy the API using Docker Compose: ``` docker-compose up ```
+You can also configure features by tweaking the `config.json` file. **NOTE:**
+You need to create a `.env` file by copying `.env.example` and also store the
+PEM file for the GitHub app as `GITHUB_APP_KEY.pem`. ## Contributing We welcome
+contributions from the community! If you'd like to contribute to Kaizen, please
+follow these steps: 1. Fork the repository 2. Create a new branch (`git
+checkout -b feature/my-feature`) 3. Commit your changes (`git commit -m 'Add
+some feature'`) 4. Push to the branch (`git push origin feature/my-feature`) 5.
+Open a Pull Request ## License Kaizen is released under the AGPL License. ##
+Contact If you have any questions or need further assistance, please feel free
+to contact us at support@cloudcode.ai.
```

