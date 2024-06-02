# Comparing `tmp/django-relations-iterator-0.0.4.tar.gz` & `tmp/django_relations_iterator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-relations-iterator-0.0.4.tar", last modified: Thu Oct 14 12:07:56 2021, max compression
+gzip compressed data, was "django_relations_iterator-0.0.5.tar", last modified: Sun Jun  2 11:02:55 2024, max compression
```

## Comparing `django-relations-iterator-0.0.4.tar` & `django_relations_iterator-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/
--rw-rw-r--   0 scrat     (1000) scrat     (1000)     1072 2021-10-14 10:05:52.000000 django-relations-iterator-0.0.4/LICENSE
--rw-rw-r--   0 scrat     (1000) scrat     (1000)     8205 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/PKG-INFO
--rw-rw-r--   0 scrat     (1000) scrat     (1000)     7595 2021-10-14 12:06:19.000000 django-relations-iterator-0.0.4/README.md
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      104 2021-10-14 10:20:16.000000 django-relations-iterator-0.0.4/pyproject.toml
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      698 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/setup.cfg
-drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/src/
-drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/
--rw-rw-r--   0 scrat     (1000) scrat     (1000)     8205 2021-10-14 12:07:56.000000 django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/PKG-INFO
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      398 2021-10-14 12:07:56.000000 django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/SOURCES.txt
--rw-rw-r--   0 scrat     (1000) scrat     (1000)        1 2021-10-14 12:07:56.000000 django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/dependency_links.txt
--rw-rw-r--   0 scrat     (1000) scrat     (1000)       19 2021-10-14 12:07:56.000000 django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/top_level.txt
-drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2021-10-14 12:07:56.177516 django-relations-iterator-0.0.4/src/relations_iterator/
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      172 2021-10-14 10:49:08.000000 django-relations-iterator-0.0.4/src/relations_iterator/__init__.py
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      777 2021-10-14 11:06:47.000000 django-relations-iterator-0.0.4/src/relations_iterator/iterator.py
--rw-rw-r--   0 scrat     (1000) scrat     (1000)     2922 2021-10-14 10:05:52.000000 django-relations-iterator-0.0.4/src/relations_iterator/relation_tree.py
--rw-rw-r--   0 scrat     (1000) scrat     (1000)      173 2021-10-14 11:07:00.000000 django-relations-iterator-0.0.4/src/relations_iterator/visitor.py
+drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)     1072 2024-06-01 14:42:06.000000 django_relations_iterator-0.0.5/LICENSE
+-rw-r--r--   0 scrat     (1000) scrat     (1000)     9192 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/PKG-INFO
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)     8619 2024-06-02 10:52:13.000000 django_relations_iterator-0.0.5/README.md
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      104 2024-06-01 14:42:06.000000 django_relations_iterator-0.0.5/pyproject.toml
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      698 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/setup.cfg
+drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/src/
+drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/
+-rw-r--r--   0 scrat     (1000) scrat     (1000)     9192 2024-06-02 11:02:55.000000 django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/PKG-INFO
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      430 2024-06-02 11:02:55.000000 django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/SOURCES.txt
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)        1 2024-06-02 11:02:55.000000 django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/dependency_links.txt
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)       19 2024-06-02 11:02:55.000000 django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/top_level.txt
+drwxrwxr-x   0 scrat     (1000) scrat     (1000)        0 2024-06-02 11:02:55.641123 django_relations_iterator-0.0.5/src/relations_iterator/
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      211 2024-06-02 10:36:43.000000 django_relations_iterator-0.0.5/src/relations_iterator/__init__.py
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      911 2024-06-02 10:36:43.000000 django_relations_iterator-0.0.5/src/relations_iterator/clone.py
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      777 2024-06-01 14:42:06.000000 django_relations_iterator-0.0.5/src/relations_iterator/iterator.py
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)     2922 2024-06-01 14:42:06.000000 django_relations_iterator-0.0.5/src/relations_iterator/relation_tree.py
+-rw-rw-r--   0 scrat     (1000) scrat     (1000)      173 2024-06-01 14:42:06.000000 django_relations_iterator-0.0.5/src/relations_iterator/visitor.py
```

### Comparing `django-relations-iterator-0.0.4/LICENSE` & `django_relations_iterator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-relations-iterator-0.0.4/PKG-INFO` & `django_relations_iterator-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: django-relations-iterator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to iterate over django relation tree
 Home-page: https://github.com/regqueryvalueex/django-relations-iterator
 Author: Alex Zayets
 Author-email: alex.consp@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/regqueryvalueex/django-relations-iterator/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-relations-Iterator
 
