# Comparing `tmp/displaylang-0.23.0b1.tar.gz` & `tmp/displaylang-0.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "displaylang-0.23.0b1.tar", last modified: Sun Jan 15 19:51:20 2023, max compression
+gzip compressed data, was "displaylang-0.24.0.tar", last modified: Sun Jun  2 18:52:21 2024, max compression
```

## Comparing `displaylang-0.23.0b1.tar` & `displaylang-0.24.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-15 19:51:20.086501 displaylang-0.23.0b1/
--rw-r--r--   0 skieffer   (501) staff       (20)    11359 2023-01-14 22:52:28.000000 displaylang-0.23.0b1/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)       61 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/NOTICE
--rw-r--r--   0 skieffer   (501) staff       (20)     2787 2023-01-15 19:51:20.086186 displaylang-0.23.0b1/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)     2368 2023-01-14 22:52:28.000000 displaylang-0.23.0b1/README.md
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-15 19:51:20.081304 displaylang-0.23.0b1/displaylang/
--rw-r--r--   0 skieffer   (501) staff       (20)        0 2023-01-14 22:52:28.000000 displaylang-0.23.0b1/displaylang/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)    21781 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/allow.py
--rw-r--r--   0 skieffer   (501) staff       (20)    18399 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/build.py
--rw-r--r--   0 skieffer   (501) staff       (20)     2622 2023-01-15 19:47:14.000000 displaylang-0.23.0b1/displaylang/builtins.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3870 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/depth.py
--rw-r--r--   0 skieffer   (501) staff       (20)    22435 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/evaluate.py
--rw-r--r--   0 skieffer   (501) staff       (20)     2379 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/exceptions.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3439 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/displaylang/visit.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-15 19:51:20.083193 displaylang-0.23.0b1/displaylang.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)     2787 2023-01-15 19:51:19.000000 displaylang-0.23.0b1/displaylang.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      497 2023-01-15 19:51:20.000000 displaylang-0.23.0b1/displaylang.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-01-15 19:51:19.000000 displaylang-0.23.0b1/displaylang.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       36 2023-01-15 19:51:19.000000 displaylang-0.23.0b1/displaylang.egg-info/requires.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       18 2023-01-15 19:51:19.000000 displaylang-0.23.0b1/displaylang.egg-info/top_level.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       38 2023-01-15 19:51:20.086588 displaylang-0.23.0b1/setup.cfg
--rw-r--r--   0 skieffer   (501) staff       (20)      690 2023-01-15 19:47:18.000000 displaylang-0.23.0b1/setup.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-01-15 19:51:20.085564 displaylang-0.23.0b1/tests/
--rw-r--r--   0 skieffer   (501) staff       (20)        0 2023-01-14 22:52:28.000000 displaylang-0.23.0b1/tests/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4029 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/tests/test_allow.py
--rw-r--r--   0 skieffer   (501) staff       (20)     2687 2023-01-15 19:47:14.000000 displaylang-0.23.0b1/tests/test_builtins.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4945 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/tests/test_call.py
--rw-r--r--   0 skieffer   (501) staff       (20)     7957 2023-01-15 19:05:49.000000 displaylang-0.23.0b1/tests/test_lang_features.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:52:21.414948 displaylang-0.24.0/
+-rw-r--r--   0 skieffer   (501) staff       (20)    11359 2024-04-26 20:27:58.000000 displaylang-0.24.0/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)       61 2024-04-26 20:27:58.000000 displaylang-0.24.0/NOTICE
+-rw-r--r--   0 skieffer   (501) staff       (20)     2974 2024-06-02 18:52:21.414889 displaylang-0.24.0/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)     2368 2024-04-26 20:27:58.000000 displaylang-0.24.0/README.md
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:52:21.412600 displaylang-0.24.0/displaylang/
+-rw-r--r--   0 skieffer   (501) staff       (20)       23 2024-06-02 18:51:32.000000 displaylang-0.24.0/displaylang/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    21781 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/allow.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    26152 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/build.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2731 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/builtins.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3870 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/depth.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    23431 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/evaluate.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2379 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/exceptions.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3439 2024-06-01 21:04:23.000000 displaylang-0.24.0/displaylang/visit.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:52:21.414460 displaylang-0.24.0/displaylang.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)     2974 2024-06-02 18:52:21.000000 displaylang-0.24.0/displaylang.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      495 2024-06-02 18:52:21.000000 displaylang-0.24.0/displaylang.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2024-06-02 18:52:21.000000 displaylang-0.24.0/displaylang.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       69 2024-06-02 18:52:21.000000 displaylang-0.24.0/displaylang.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       12 2024-06-02 18:52:21.000000 displaylang-0.24.0/displaylang.egg-info/top_level.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2024-04-26 20:27:58.000000 displaylang-0.24.0/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      604 2024-06-02 18:52:21.415180 displaylang-0.24.0/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2024-06-02 18:52:21.414160 displaylang-0.24.0/tests/
+-rw-r--r--   0 skieffer   (501) staff       (20)     4029 2024-06-01 21:04:23.000000 displaylang-0.24.0/tests/test_allow.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     2687 2024-06-01 21:04:23.000000 displaylang-0.24.0/tests/test_builtins.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4945 2024-06-01 21:04:23.000000 displaylang-0.24.0/tests/test_call.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     9141 2024-06-01 21:04:23.000000 displaylang-0.24.0/tests/test_lang_features.py
```

### Comparing `displaylang-0.23.0b1/LICENSE` & `displaylang-0.24.0/LICENSE`

 * *Files identical despite different names*

### Comparing `displaylang-0.23.0b1/PKG-INFO` & `displaylang-0.24.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: displaylang
-Version: 0.23.0b1
-Summary: Just enough Python to write displays
-Home-page: https://github.com/proofscape/displaylang
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 # DisplayLang
 
 The problem: Support a limited subset of the Python language, powerful enough
 to allow authors to conveniently build HTML displays based on SymPy classes,
 but limited enough to offer a reasonable expectation of safe evaluation.
 
 We call the language "DisplayLang". It was originally designed for authoring
