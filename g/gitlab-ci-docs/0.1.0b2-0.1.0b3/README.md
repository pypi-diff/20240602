# Comparing `tmp/gitlab_ci_docs-0.1.0b2.tar.gz` & `tmp/gitlab_ci_docs-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_ci_docs-0.1.0b2.tar", last modified: Tue May 28 21:20:11 2024, max compression
+gzip compressed data, was "gitlab_ci_docs-0.1.0b3.tar", last modified: Sun Jun  2 19:19:26 2024, max compression
```

## Comparing `gitlab_ci_docs-0.1.0b2.tar` & `gitlab_ci_docs-0.1.0b3.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 21:20:11.992696 gitlab_ci_docs-0.1.0b2/
--rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 gitlab_ci_docs-0.1.0b2/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 gitlab_ci_docs-0.1.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0     3838 2024-05-28 21:20:11.992696 gitlab_ci_docs-0.1.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     3244 2024-05-28 19:08:29.000000 gitlab_ci_docs-0.1.0b2/README.md
--rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 gitlab_ci_docs-0.1.0b2/pyproject.toml
--rw-rw-rw-   0        0        0      828 2024-05-28 21:20:11.992696 gitlab_ci_docs-0.1.0b2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 21:20:11.961454 gitlab_ci_docs-0.1.0b2/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 21:20:11.992696 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/
--rw-rw-rw-   0        0        0     3838 2024-05-28 21:20:11.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2024-05-28 21:20:11.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 21:20:11.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 18:52:21.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-28 21:20:11.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-28 21:20:11.000000 gitlab_ci_docs-0.1.0b2/src/gitlab_ci_docs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 21:20:11.992696 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/
--rw-rw-rw-   0        0        0      163 2024-05-28 21:19:40.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/__init__.py
--rw-rw-rw-   0        0        0      831 2024-05-25 15:37:55.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/__main__.py
--rw-rw-rw-   0        0        0     2697 2024-05-28 20:46:04.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/docsbuilder.py
--rw-rw-rw-   0        0        0     1543 2024-05-28 19:05:40.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/docsgen.py
--rw-rw-rw-   0        0        0       86 2024-04-01 16:26:26.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/errors.py
--rw-rw-rw-   0        0        0     4152 2024-05-28 20:36:43.000000 gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/pipelineparser.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:19:26.132963 gitlab_ci_docs-0.1.0b3/
+-rw-rw-rw-   0        0        0     1092 2024-03-29 11:49:25.000000 gitlab_ci_docs-0.1.0b3/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-01 16:26:26.000000 gitlab_ci_docs-0.1.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4267 2024-06-02 19:19:26.132963 gitlab_ci_docs-0.1.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     3673 2024-06-02 08:02:35.000000 gitlab_ci_docs-0.1.0b3/README.md
+-rw-rw-rw-   0        0        0       88 2024-04-01 16:26:26.000000 gitlab_ci_docs-0.1.0b3/pyproject.toml
+-rw-rw-rw-   0        0        0      828 2024-06-02 19:19:26.132963 gitlab_ci_docs-0.1.0b3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-02 19:19:26.086099 gitlab_ci_docs-0.1.0b3/src/
+drwxrwxrwx   0        0        0        0 2024-06-02 19:19:26.132963 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/
+-rw-rw-rw-   0        0        0     4267 2024-06-02 19:19:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2024-06-02 19:19:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-02 19:19:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 18:52:21.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-06-02 19:19:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-02 19:19:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlab_ci_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-02 19:19:26.117343 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/
+-rw-rw-rw-   0        0        0      163 2024-06-02 18:23:26.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/__init__.py
+-rw-rw-rw-   0        0        0      945 2024-06-02 19:05:54.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/__main__.py
+-rw-rw-rw-   0        0        0     3012 2024-06-02 19:09:07.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/docsbuilder.py
+-rw-rw-rw-   0        0        0     1887 2024-06-02 17:33:29.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/docsgen.py
+-rw-rw-rw-   0        0        0       83 2024-05-31 17:08:46.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/errors.py
+drwxrwxrwx   0        0        0        0 2024-06-02 19:19:26.132963 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/
+-rw-rw-rw-   0        0        0      550 2024-06-02 09:00:09.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/__init__.py
+-rw-rw-rw-   0        0        0      555 2024-06-02 09:03:36.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/globalvariables.py
+-rw-rw-rw-   0        0        0     1276 2024-06-02 18:21:44.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/rule.py
+-rw-rw-rw-   0        0        0     2465 2024-06-02 19:09:03.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/variable.py
+-rw-rw-rw-   0        0        0      623 2024-06-02 18:36:09.000000 gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/workflow.py
```

### Comparing `gitlab_ci_docs-0.1.0b2/LICENSE` & `gitlab_ci_docs-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_ci_docs-0.1.0b2/README.md` & `gitlab_ci_docs-0.1.0b3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-## Overview
-
-The CI/CD solution by gitlba is great, however it has some limitations. The way how a pipeline is defined is definitelly one of thme. There's nothing woring about YAML itself, but gitlab pipeline is so complex to be written in a markup language.
-
-For instance, let's assume there is the design where we want to trigger a pipeline from web UI or by API call. The pipeline consumes variables as input. There is no way how to define variable's type, options or if it's required or if it shouldn't be overriden. This sort of information is always part of a documentation. This package provides functionality to create simple documentation of *workflow* section, which can contain all of these infromation.
+## Motivation
+Let's assume the design when we want to trigger a pipeline from web UI or by an API call. The pipeline consumes variables as input. It would be very helpful to know the type of a variable or its valid options. This kind of information is usually part of the documentation. This package provides functionality to automate the creation of this documentation.
 