-Provides utilities for iterating over django model instances hierarchy
+Provides utilities for iterating over django model instances hierarchy. Provides easy out-of-the-box way to clone django instances.
+
+Reasoning and solution for use case with cloning - https://hackernoon.com/the-smart-way-to-clone-django-instances
 
 ## Example:
 #### Simple instances tree clone
 
 
 ```python
 #models.py
@@ -59,50 +59,48 @@
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     description = models.TextField(max_length=3000)
 
 ```
 
 ```python
 #clone.py
-from relations_iterator import TreeNode, AbstractVisitor, RelationTreeIterator, ConfigurableRelationTree
+from relations_iterator import clone, CloneVisitor
 from .models import Meeting
 
 # because of config, tree will ignore comments, but will consider all participations and invitations
 CLONE_STRUCTURE = {
     'participations': {
         'invitations': {}
     }
 }
 
+        
+meeting = Meeting.objects.last()
+clone(meeting, CLONE_STRUCTURE, CloneVisitor())
 
-class CloneVisitor(AbstractVisitor):
-    def visit(self, node: TreeNode):
-        node.instance.pk = None
-        if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
-            setattr(
-                node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
-            )
-        node.instance.save()
+```
 
+#### Customizing cloning process
 
-def clone(instance, config):
-    
-    visitor = CloneVisitor()
-    tree = ConfigurableRelationTree(root=instance, structure=config)
-    for node in RelationTreeIterator(tree=tree):
-        visitor.visit(node)
+```python
 
-        
-meeting = Meeting.objects.last()
-clone(meeting, CLONE_STRUCTURE)
+# Example: you want to set title for cloned Meeting as {original_title}-COPY 
+# and set time of the instance to None
+class CustomCloneVisitor(CloneVisitor):
+    @singledispatchmethod
+    def customize(self, instance):
+        pass
+
+    @customize.register
+    def _(self, instance: Meeting):
+        instance.title = f'{instance.title}-COPY'
+        instance.time = None
 
 ```
+
 ## Installation
 
 ```shell
 pip install django-relations-iterator
 ```
 
 ## Features
@@ -188,33 +186,68 @@
 
 ```python
 from relations_iterator import AbstractVisitor
 ```
 
 Provides abstract class, with interface to implement visitor pattern. You must implement `.visit(node)` method, to complete implementation
 
+
+### Instances cloning feature
+
+```python
+from relations_iterator import clone, CloneVisitor
+```
+
+Provides function to clone instances and simple CloneVisitor class, just as explained below in examples section.
+
+`clone` function accepts 3 arguments:
+
+- `instance` - django Model instance, that needs to be cloned
+- `config` - config dictionary of the structure that needs to be cloned
+- `visitor` - visitor instance. `CloneVisitor` can be used directly or you can customize it and pass your own implementation
+
+Config explanation:
+
+Example:
+```python
+
+# Config for cloning Meeting instance, we want to clone also participation's and invitations
+config = {
+    'participations': {  # related name for `Participation` model, that have fk to Meeting
+        'invitations': {}  # related name for `Invitation` model, that have fk to `Participation` model
+    }
+}
+# All other relations will be skipped, as they are not listed in config
+```
+
+
 #### Examples:
-#### Clone visitor
+#### Clone visitor full implementation
 
 ```python
-from relations_iterator import TreeNode
+from django.db.models import Model
+from relations_iterator import TreeNode, AbstractVisitor
 
 
 class CloneVisitor(AbstractVisitor):
     def visit(self, node: TreeNode):
         node.instance.pk = None
         if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
+            parent_joining_field, instance_joining_field = node.relation.get_joining_fields()[0]
             setattr(
                 node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
+                instance_joining_field.attname,
+                parent_joining_field.value_from_object(node.parent.instance)
             )
+        self.customize(node.instance)
         node.instance.save()
 
+    def customize(self, instance: Model) -> None:
+        pass
+
 ```
 
 Clone visitor will clone every instance in hierarchy and set proper parent, so it can be used to implement instance hierarchy clone
 
 ```python
 CLONE_STRUCTURE = {
     'participations': {
@@ -276,9 +309,7 @@
 ```python
 # Output
 [<TreeNode for Meeting: Meeting object (2)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (3)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (3)>, <TreeNode for Invitation: Invitation object (2)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (4)>]
 ```
-
-
```

### Comparing `django-relations-iterator-0.0.4/README.md` & `django_relations_iterator-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # django-relations-Iterator
 