```

### Comparing `displaylang-0.23.0b1/displaylang/allow.py` & `displaylang-0.24.0/displaylang/allow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/displaylang/build.py` & `displaylang-0.24.0/displaylang/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -25,15 +25,15 @@
 import copy
 
 from .builtins import (
     basic_callables as builtin_basic_callables,
     other_callables as builtin_other_callables,
 )
 from .depth import check_displaylang_dims
-from .evaluate import ExpressionEvaluator, reject
+from .evaluate import ExpressionEvaluator, reject, NestedCodeBlockProcessor
 from .exceptions import ControlledEvaluationException
 
 
 FSTRING_CONVERSION_CODES = {
     115: "!s", 114: "!r", 97: "!a"
 }
 
@@ -65,29 +65,31 @@
 
     def visit_Import(self, node):
         reject('Import statements are not allowed.', node)
 
     def visit_ImportFrom(self, node):
         reject('Import statements are not allowed.', node)
 
-    def visit_Lambda(self, node):
-        reject('Lambdas are not supported.', node)
-
     ###########################################################################
     # Supported statement types.
     # (ast.Expr is already supported in our subclass.)
 
-    def visit_Assign(self, node):
+    def visit_Assign(self, node, use_prebuilt_value=False, prebuilt_value=None):
         """
         Handle any type of assignment, including multiple and unpacking.
         Each assignment is recorded as a local var, available for subsequent
         statements.
         Return list of `Assignment` instances.
+
+        The kwargs concerning "prebuilt values" help us re-use this method in
+        places like our `visit_For` method. The reason we need a separate `user_prebuilt_value`
+        kwarg is because we can't rely on truthiness of the `prebuilt_value` kwarg to tell
+        us whether we want to use it; the desired value could be e.g. False, None, etc.
         """