-In my opinion, the *workflow* section should be part of every clean/nice pipeline definition ("code").
-Let's define the naming convention, which covers some scenarios, and all other information write to comment. I know, comments sound awful, but it is the most safe way to achieve what we need.
+<img alt="Generated table example" src="doc/table_sample.PNG">
 
-## How does it work
+## Overview
 The output of this script is simple description (documentation) of *workflow* section. It parses workflow section and inserts it to readme file. Currently, output documentation is only as html table.
-
-### Readme file
-By default, the script inserts generated table in the beggining of the file. However, it is possible to mark position in the file where the table will be inserted. The mark token is *\<!--PIPELINE_DOCS-->*
-
-If token is present, the table is insreted below it.
+<br>Properties of variables are defined in comment using the format described in following section.
 
 ### Variable definition
 As mentioned before, we write all parameters of a variable to a comment. Format of a comment is very simple.
 1. **first part** describes if variable is required on input. By default a variable is considered as optional. To "set" is as required, put *required* to the comment - *# required*
 1. **second part** descibes variable's type or valid options.
     - **type** - starts with colon. Typename can be whatever made up. *:type*
     - **choices** - dev|test
@@ -27,27 +19,57 @@
 #### Example
 ```yaml
 ENV: dev  # required dev|test|prod
 ACCOUNT_ALIAS: null  # required :str
 IMAGE_TAG: 0.1.0  # :version
 ```
 
+### Pipeline name
+Using of the pipeline name improves readability of pipeline runs and also describes the task executed by the pipeline.
+
+Variable **PIPELINE_NAME** is showed in the separated column of the table.
+
 ## Usage
-The tool can be used from command line or imported as module in a code. It requires only two parameters on input:
-- path to yaml file containing thw *workflow* section
-- path to documentation file where generated table is inserted to
+The tool can be used from command line or imported as module in a code. Output is written to the readme file.
+
+### Insert to the Readme
+By default, the script inserts generated table in the beggining of the file. However, it is possible to mark position in the file where the table will be inserted. The mark token is <br>*\<!--PIPELINE_DOCS-->*
+
+If token is present, the table is insreted below it.
 
 ### Command line