-Provides utilities for iterating over django model instances hierarchy
+Provides utilities for iterating over django model instances hierarchy. Provides easy out-of-the-box way to clone django instances.
+
+Reasoning and solution for use case with cloning - https://hackernoon.com/the-smart-way-to-clone-django-instances
 
 ## Example:
 #### Simple instances tree clone
 
 
 ```python
 #models.py
@@ -42,50 +44,48 @@
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     description = models.TextField(max_length=3000)
 
 ```
 
 ```python
 #clone.py
-from relations_iterator import TreeNode, AbstractVisitor, RelationTreeIterator, ConfigurableRelationTree
+from relations_iterator import clone, CloneVisitor
 from .models import Meeting
 
 # because of config, tree will ignore comments, but will consider all participations and invitations
 CLONE_STRUCTURE = {
     'participations': {
         'invitations': {}
     }
 }
 
+        
+meeting = Meeting.objects.last()
+clone(meeting, CLONE_STRUCTURE, CloneVisitor())
 
-class CloneVisitor(AbstractVisitor):
-    def visit(self, node: TreeNode):
-        node.instance.pk = None
-        if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
-            setattr(
-                node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
-            )
-        node.instance.save()
+```
 
+#### Customizing cloning process
 
-def clone(instance, config):
-    
-    visitor = CloneVisitor()
-    tree = ConfigurableRelationTree(root=instance, structure=config)
-    for node in RelationTreeIterator(tree=tree):
-        visitor.visit(node)
+```python
 
-        
-meeting = Meeting.objects.last()
-clone(meeting, CLONE_STRUCTURE)
+# Example: you want to set title for cloned Meeting as {original_title}-COPY 
+# and set time of the instance to None
+class CustomCloneVisitor(CloneVisitor):
+    @singledispatchmethod
+    def customize(self, instance):
+        pass
+
+    @customize.register
+    def _(self, instance: Meeting):
+        instance.title = f'{instance.title}-COPY'
+        instance.time = None
 
 ```
+
 ## Installation
 
 ```shell
 pip install django-relations-iterator
 ```
 
 ## Features
@@ -171,33 +171,68 @@
 
 ```python
 from relations_iterator import AbstractVisitor
 ```
 
 Provides abstract class, with interface to implement visitor pattern. You must implement `.visit(node)` method, to complete implementation
 
+
+### Instances cloning feature
+
+```python
+from relations_iterator import clone, CloneVisitor
+```
+
+Provides function to clone instances and simple CloneVisitor class, just as explained below in examples section.
+
+`clone` function accepts 3 arguments:
+
+- `instance` - django Model instance, that needs to be cloned
+- `config` - config dictionary of the structure that needs to be cloned
+- `visitor` - visitor instance. `CloneVisitor` can be used directly or you can customize it and pass your own implementation
+
+Config explanation:
+
+Example:
+```python
+
+# Config for cloning Meeting instance, we want to clone also participation's and invitations
+config = {
+    'participations': {  # related name for `Participation` model, that have fk to Meeting
+        'invitations': {}  # related name for `Invitation` model, that have fk to `Participation` model
+    }
+}
+# All other relations will be skipped, as they are not listed in config
+```
+
+
 #### Examples:
-#### Clone visitor
+#### Clone visitor full implementation
 
 ```python
-from relations_iterator import TreeNode
+from django.db.models import Model
+from relations_iterator import TreeNode, AbstractVisitor
 
 
 class CloneVisitor(AbstractVisitor):
     def visit(self, node: TreeNode):
         node.instance.pk = None
         if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
+            parent_joining_field, instance_joining_field = node.relation.get_joining_fields()[0]
             setattr(
                 node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
+                instance_joining_field.attname,
+                parent_joining_field.value_from_object(node.parent.instance)
             )
+        self.customize(node.instance)
         node.instance.save()
 
+    def customize(self, instance: Model) -> None:
+        pass
+
 ```
 
 Clone visitor will clone every instance in hierarchy and set proper parent, so it can be used to implement instance hierarchy clone
 
 ```python
 CLONE_STRUCTURE = {
     'participations': {
```

### Comparing `django-relations-iterator-0.0.4/setup.cfg` & `django_relations_iterator-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-relations-iterator
-version = 0.0.4
+version = 0.0.5
 author = Alex Zayets
 author_email = alex.consp@gmail.com
 description = Tool to iterate over django relation tree
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/regqueryvalueex/django-relations-iterator
 project_urls =
```

### Comparing `django-relations-iterator-0.0.4/src/django_relations_iterator.egg-info/PKG-INFO` & `django_relations_iterator-0.0.5/src/django_relations_iterator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: django-relations-iterator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool to iterate over django relation tree
 Home-page: https://github.com/regqueryvalueex/django-relations-iterator
 Author: Alex Zayets
 Author-email: alex.consp@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/regqueryvalueex/django-relations-iterator/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # django-relations-Iterator
 