-        built_value = self.visit(node.value)
+        built_value = prebuilt_value if use_prebuilt_value else self.visit(node.value)
         assignments = []
         for target in node.targets:
             addresses = self.unpack_assignment_target(target, node)
             for target_name, address in addresses.items():
                 v = built_value
                 for i in address:
                     try:
@@ -255,14 +257,179 @@
                     fsv = v.format_spec.values
                     if len(fsv) == 1 and isinstance(fsv[0], ast.Constant):
                         t += ":" + fsv[0].value
                 t += "}"
                 s += t.format(val)
         return s
 
+    ###########################################################################
+
+    def visit_Break(self, node):
+        raise DisplayLangBreakException
+
+    def visit_Continue(self, node):
+        raise DisplayLangContinueException
+
+    def visit_FunctionDef(self, node):
+        self.recurse(node, fields=['args'])
+        p = DisplayLangNestedCodeBlockProcessor(self, node.body,
+                                                signature=node.args, return_just_value=True)
+        name = node.name
+        self.add_current_name(node.name, p)
+        return Assignment(name, p)
+
+    def visit_Lambda(self, node):
+        self.recurse(node, fields=['args'])
+        code = [ast.Return(node.body)]
+        p = DisplayLangNestedCodeBlockProcessor(self, code,
+                                                signature=node.args, return_just_value=True)
+        return p
+
+    def visit_arguments(self, node):
+        self.recurse(node)
+        return node
+
+    def visit_arg(self, node):
+        return node.arg
+
+    def visit_For(self, node):
+        self.recurse(node, fields=['iter'])
+        p = DisplayLangNestedCodeBlockProcessor(self, node.body)
+        for value in node.iter:
+            asgn = ast.Assign([node.target], value)
+            self.visit_Assign(asgn, use_prebuilt_value=True, prebuilt_value=value)
+            try:
+                p()
+            except DisplayLangBreakException:
+                break
+            except DisplayLangContinueException:
+                continue
+        else:
+            if node.orelse:
+                p = DisplayLangNestedCodeBlockProcessor(self, node.orelse)
+                p()
+
+    def visit_If(self, node):
+        self.recurse(node, fields=['test'])
+        code = node.body if node.test else node.orelse
+        p = DisplayLangNestedCodeBlockProcessor(self, code)
+        r, _ = p()
+        # Not sure there's actually any need to return anything here...
+        return r
+
+
+class DisplayLangNestedCodeBlockProcessor(NestedCodeBlockProcessor):
+    """
+    Forms an object which can be invoked (called) in order to evaluate a nested code
+    block, as found in function definitions, and control structures like for-loops
+    and if-else structures.
+
+    May be invoked multiple times, since only a *deep copy* of the nested code block
+    is ever processed and transformed by the evaluation process.
+    """
+
+    def __init__(self, evaluator, body, signature=None, return_just_value=False):
+        """
+        :param evaluator: the DisplayLangEvaluator that wants to process a nested
+            code block.
+        :param body: list of ast statement nodes, representing the block of code
+            to be processed.
+        :param signature: optional `ast.arguments` node, representing expected
+            arguments that can be passed into the evaluation.
+        """
+        NestedCodeBlockProcessor.__init__(self, evaluator)
+        self.body = body
+        self.signature = signature
+        self.return_just_value = return_just_value
+
+    def receive_args(self, *args, **kwargs):
+        """
+        Our job is to interpret the passed args and kwargs according to `self.signature`
+        (which is an ast.arguments in which all of the subfields have been evaluated
+        already), and then store the results as local vars in `self.evaluator`.
+
+        FOR NOW: We are only interpreting the `args` and `defaults` in the signature.
+        This means that we are currently ignoring `kw_defaults`, `kwarg`, `kwonlyargs`,
+        `posonlyargs`, and `vararg`. So, right now, the only type of function signature
+        we support is one with a finite list of pos args, followed immediately (no star)
+        by a finite set of kwargs. In the future, we can try to support everything.
+        """
+
+        # FIXME:
+        #  Should we just be reusing our AllowedCallable class here?
+        #  Didn't we already do all the work of receiving a set of expected arguments?
+
+        sig = self.signature
+        n0 = len(sig.args)
+        k0 = len(sig.defaults)
+        a0 = n0 - k0
+        args0 = sig.args[:a0]
+        kwargs0 = {k: v for k, v in zip(sig.args[-k0:], sig.defaults)}
+
+        a1 = len(args)
+        k1 = len(kwargs)
+        n1 = a1 + k1
+
+        if a1 < a0:
+            raise TypeError(f'Not enough positional args. Expecting {args0}.')
+        if n1 > n0:
+            raise TypeError(f'Too many args. Expecting {sig.args}.')
+
+        keys0 = set(kwargs0.keys())
+        keys1 = set(kwargs.keys())
+        X = keys1 - keys0
+        if X:
+            raise TypeError(f'Unexpected keyword arguments {X}. Expecting {keys0}.')
+
+        new_vars = {}
+        new_vars.update({
+            k: v for k, v in zip(sig.args, args)
+        })
+        for k in sig.args[a1:]:
+            new_vars[k] = kwargs.get(k, kwargs0[k])
+
+        for k, v in new_vars.items():
+            self.evaluator.add_current_name(k, v)
+
+    def __call__(self, *args, **kwargs):
+        """
+        Call the `process_displaylang()` function on the code block, and return its
+        return value.
+        """
+        if self.signature:
+            self.receive_args(*args, **kwargs)
+        code = copy.deepcopy(self.body)
+        ret_val, loc_vars = process_displaylang(
+            code, self.evaluator.basic_vars, self.evaluator.local_vars,
+            self.evaluator.allowed_callables.values(),
+            add_builtins=False,
+            allow_local_var_calls=self.evaluator.allow_local_var_calls,
+            abstract_function_classes=self.evaluator.abstract_function_classes,
+            abstract_relation_classes=self.evaluator.abstract_relation_classes,
+            require_returned_str=False
+        )
+        return ret_val if self.return_just_value else (ret_val, loc_vars)
+
+
+SUPPORTED_STATEMENT_TYPES = (
+    ast.Assign, ast.AugAssign, ast.Expr, ast.Return,
+    ast.FunctionDef, ast.For, ast.If,
+    ast.Break, ast.Continue,
+)
+
+
+class DisplayLangBreakException(Exception):
+    """Raised when a `break` statement is encountered."""
+    ...
+
+
+class DisplayLangContinueException(Exception):
+    """Raised when a `continue` statement is encountered."""
+    ...
+
 
 class DisplayLangProcessor:
     """
     Handles the full process of initial checks, plus parsing and evaluating of
     a string of DisplayLang.
     """
 