-The packegs is called **gitlabcidocs** and consumes following arguments:
-- **--ci-file [**_optional_**]**
-<br>Path to the file containing workflow section.
-<br>Default value is *.gitlab-ci.yml*
-- **--doc-file [**_optional_**]**
-<br>Path to the output file.
-<br>Default value is *README.md*
+The package  **gitlabcidocs** consumes following arguments:
+<ul>
+    <li><b>--ci-file</b> <i>[optional]</i></li>
+    <ul style="list-style-type:none;">
+        <li>Path to the file containing workflow section.</li>
+        <li>Default value is <i>.gitlab-ci.yml</i></li>
+    </ul>
+</ul>
+<ul>
+    <li><b>--doc-file</b> <i>[optional]</i></li>
+    <ul style="list-style-type:none;">
+        <li>Path to the output file.</li>
+        <li>Default value is <i>README.md</i></li>
+    </ul>
+</ul>
+<ul>
+    <li><b>--include-all-rules, -a</b> <i>[optional]</i></li>
+    <ul style="list-style-type:none;">
+        <li>If set to *true*, all rules in the workflow section are included. Otherwise only rules which includes $CI_PIPELINE_SOURCE==web|api|pipeline in the if statement are documented.</li>
+        <li>Default is <i>true</i></li>
+    </ul>
+</ul>
+<ul>
+    <li><b>--include-global-vars, -g</b> <i>[optional]</i></li>
+    <ul style="list-style-type:none;">
+        <li>If set, global variables section is included.</li>
+        <li>Default value is <i>false</i></li>
+    </ul>
+</ul>
 
 ```bash
 python -m gitlabcidocs --ci-file my_workflow.yml --doc-file myREADME.md
 ```
 
 ### Import in code
 The module *gitlab-ci-docs* contains *create_docs* function. The functions consumes the same arguments as cli tool, but there are no default values set.
```

### Comparing `gitlab_ci_docs-0.1.0b2/setup.cfg` & `gitlab_ci_docs-0.1.0b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/__main__.py` & `gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 import argparse
 import docsgen
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--include-all-rules', required=False, default=True, action='store_true', help='If true, document all workflow rules. Otherwise only rules with $CI_PIPELINE_SOURCE=web|pipeline|api are included')
-    parser.add_argument('--ci-file', required=False, default='.gitlab-ci.yml', help='Path to gitlab-ci.yml')
-    parser.add_argument('--doc-file', required=False, default='README.md', help='Path to the file in the docs are injected to')
+    parser.add_argument('--ci-file', default='.gitlab-ci.yml', help='Path to gitlab-ci.yml')
+    parser.add_argument('--doc-file', default='README.md', help='Path to the file in the docs are injected to')
+    parser.add_argument('--include-all-rules', '-a', action='store_true', help='If set, include all workflow rules. Otherwise only rules with $CI_PIPELINE_SOURCE=web|pipeline|api are included')
+    parser.add_argument('--include-global-vars', '-g', action='store_true', help='If set, global variables section is included')
     return parser.parse_args()
 
 
 if __name__ == '__main__':
     args = parse_arguments()
 
-    docsgen.create_docs(args.ci_file, args.doc_file, args.include_all_rules)
+    docsgen.create_docs(
+        args.ci_file, args.doc_file, args.include_all_rules, args.include_global_vars
+    )
```

### Comparing `gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/docsbuilder.py` & `gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/docsbuilder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 from typing import List, Dict
-from pipelineparser import Workflow, Rule, Variable
+from pipelineparser.workflow import Workflow
+from pipelineparser.rule import Rule
+from pipelineparser.variable import Variable
+from pipelineparser.globalvariables import GlobalVariables
 
 
 class HTMLBuilder:
 
-    def __init__(self, workflow: Workflow):
-        self._show_pipelinename_column = False
+    def get_workflow_table(self, workflow: Workflow) -> str:
         headers = ['Trigger', 'Variable', 'Default value', 'Required', 'Type', 'Choices']
         if workflow.pipeline_name_in_rules:
             headers.insert(0, 'Pipeline name')
-            self._show_pipelinename_column = True
-        self._docs = self.table(headers, workflow.rules)
 
-    @property
-    def docs(self) -> str:
-        return self._docs
+        return '\n'.join([
+            '<b>Pipeline worflow</b>',
+            '<table>',
+            self.headers(*headers),
+            '\n'.join([self.create_rule_rows(r, workflow.pipeline_name_in_rules) for r in workflow.rules]),
+            '</table>'
+        ])
+
+    def get_global_vars_table(self, globalvars: GlobalVariables) -> str:
+        return '\n'.join([
+            '<b>Global variables</b>',
+            '<table>',
+            self.headers('Name', 'Value', 'Required', 'Type', 'Choices'),
+            '\n'.join([self.row(self.get_variable_cells(v)) for v in globalvars.variables]),
+            '</table>'
+        ])
 
-    def get_variable_cells(self, variable: Variable, is_mutable: bool) -> List[Dict[str, str]]:
+    def get_variable_cells(self, variable: Variable) -> List[Dict[str, str]]:
         cells = [
             {'value': variable.name},
             {'value': variable.value}
         ]