-Provides utilities for iterating over django model instances hierarchy
+Provides utilities for iterating over django model instances hierarchy. Provides easy out-of-the-box way to clone django instances.
+
+Reasoning and solution for use case with cloning - https://hackernoon.com/the-smart-way-to-clone-django-instances
 
 ## Example:
 #### Simple instances tree clone
 
 
 ```python
 #models.py
@@ -59,50 +59,48 @@
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
     description = models.TextField(max_length=3000)
 
 ```
 
 ```python
 #clone.py
-from relations_iterator import TreeNode, AbstractVisitor, RelationTreeIterator, ConfigurableRelationTree
+from relations_iterator import clone, CloneVisitor
 from .models import Meeting
 
 # because of config, tree will ignore comments, but will consider all participations and invitations
 CLONE_STRUCTURE = {
     'participations': {
         'invitations': {}
     }
 }
 
+        
+meeting = Meeting.objects.last()
+clone(meeting, CLONE_STRUCTURE, CloneVisitor())
 
-class CloneVisitor(AbstractVisitor):
-    def visit(self, node: TreeNode):
-        node.instance.pk = None
-        if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
-            setattr(
-                node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
-            )
-        node.instance.save()
+```
 
+#### Customizing cloning process
 
-def clone(instance, config):
-    
-    visitor = CloneVisitor()
-    tree = ConfigurableRelationTree(root=instance, structure=config)
-    for node in RelationTreeIterator(tree=tree):
-        visitor.visit(node)
+```python
 
-        
-meeting = Meeting.objects.last()
-clone(meeting, CLONE_STRUCTURE)
+# Example: you want to set title for cloned Meeting as {original_title}-COPY 
+# and set time of the instance to None
+class CustomCloneVisitor(CloneVisitor):
+    @singledispatchmethod
+    def customize(self, instance):
+        pass
+
+    @customize.register
+    def _(self, instance: Meeting):
+        instance.title = f'{instance.title}-COPY'
+        instance.time = None
 
 ```
+
 ## Installation
 
 ```shell
 pip install django-relations-iterator
 ```
 
 ## Features
@@ -188,33 +186,68 @@
 
 ```python
 from relations_iterator import AbstractVisitor
 ```
 
 Provides abstract class, with interface to implement visitor pattern. You must implement `.visit(node)` method, to complete implementation
 
+
+### Instances cloning feature
+
+```python
+from relations_iterator import clone, CloneVisitor
+```
+
+Provides function to clone instances and simple CloneVisitor class, just as explained below in examples section.
+
+`clone` function accepts 3 arguments:
+
+- `instance` - django Model instance, that needs to be cloned
+- `config` - config dictionary of the structure that needs to be cloned
+- `visitor` - visitor instance. `CloneVisitor` can be used directly or you can customize it and pass your own implementation
+
+Config explanation:
+
+Example:
+```python
+
+# Config for cloning Meeting instance, we want to clone also participation's and invitations
+config = {
+    'participations': {  # related name for `Participation` model, that have fk to Meeting
+        'invitations': {}  # related name for `Invitation` model, that have fk to `Participation` model
+    }
+}
+# All other relations will be skipped, as they are not listed in config
+```
+
+
 #### Examples:
-#### Clone visitor
+#### Clone visitor full implementation
 
 ```python
-from relations_iterator import TreeNode
+from django.db.models import Model
+from relations_iterator import TreeNode, AbstractVisitor
 
 
 class CloneVisitor(AbstractVisitor):
     def visit(self, node: TreeNode):
         node.instance.pk = None
         if node.parent is not None:
-            parent_joining_column, instance_joining_column = node.relation.get_joining_columns()[0]
+            parent_joining_field, instance_joining_field = node.relation.get_joining_fields()[0]
             setattr(
                 node.instance,
-                instance_joining_column,
-                getattr(node.parent.instance, parent_joining_column)
+                instance_joining_field.attname,
+                parent_joining_field.value_from_object(node.parent.instance)
             )
+        self.customize(node.instance)
         node.instance.save()
 
+    def customize(self, instance: Model) -> None:
+        pass
+
 ```
 
 Clone visitor will clone every instance in hierarchy and set proper parent, so it can be used to implement instance hierarchy clone
 
 ```python
 CLONE_STRUCTURE = {
     'participations': {
@@ -276,9 +309,7 @@
 ```python
 # Output
 [<TreeNode for Meeting: Meeting object (2)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (3)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (3)>, <TreeNode for Invitation: Invitation object (2)>]
 [<TreeNode for Meeting: Meeting object (2)>, <TreeNode for Participation: Participation object (4)>]
 ```
-
-
```

### Comparing `django-relations-iterator-0.0.4/src/relations_iterator/iterator.py` & `django_relations_iterator-0.0.5/src/relations_iterator/iterator.py`

 * *Files identical despite different names*

### Comparing `django-relations-iterator-0.0.4/src/relations_iterator/relation_tree.py` & `django_relations_iterator-0.0.5/src/relations_iterator/relation_tree.py`

 * *Files identical despite different names*