@@ -278,87 +445,109 @@
             If -1 (the default), we use half of ``sys.getrecursionlimit()``, i.e.
             half the maximum depth of the Python interpreter stack.
         """
         self.evaluator = evaluator
         self.max_len = max_len
         self.max_depth = max_depth
 
-    def process(self, code, local_vars):
+    def process(self, code, local_vars, require_returned_str=True):
         """
-        Evaluate a string of DisplayLang, and return the generated HTML string,
+        Evaluate some DisplayLang, and return the generated HTML string,
         plus dictionary of newly defined symbols.
 
-        :param code: str
-            The string of DisplayLang that is to be processed.
+        :param code: str, or list of ast nodes
+            Either a string of DisplayLang that still needs to be parsed, or
+            a list of ast nodes representing statements, as results from the
+            parsing process, and typically represents the `body` element of
+            an ast.Module or other control structure, like ast.For or ast.If.
 
         :param local_vars: dict
             The initial local vars that are defined at the start of the
             evaluation. Note: will be extended by any new vars that are defined
             by the DisplayLang code being processed. Pass a copy if you don't
             want the dict to be modified.
 
+        :param require_returned_str: boolean
+            If True (the default) then the given code is required to return a
+            string. If False, then it is not.
+
         :returns: pair (str, dict)
             The string constructed by the code, and the dictionary of all local
             vars defined at the time of the return statement. In particular, this
             will include any new vars defined in the course of the DisplayLang code
             being evaluated.
 
         :raises: ControlledEvaluationException
             if...
                 ...the code is too long or too deep;
                 ...Python AST parser reports a SyntaxError in the code;