-        if is_mutable:
+        if not variable.is_const and variable.is_described:
             cells += [
                 {'value': variable.required_str},
                 {'value': variable.typename if variable.typename else '-'},
                 {'value': variable.choices_str if variable.choices_str else '-'}
             ]
         return cells
 
     def get_trigger_cell(self, rule: Rule) -> str:
         return '<br>'.join([i for i in [
             f'<b>if:</b> {rule.condition}' if rule.condition else '',
             f'<b>when:</b> {rule.when}' if rule.when else ''
         ] if i])
 
-    def create_rule_rows(self, rule: Rule) -> str:
+    def create_rule_rows(self, rule: Rule, pipelinename_column: bool) -> str:
         rowspan = len(rule.variables) if rule.variables else 1
-        pipeline_name_cell = [{'value': rule.pipeline_name, 'rowspan': rowspan}] if self._show_pipelinename_column else []
+        pipeline_name_cell = [{'value': rule.pipeline_name, 'rowspan': rowspan}] if pipelinename_column else []
 
         first_row = self.row(
             pipeline_name_cell
             + [{'value': self.get_trigger_cell(rule), 'rowspan': rowspan}]
-            + (self.get_variable_cells(rule.variables[0], rule.is_mutable) if rule.variables else [])
+            + (self.get_variable_cells(rule.variables[0]) if rule.variables else [])
         )
-        other_rows = '\n'.join([self.row(self.get_variable_cells(v, rule.is_mutable)) for v in rule.variables[1:]])
+        other_rows = '\n'.join([self.row(self.get_variable_cells(v)) for v in rule.variables[1:]])
 
         return first_row + other_rows
 
-    def table(self, headers: List[str], rules: List[Rule]) -> str:
-        return '\n'.join([
-            '<table>',
-            self.headers(headers),
-            '\n'.join([self.create_rule_rows(r) for r in rules]),
-            '</table>'
-        ])
-
-    def headers(self, headers: List[str]) -> str:
+    def headers(self, *headers: List[str]) -> str:
         return f'<tr>{"".join([f"<th>{h}</th>" for h in headers])}</tr>'
 
     def row(self, data: List[Dict[str, str]]) -> str:
         return f'<tr>{"".join([self.cell(v["value"], v.get("rowspan", None)) for v in data])}</tr>'
 
     def cell(self, value: str, rowspan=None) -> str:
         rowspan = f' rowspan="{rowspan}"' if rowspan and rowspan > 1 else ''
```

### Comparing `gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/docsgen.py` & `gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/docsgen.py`

 * *Files 26% similar despite different names*

```diff
@@ -36,15 +36,27 @@
         out_lines.insert(begin_docs_line_idx+1, f'{docs}\n{docs_token}\n\n')
     else:
         out_lines = out_lines[:begin_docs_line_idx+1] + [docs+'\n'] + out_lines[end_docs_line_idx:]
 
     write_doc_file(doc_file_path, ''.join(out_lines))
 
 
-def create_docs(ci_file_path: str|Path, doc_file_path: str|Path, include_all_rules: bool) -> str:
-    workflow = pipelineparser.CiFileParser(ci_file_path).get_workflow(include_all_rules)
-    docs = docsbuilder.HTMLBuilder(workflow).docs
-    insert_to_doc_file(docs, doc_file_path)
-    return docs
+def create_docs(
+        ci_file_path: str|Path,
+        doc_file_path: str|Path,
+        include_all_rules: bool = False,
+        include_global_vars: bool = False) -> str:
+    ci_parser = pipelineparser.CiFileParser(ci_file_path)
+    htmlbuilder = docsbuilder.HTMLBuilder()
+
+    workflow = ci_parser.get_workflow(include_all_rules)
+    result_html = htmlbuilder.get_workflow_table(workflow)
+    if include_global_vars:
+        global_vars = ci_parser.get_global_variables()
+        result_html += '\n' + htmlbuilder.get_global_vars_table(global_vars)
+
+    insert_to_doc_file(result_html, doc_file_path)
+
+    return result_html
```

### Comparing `gitlab_ci_docs-0.1.0b2/src/gitlabcidocs/pipelineparser.py` & `gitlab_ci_docs-0.1.0b3/src/gitlabcidocs/pipelineparser/variable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import re
-from ruamel.yaml import YAML
-from typing import Dict, List
-from errors import BadVariableCommentFormatError
+from typing import List
+from errors import VariableCommentFormatError
 
 
 class Variable:
 
     _regex_value_regex = '[a-zA-Z0-9-_\.]'
     _regex_group_req = '(?P<required>required\s?)?'
     _regex_group_type = '(?P<type>:[a-zA-Z]+)?'
     _regex_group_opt = property(lambda s: f'(?P<options>{s._regex_value_regex}+(\|{s._regex_value_regex}+)*)?')
     _regex = property(lambda s: f'^#\s*{s._regex_group_req}{s._regex_group_type}{s._regex_group_opt}$')
 