-                ...the code contains any statement type other than Assignment,
-                    Expr, or Return;
+                ...the code contains any statement type other than those listed
+                    in the SUPPORTED_STATEMENT_TYPES;
                 ...we encounter a Python AST node type that is not supported, i.e.
                     the code goes outside the subset of Python we support;
                 ...an attempt is made to call a callable that is not allowed;
                 ...an attempt is made to pass unaccepted arguments or argument
                      types to a callable;
                 ...anything goes wrong during building. In particular, this
                     includes the case that the python code contains not a syntax
                     but a runtime error;
+            and, if `require_returned_str` True, then if...
                 ...the return value of the code is not a string;
                 ...the code has no return value.
         """
-        check_displaylang_dims(code, max_len=self.max_len, max_depth=self.max_depth)
+        # Obtain list of statement nodes
+        statement_nodes = []
+        if isinstance(code, list):
+            statement_nodes = code
+        elif isinstance(code, str):
+            check_displaylang_dims(code, max_len=self.max_len, max_depth=self.max_depth)
 
-        try:
-            node = ast.parse(code)
-        except (SyntaxError, MemoryError) as e:
-            # SyntaxError should correspond to a Python syntax error in the given
-            # code. MemoryError should be raised if the code has excessive
-            # complexity, e.g. 300 nested lists etc. We have tried to already
-            # catch such cases with the call to `check_display_build_dims`, but
-            # this is a second chance to try to catch it.
-            msg = 'Error parsing display widget build code.\n' + str(e)
-            raise ControlledEvaluationException(msg) from e
-
-        if not isinstance(node, ast.Module):
-            reject('Outer node should be a Module.')
-
-        for i, stmt in enumerate(node.body):
-            if not isinstance(stmt, (ast.Assign, ast.AugAssign, ast.Expr, ast.Return)):
-                msg = 'Only assignment, expression, and return statements are allowed'
-                msg += f' in DisplayLang, but statement {i} (zero-based) is a {stmt.__class__}.'
-                reject(msg)
+            try:
+                node = ast.parse(code)
+            except (SyntaxError, MemoryError) as e:
+                # SyntaxError should correspond to a Python syntax error in the given
+                # code. MemoryError should be raised if the code has excessive
+                # complexity, e.g. 300 nested lists etc. We have tried to already
+                # catch such cases with the call to `check_display_build_dims`, but
+                # this is a second chance to try to catch it.
+                msg = 'Error parsing display widget build code.\n' + str(e)
+                raise ControlledEvaluationException(msg) from e
 
-        statement_nodes = node.body
+            if not isinstance(node, ast.Module):
+                reject('Outer node should be a Module.')
+
+            statement_nodes = node.body
+        else:
+            reject('code must be either string or list of ast nodes')
+
+        # Check node types
+        for i, stmt in enumerate(statement_nodes):
+            if not isinstance(stmt, SUPPORTED_STATEMENT_TYPES):
+                msg = f'Statement {i} (zero-based) is a {stmt.__class__}.'
+                msg += 'Supported statement types in DisplayLang are: '
+                msg += ', '.join(str(t.__class__) for t in SUPPORTED_STATEMENT_TYPES)
+                reject(msg)
 
         self.evaluator.set_local_vars(local_vars)
 
         def failed_to_return_string():
-            msg = 'DisplayLang code failed to return a string.'
-            raise ControlledEvaluationException(msg)
+            if require_returned_str:
+                msg = 'DisplayLang code failed to return a string.'
+                raise ControlledEvaluationException(msg)
 
         for node in statement_nodes:
             try:
                 result = self.evaluator.visit(node)
             # Re-raise exceptions we have deliberately raised.
             except ControlledEvaluationException as ce:
                 raise ce from None
+            except DisplayLangBreakException as e:
+                raise e from None
+            except DisplayLangContinueException as e:
+                raise e from None
             # After that, we need a catch-all, since the Builder will attempt
             # constructions based on the user's (restricted) Python code, which
             # could easily contain any manner of runtime Python error. E.g. if the
             # user tried to do
             #   foo = f'{1.23:d}'
             # we will try to process the format string in good faith, but it will
             # fail since format code d does not apply to float 1.23.
@@ -370,14 +559,16 @@
                 val = result.value
                 if not isinstance(val, str):
                     failed_to_return_string()
                 return val, local_vars
 
         failed_to_return_string()
 
+        return None, local_vars
+
 
 def make_displaylang_processor(basic_vars,
                         allowed_callables,
                         add_builtins=False,
                         allow_local_var_calls=False,
                         abstract_function_classes=None,
                         abstract_relation_classes=None,
@@ -435,21 +626,23 @@
 def process_displaylang(code, basic_vars, local_vars,
                         allowed_callables,
                         add_builtins=False,
                         allow_local_var_calls=False,
                         abstract_function_classes=None,
                         abstract_relation_classes=None,
                         max_len=0,
-                        max_depth=-1):
+                        max_depth=-1,
+                        require_returned_str=True):
     p = make_displaylang_processor(
         basic_vars, allowed_callables, add_builtins=add_builtins,
         allow_local_var_calls=allow_local_var_calls,
         abstract_function_classes=abstract_function_classes,
         abstract_relation_classes=abstract_relation_classes,
         max_len=max_len, max_depth=max_depth
     )
-    return p.process(code, local_vars)
+    return p.process(code, local_vars, require_returned_str=require_returned_str)
+
 
 # A basic DisplayLangProcessor, supporting the built-in functions and methods:
 basic_displaylang_processor = make_displaylang_processor(
     {}, [], add_builtins=True
 )
```

### Comparing `displaylang-0.23.0b1/displaylang/builtins.py` & `displaylang-0.24.0/displaylang/builtins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -28,31 +28,36 @@
 
 # As the language evolves, we expect the lists of allowed callables to grow.
 
 # The "basic callables" are the ones that will be added to your `basic_vars`
 # in `process_displaylang()` if you set `add_builtins=True` there. They will
 # also be added to the set of allowed callables in this case.
 basic_callables = [
+    c(enumerate, [Any]),
     c(len, [
         [Iterable],
         [s.ANY],
     ]),
+    c(list, [Any]),
     c(range, [t(int)]),
+    c(reversed, [Any]),
     c(str, [Any]),
     c(sum, [
         [Sequence],
         [Sequence, Any],
     ]),
     c(zip, [t(Iterable)]),
 ]
 
 # While the "other callables" will not be added to `basic_vars`, they will be
 # added to the set of allowed callables when you set `add_builtins=True`
 # in `process_displaylang()`.
 other_callables = [
+    c(dict.items, [], method_of=dict),
+
     c(list.append, [Any], method_of=list),
     c(list.extend, [Sequence], method_of=list),
 
     c(str.join, [Sequence[str]], method_of=s.ANY),
     c(str.lower, [], method_of=s.ANY),
     c(str.replace, [s.ANY, s.ANY], method_of=s.ANY),
     c(str.split, [
```

### Comparing `displaylang-0.23.0b1/displaylang/depth.py` & `displaylang-0.24.0/displaylang/depth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/displaylang/evaluate.py` & `displaylang-0.24.0/displaylang/evaluate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -228,14 +228,20 @@
     # record a helpful error message (if called for).
     banned_builtin_callables = {
         exec: None,
         eval: None,
         # The problem with `map` is that it carries out a function call which we do
         # not get to visit, meaning it gets around the safety provided by our
         # `visit_Call()` method. Display authors should use comprehensions instead.
+        # FIXME:
+        #  Maybe we should just make the name `map` point to a function of our
+        #  own, which will do the same thing, but perform the function calls
+        #  using our safe evaluator.
+        #  ...In the same way, maybe `exec` and `eval` could just point to our
+        #  own safe executor and evaluator.
         map: "`map` is not supported. Use a list comprehension instead.",
     }
 
     def __init__(self, basic_vars=None, local_vars=None,
                  allow_local_var_calls=False,
                  abstract_function_classes=None,
                  abstract_relation_classes=None):
@@ -387,14 +393,18 @@
             logging.info('<called as abstract function>')
             return F(*A, **K)
 
         if self.allow_local_var_calls and F in self.local_vars.values():
             logging.info('<called as local var>')
             return F(*A, **K)
 
+        if isinstance(F, NestedCodeBlockProcessor):
+            logging.info('<called as NestedCodeBlockProcessor>')
+            return F(*A, **K)
+
         if type(F) in self.dunder_callables:
             logging.info('<called as dunder callable>')
             A = [F] + A
             dc = self.dunder_callables[type(F)]
             return dc(*A, **K)
 
         if is_builtin_method(F) or type(F) == types.MethodType:
@@ -586,7 +596,22 @@
         visit the AST.
     :param s: the string to be parsed into an AST, then visited.
     :return: the return value of `expression_evaluator.visit()`.
     """
     node = ast.parse(s)
     node = ast.Expr(node.body[0].value)
     return expression_evaluator.visit(node)