-    def __init__(self, name: str, value: str, comment: str):
+    def __init__(self, name: str, value: str, comment: str, const: bool = False):
         self._name = name
         self._value = value
         self._required = False
         self._choices = []
         self._typename = ''
+        self._is_const = const
+        self._is_described = False
 
         if (comment := comment.strip()) and comment != '#':
             if (matched := re.fullmatch(self._regex, comment)) is None:
-                raise BadVariableCommentFormatError(f'Variable comment ({comment}) has invalid format. Valid format: {self._regex}')
+                raise VariableCommentFormatError(f'Variable comment ({comment}) has invalid format. Valid format: {self._regex}')
             if matched['options'] and matched['type']:
-                raise BadVariableCommentFormatError(f'Variable comment ({comment}) has invalid format. Valid format: {self._regex}')
+                raise VariableCommentFormatError(f'Variable comment ({comment}) has invalid format. Valid format: {self._regex}')
 
+            self._is_described = True
             self._required = bool(matched['required'])
             self._choices = list(set(matched['options'].split('|'))) if matched['options'] else []
             self._typename = matched['type'][1:] if matched['type'] else None
 
     @property
     def name(self) -> str:
         return self._name
@@ -61,73 +63,14 @@
     def choices_str(self) -> str:
         return ', '.join(self._choices) if self._choices else ''
 
     @property
     def typename(self) -> str:
         return self._typename
 
-
-class Rule:
-
-    _regex_pipeline_source = '\$CI_PIPELINE_SOURCE\s==\s[\'"]?(web|pipeline|api|trigger)[\'"]?'
-
-    def __init__(self, rule: Dict):
-        self._pipeline_name = ''
-        self._condition = rule.get('if', None)
-        self._when = rule.get('when', None)
-        self._variables = [
-            Variable(
-                name=key,
-                value=rule['variables'][key],
-                comment=c[2].value if (c := rule['variables'].ca.items.get(key, None)) else ''
-            ) for key in rule.get('variables', {}) if key != 'PIPELINE_NAME'
-        ]
-        self._pipeline_name = rule.get('variables', {}).get('PIPELINE_NAME', '')
-
-    @property
-    def is_mutable(self) -> bool:
-        return bool(re.search(self._regex_pipeline_source, self.condition))
-
     @property
-    def condition(self) -> str:
-        return self._condition
+    def is_const(self) -> bool:
+        return self._is_const or self.name.startswith('_')
 
     @property
-    def when(self):
-        return self._when
-
-    @property
-    def variables(self) -> List[Variable]:
-        return self._variables
-
-    @property
-    def pipeline_name(self) -> str:
-        return self._pipeline_name
-
-
-class Workflow:
-
-    def __init__(self, workflow: Dict, include_all_rules: bool):
-        self._pipeline_name = workflow.get('name', '')
-        self._rules = [rule for rule in [Rule(r) for r in workflow['rules']] if include_all_rules or rule.is_mutable]
-
-    @property
-    def rules(self) -> List[Rule]:
-        return self._rules
-
-    @property
-    def pipeline_name(self) -> str:
-        return self._pipeline_name
-
-    @property
-    def pipeline_name_in_rules(self):
-        return any(r.pipeline_name for r in self.rules)
-
-
-class CiFileParser:
-
-    def __init__(self, filepath: str):
-        with open(filepath) as f:
-            self._pipeline = YAML().load(f)
-
-    def get_workflow(self, include_all_rules: bool) -> Workflow:
-        return Workflow(self._pipeline['workflow'], include_all_rules)
+    def is_described(self) -> bool:
+        return self._is_described
```