+
+
+class NestedCodeBlockProcessor:
+    """
+    Abstract base class, defined here to help break cyclic import issues.
+    The important subclass is `DisplayLangNestedCodeBlockProcessor`, defined in build.py,
+    but we need the class for an `isinstance()` check here in evaluate.py, in `ControlledEvaluator`.
+    """
+
+    def __init__(self, evaluator):
+        """
+        :param evaluator: the ControlledEvaluator that wants to process a nested
+            code block.
+        """
+        self.evaluator = evaluator
```

### Comparing `displaylang-0.23.0b1/displaylang/exceptions.py` & `displaylang-0.24.0/displaylang/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/displaylang/visit.py` & `displaylang-0.24.0/displaylang/visit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/displaylang.egg-info/PKG-INFO` & `displaylang-0.24.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: displaylang
-Version: 0.23.0b1
+Version: 0.24.0
 Summary: Just enough Python to write displays
 Home-page: https://github.com/proofscape/displaylang
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: pfsc-util>=0.22.8
+Requires-Dist: typeguard==2.13.3
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: invoke; extra == "dev"
 
 # DisplayLang
 
 The problem: Support a limited subset of the Python language, powerful enough
 to allow authors to conveniently build HTML displays based on SymPy classes,
 but limited enough to offer a reasonable expectation of safe evaluation.
```

### Comparing `displaylang-0.23.0b1/tests/test_allow.py` & `displaylang-0.24.0/tests/test_allow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/tests/test_builtins.py` & `displaylang-0.24.0/tests/test_builtins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/tests/test_call.py` & `displaylang-0.24.0/tests/test_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
```

### Comparing `displaylang-0.23.0b1/tests/test_lang_features.py` & `displaylang-0.24.0/tests/test_lang_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------- #
 #   DisplayLang                                                               #
 #                                                                             #
-#   Copyright (c) 2020-2023 DisplayLang Contributors                          #
+#   Copyright (c) 2020-2024 DisplayLang Contributors                          #
 #                                                                             #
 #   Licensed under the Apache License, Version 2.0 (the "License");           #
 #   you may not use this file except in compliance with the License.          #
 #   You may obtain a copy of the License at                                   #
 #                                                                             #
 #       http://www.apache.org/licenses/LICENSE-2.0                            #
 #                                                                             #
@@ -148,14 +148,80 @@
 """
 
 build_14 = """
 # This involves an empty comprehension:
 return str(['foo' for r in range(2, 2)])
 """
 
+build_15 = """
+def foo(a, b, c=7, d=11):
+    e = 2*a
+    return b + c + d + e
+return str(foo(3, 5))
+"""
+
+build_16 = """
+if 3 > 7:
+    x = 2
+elif 1 > 9:
+    x = 3
+else:
+    x = 4
+return str(x)
+"""
+
+build_17 = """
+n = 0
+for a, b in zip([1, 2, 3], [1, 4, 9]):
+    n += a + b
+return str(n)
+"""
+
+build_18 = """
+x = 4
+if 3 > 7:
+    x = 2
+return str(x)
+"""
+
+build_19 = """
+n = 0
+for a, b in zip([1, 2, 3], [1, 4, 9]):
+    n += a + b
+    if n > 5:
+        break
+else:
+    n = 1
+return str(n)
+"""
+
+build_20 = """
+n = 0
+for a, b in zip([1, 2, 3], [1, 4, 9]):
+    n += a + b
+    if n > 30:
+        break
+else:
+    n = 1
+return str(n)
+"""
+
+build_21 = """
+n = 0
+for a, b in zip([1, 2, 3], [1, 4, 9]):
+    if a % 2 == 1:
+        continue
+    n += a + b
+return str(n)
+"""
+
+build_22 = """
+foo = lambda a, b, c=7, d=11: b + c + d + 2*a 
+return str(foo(3, 5))
+"""
 
 @pytest.mark.parametrize('code, s_exp, d_exp', [
     [build_00, 'foobar', {'s': 'foo', 't': 'foobar'}],
     [build_01, '10', {'a': 5, 'b': 10}],
     [build_02, '[4, 6, 10, 14]', {'foo': [4, 6, 10, 14]}],
     [build_03, '[8, 18]', {'foo2': [8, 18]}],
     [build_04, '[6, 10, 14]', {'foo': [6, 10, 14]}],
@@ -165,24 +231,33 @@
     [build_08, '{0: 0, 1: 1, 2: 4, 3: 9}', {}],
     [build_09, '{0, 1, 4, 9}', {}],
     [build_10, '3 -1 30 1.25 3 4 32 28 1 14 6 8', {}],
     [build_11, '7 -7 False -8 False True', {}],
     [build_12, '2', {'a': 2}],
     [build_13, '13', {'a': 1, 'b': 2, 'c': 3, 'f': 1, 'g': (2, 3), 'p': [1, (2, 3)]}],
     [build_14, '[]', {}],
+    [build_15, '29', None],
+    [build_16, '4', {'x': 4}],
+    [build_17, '20', {'n': 20, 'a': 3, 'b': 9}],
+    [build_18, '4', {'x': 4}],
+    [build_19, '8', {'n': 8, 'a': 2, 'b': 4}],
+    [build_20, '1', {'n': 1, 'a': 3, 'b': 9}],
+    [build_21, '6', {'n': 6, 'a': 3, 'b': 9}],
+    [build_22, '29', None],
 ])
 def test_build(code, s_exp, d_exp):
     s, d = process_displaylang(code, {}, {}, [], add_builtins=True)
     interactive = False
     if interactive:
         print()
         print(s)
         print(d)
     assert s == s_exp
-    assert d == d_exp
+    if d_exp is not None:
+        assert d == d_exp
 
 
 def test_build_with_fixed_processor():
     """
     Try using a fixed DisplayLangProcessor, to process multiple code strings.
     """
     cases = [
```

